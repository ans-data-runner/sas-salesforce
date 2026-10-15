# SAS KPI review pack: PBIX file breakdown

The four Power BI files in the 15/10/2026 SAS review pack, decoded from their data models and report definitions. Each file has its purpose, data sources (full SQL / Power Query M), tables and columns, relationships, DAX measures, report pages and visuals, filters, and observations relevant to rebuilding the KPI in Microsoft Fabric.

**Context:** SAS International is a manufacturer whose ERP is Infor SyteLine (CloudSuite Industrial, SQL Server; site `RBMW`, warehouses BE = Bridgend, MB = Maybole, RDG = Reading). The KPIs are being rebuilt in a Fabric medallion platform into a weekly KPI result table. Each row there holds week ending Friday, target, actual and RAG.

| # | File | KPI it supports | Source system |
|---|---|---|---|
| 1 | OTIF Dashboard.pbix | Manufacturing Bridgend & Maybole: Delivery (OTIF to delivery date), target 95% | SyteLine SQL (`SAS_OTIF_mst`, live DB) |
| 2 | SOP - Cost KPI - UAT.pbix | Sales Order Processing: Cost (£/FTE = order value completed / FTE), target £33,026 | SyteLine SQL (UAT DB) + SharePoint Excel |
| 3 | Product Eng BE - Quality KPI.pbix | Product Engineering Bridgend: Quality, numerator (count of BOM Helpdesk tickets) | SharePoint list |
| 4 | Product Eng MB - Quality KPI.pbix | Product Engineering Maybole: Quality, numerator (count of SafetyCulture issues) | SafetyCulture (iAuditor) connector |

---

## 1. OTIF Dashboard.pbix

**Purpose:** Weekly OTIF % by supplying site, with failure analysis. Built by Matt (SAS) on top of Sarah's SyteLine OTIF tables. Rob's email says to switch the database from `RBMW_Live` to `RBMW_UAT` for development.

### Data model
| Table | Type | Columns |
|---|---|---|
| `Query1` | Native SQL (Import) | Line, Group, ShipDate, AcknowledgedDate, Whse, Customer, ShipmentDetail, OTIF, Commment, FailCode, rowpointer, CoNum, Year, Week, SiteRef, Department, FailNote, FailureMode, Uf_MaterialGroup, Project, Name, ProjectName, Region, DrivingDate, QtyOS, LineCount, Included, DateChangeReason, ShowOnDashboard |
| `Date` | DAX calculated table | Date, WeekNo, Year, Month, MonthNo, DayofMonthNo, WeekYear, YearWeekNo, YearMonth, YearMonthNo |

**Relationship:** `Query1[DrivingDate]` → `Date[Date]` (many-to-one, single direction, active).

### Source query: `Query1` (Power Query M with native SQL)
Server `sas-erp-sql01.erp.sas`, database `RBMW_Live`:
```
let
    Source = Sql.Database("sas-erp-sql01.erp.sas", "RBMW_Live", [Query="SELECT 
    -- OTIF Core Fields
    otif.Line,
    otif.[Group],
    CASE
        WHEN otif.ShipDate IS NULL THEN otif.AcknowledgedDate
        ELSE otif.ShipDate
    END AS DrivingDate,
    otif.ShipDate,
    otif.AcknowledgedDate,
    otif.Whse,
    otif.Customer,
    otif.ShipmentDetail,
    CASE 
        WHEN otif.ShipDate IS NULL THEN 'OUTSTANDING'
        WHEN otif.OTIF = 0 THEN 'NOT ON TIME IN FULL'
        ELSE 'ON TIME IN FULL'
    END AS OTIF,
    otif.Commment,
    otif.FailCode,
    otif.rowpointer,
    otif.CoNum,
    otif.[Year],
    otif.[Week],
    otif.SiteRef,
    otif.QtyOS,
    otif.LineCount,
    otif.Included,
    CASE
        WHEN otif.ShipDate IS NULL OR otif.Included = 1 THEN 1
        ELSE 0
    END AS ShowOnDashboard,
    
    -- Failure Details
    otif_fail.Department,
    otif_fail.FailNote,
    otif_fail.FailureMode,
    
    -- Order Details
    oh.Uf_MaterialGroup,
    
    -- Project Information
    proj.Project,
    proj.Name,
    CONCAT(proj.Project, ' - ', proj.Name) AS ProjectName,

    -- Customer Region
    cust.description AS Region,

    -- Date Change Reason
    date_change.Reason AS DateChangeReason

FROM [RBMW_Live].[dbo].[SAS_OTIF_mst] AS otif

LEFT JOIN [RBMW_Live].[dbo].[SAS_OTIF_Fail_mst] AS otif_fail 
    ON otif.CoNum = otif_fail.CoNum 
    AND otif.Whse = otif_fail.Whse 
    AND otif.AcknowledgedDate = otif_fail.AcknowledgedDate

LEFT JOIN [RBMW_Live].[dbo].[co_mst] AS oh 
    ON otif.CoNum = oh.co_num AND oh.site_ref = 'RBMW'

LEFT JOIN [RBMW_Live].[dbo].[SASproject] AS proj 
    ON oh.Uf_Project = proj.Project

LEFT JOIN [RBMW_Live].[dbo].endtype_mst AS cust 
    ON cust.end_user_type = oh.end_user_type AND cust.site_ref = oh.site_ref


LEFT JOIN (
    SELECT co_num, Reason,
           ROW_NUMBER() OVER (PARTITION BY co_num ORDER BY changeDate DESC) AS rn
    FROM [RBMW_Live].[dbo].[SAS_CoDueDateLog_mst]
) AS date_change
    ON otif.CoNum = date_change.co_num
    AND date_change.rn = 1"])
in
    Source
```
Source tables: `SAS_OTIF_mst` (custom SAS OTIF event table: one row per delivery event = order + warehouse + acknowledged date), `SAS_OTIF_Fail_mst` (failure reason codes), `co_mst`, `SASproject` (custom), `endtype_mst` (region), `SAS_CoDueDateLog_mst` (custom date-change log).

### Date table (DAX)
```
VAR MinYear = DATE(2000,1,1)
VAR MaxYear = DATE(2030,12,31)
RETURN
ADDCOLUMNS (
    CALENDAR(MinYear,MaxYear),
    "WeekNo", WEEKNUM([Date]),
    "Year", YEAR([Date]),
    "Month", FORMAT([Date], "MMM"),
    "MonthNo", MONTH([Date]),
    "DayofMonthNo", Day([Date]),
    "WeekYear", YEAR([Date]) & " " & WEEKNUM([Date]),
    "YearWeekNo", YEAR([Date]) & FORMAT(WEEKNUM([Date]),"00"),
    "YearMonth", YEAR([Date]) & " " & MONTH([Date]),
    "YearMonthNo", YEAR([Date]) & FORMAT(Month([Date]),"00")
)
```
`WEEKNUM()` with no second argument uses Sunday-start weeks with week 1 containing 1 January. These are **not** ISO weeks and not Friday-ending weeks.

### DAX measures (table `Query1`)
```
OTIF (%) :=
DIVIDE(
    CALCULATE(COUNTROWS(Query1), Query1[OTIF] = "ON TIME IN FULL" && Query1[Included] = 1),
    CALCULATE(COUNTROWS(Query1), Query1[Included] = 1)
)

OTIF Target := 0.95
```

### Report pages and visuals
| Page | Visuals |
|---|---|
| OTIF dashboard | Card: `OTIF (%)`. Line + stacked column "Weekly OTIF": axis `Date[WeekYear]`, columns split by `Query1[OTIF]` status, lines `OTIF (%)` and `OTIF Target`. Slicers: Whse (supplying site), Year, Region, ProjectName, Customer |
| OTIF fail details | Column chart "Weekly OTIF Fails" (`Date[WeekNo]`, `OTIF`, `OTIF (%)`). Table: AcknowledgedDate, CoNum, Customer, Department, FailNote, FailureMode, ProjectName, Region, ShipDate, Whse. Slicers: Year, Customer, ProjectName, Whse, Region. Page filter on `OTIF` |
| Missing OTIF Reasons | Cards: count of CoNum filtered to Whse = 'BE' / 'MB' / 'RDG'. Column chart "OTIF Fails missing reason codes". Detail table. Page filters on OTIF, Department, FailCode, FailNote, FailureMode |
| Failure Analysis | Donuts: "Failure by Failure Mode", "Failure by Department" (count of CoNum). Slicers: ProjectName, Customer, Year, Region, Whse |
| OTIF Definition | Text-only explanation (summarised below) |

**Report-level filters:**
- `Date[Date]` relative date, the last 1 year up to today.
- `Query1[ShowOnDashboard] = 1`.
- `Query1[DateChangeReason]`, categorical, with no values selected.

### Business definition (from the "OTIF Definition" page)
- OTIF is measured **per delivery event**. An order shipping lines from different sites or on different dates produces one OTIF event per site/date. If any line in the event is not on time and in full, the event fails.
- It is measured against the **Original Acknowledged Date** if populated. It uses the Customer Delivery Date instead if that's blank or the "Customer Request" box is ticked (a re-date at the customer's request is not counted as a fail).
- The "Same Day Shipment" flag is used when an order is dispatched and delivered the same day. Normally orders ship the day before delivery.
- UK orders are measured on delivery to the customer; export orders on dispatch date. Internal material transfers are removed from UK orders to avoid double counting.
- Region comes from End User Type on the customer order header. Reason codes are entered via the "SAS OTIF Fails" form.

### Observations for the rebuild
1. The KPI = `count(events where ShipDate not null AND OTIF <> 0 AND Included = 1) / count(events where Included = 1)`, per Whse, per week of DrivingDate. Outstanding events (ShipDate null) with Included = 1 sit in the denominator and count as fails.
2. In the SQL, `OTIF IS NULL` with a ShipDate falls to the `ELSE` branch, so it's treated as ON TIME IN FULL.
3. `COUNTROWS(Query1)` counts rows **after** the LEFT JOIN to `SAS_OTIF_Fail_mst`. If an event has more than one fail record, it's counted more than once.
4. Weekly bucketing uses `WEEKNUM(DrivingDate)` (Sunday-start). The KPI report uses Friday week-ending weeks, so boundary days can land in a different week.
5. Reference values from SAS's SyteLine OTIF report (2026, %):

   | Week | 29 | 30 | 31 | 32 | 33 | 34 |
   |---|---|---|---|---|---|---|
   | BE | 94 | 91 | 94 | 95 | 89 | 77 |
   | MB | 88 | 52 | 86 | 33 | 91 | 71 |

   The PBIX shows week 31 as BE 94.03% and MB 85.71%, which agrees.

---

## 2. SOP - Cost KPI - UAT.pbix

**Purpose:** SOP Cost KPI "£/FTE": the weekly value of orders completed, divided by the FTE headcount for that week. Built by Rob (SAS) against the UAT database to help with the calculation.

### Data model
| Table | Type | Columns |
|---|---|---|
| `ValueOfOrdersCompleted` | Native SQL (Import) | WeekEnding, OrderValue, WeekNoValueOfOrders |
| `FTEHeadcount` | SharePoint folder → Excel | Source.Name, WeekNo, WeekEndingFriday, FTEHeadcount |

**Relationship:** `ValueOfOrdersCompleted[WeekNoValueOfOrders]` → `FTEHeadcount[WeekNo]` (joined on a **week number**, not a date).

### Source query: `ValueOfOrdersCompleted`
Server `SAS-DEV-DB01`, database `RBMW_UAT`:
```
let
    Source = Sql.Database("SAS-DEV-DB01", "RBMW_UAT", [Query="SELECT
    DATEADD(day,
            6 - DATEPART(weekday, CAST(coitem_mst.Uf_OrderedDate AS date)),
            CAST(coitem_mst.Uf_OrderedDate AS date)
    ) AS WeekEnding,

    ROUND(
        SUM(
            coitem_mst.qty_ordered_conv *
            (coitem_mst.price_conv * (1 - coitem_mst.disc / 100.0))
            / ISNULL(co_mst.exch_rate,1)
        ),
        0
    ) AS OrderValue

FROM dbo.coitem_mst
JOIN dbo.co_mst
    ON co_mst.site_ref = coitem_mst.site_ref
   AND co_mst.co_num = coitem_mst.co_num

WHERE
    coitem_mst.site_ref = 'RBMW'
    AND coitem_mst.stat < 'P'
    AND co_mst.type IN ('B','R')
    AND LEFT(co_mst.co_num,1) <> 'I'
    AND co_mst.end_user_type IN ('2','13','26','28')
    AND coitem_mst.rma_num IS NULL
    AND ISNULL(coitem_mst.Uf_LongDescription,'') NOT LIKE '%CARRIAGE%'

GROUP BY
    DATEADD(day,
            6 - DATEPART(weekday, CAST(coitem_mst.Uf_OrderedDate AS date)),
            CAST(coitem_mst.Uf_OrderedDate AS date)
    )"]),
    #"Sorted Rows" = Table.Sort(Source,{{"WeekEnding", Order.Descending}}),
    #"Added Conditional Column" = Table.AddColumn(#"Sorted Rows", "WeekNoValueOfOrders", each if [WeekEnding] = #datetime(2026, 1, 2, 0, 0, 0) then 1 else if [WeekEnding] = #datetime(2026, 1, 9, 0, 0, 0) then 2 else ... (hard-coded, one branch per Friday) ... else if [WeekEnding] = #datetime(2027, 1, 1, 0, 0, 0) then 53 else null)
in
    #"Added Conditional Column"
```
(The `WeekNoValueOfOrders` column is a hard-coded M if/else chain mapping each 2026 Friday to week 1–53. It returns null for any other year.)

### Source query: `FTEHeadcount`
```
let
    Source = SharePoint.Files("https://sasint.sharepoint.com/sites/SASINTProjects", [ApiVersion = 15]),
    #"Sorted Rows" = Table.Sort(Source,{{"Folder Path", Order.Descending}}),
    #"Filtered Rows" = Table.SelectRows(#"Sorted Rows", each ([Folder Path] = "https://sasint.sharepoint.com/sites/SASINTProjects/United Kingdom/SOP KPIs - FTE/")),
    #"Filtered Hidden Files1" = Table.SelectRows(#"Filtered Rows", each [Attributes]?[Hidden]? <> true),
    #"Invoke Custom Function1" = Table.AddColumn(#"Filtered Hidden Files1", "Transform File (2)", each #"Transform File (2)"([Content])),
    #"Renamed Columns1" = Table.RenameColumns(#"Invoke Custom Function1", {"Name", "Source.Name"}),
    #"Removed Other Columns1" = Table.SelectColumns(#"Renamed Columns1", {"Source.Name", "Transform File (2)"}),
    #"Expanded Table Column1" = Table.ExpandTableColumn(#"Removed Other Columns1", "Transform File (2)", Table.ColumnNames(#"Transform File (2)"(#"Sample File (3)"))),
    #"Changed Type" = Table.TransformColumnTypes(#"Expanded Table Column1",{{"Source.Name", type text}, {"WeekNo", Int64.Type}, {"WeekEndingFriday", type date}, {"FTEHeadcount", type number}})
in
    #"Changed Type"
```
The helper function reads sheet **`FabricStagingSheet`** (promoted headers) from each file in the folder `SASINTProjects/United Kingdom/SOP KPIs - FTE/`. The file is "SOP KPIs - FTE headcount.xlsx", populated manually by Laurence.

### DAX measures
```
FTECalc :=
DIVIDE(
    SUM('ValueOfOrdersCompleted'[OrderValue]),
    SUM('FTEHeadcount'[FTEHeadcount])
)
```

### Report page
One page, "SOP - Cost KPI - UAT", with three tables:
- FTEHeadcount (WeekNo, WeekEndingFriday, FTEHeadcount).
- WeekNo with `FTECalc`.
- ValueOfOrdersCompleted (WeekEnding, OrderValue, WeekNoValueOfOrders), filtered to WeekEnding from 2026-01-01.

The page also has bookmarks, a SAS logo and a screenshot image.

### Observations for the rebuild
1. Week ending uses `DATEADD(day, 6 - DATEPART(weekday, d), d)` with SQL Server's default `DATEFIRST 7`. Sunday–Friday map to that week's Friday, but **Saturday maps back to the previous Friday**, so weeks run Sunday–Saturday labelled by the Friday.
2. The "completed" date used is `coitem_mst.Uf_OrderedDate` (a custom field), as Sarah specified.
3. Filters: lines with `stat < 'P'` (string comparison); order types B/R; excludes order numbers starting with 'I'; end-user types 2/13/26/28; excludes RMA lines and carriage lines. Value is converted to GBP via `co_mst.exch_rate`.
4. Known reconciliation gap (Rob): week 27 2026 (w/e 03/07) shows £770,562 in the SOP KPI report but £783,352 in SyteLine, probably snapshot timing.
5. The week-number join and hard-coded 2026 mapping don't carry over between years. A date-based join on WeekEnding = WeekEndingFriday is safer.
6. 2026 target from the KPI sheet: £33,026 per FTE, Under Breach (higher is better).

---

## 3. Product Eng BE - Quality KPI.pbix

**Purpose:** Numerator for the Product Engineering Bridgend Quality KPI, "% of quality defects vs items output" = BOM Helpdesk tickets ÷ items completed (the denominator comes from SyteLine, not this file). Target 4%, Over Breach.

### Data model
| Table | Type | Columns |
|---|---|---|
| `BOMHelpdeskTickets` | SharePoint list (Import) | Id, Title, AdditionalInfo, Priority, Status, Description, Assignedto0Id, Assignedto0StringId, Attachments, RelatedIssueId, Job/CustomerOrder#, Item#, QtyonOrder, Created, Issue Type, Department, ID 2, Modified, AuthorId, EditorId, GUID, plus SharePoint system columns (ContentTypeId, ServerRedirectedEmbedUri/Url, OData__ColorTag, ComplianceAssetId, OData__FormSourceId_0, OData__UIVersionString, FileSystemObjectType, On Copy (PersoId…) |

No relationships and no DAX measures.

### Source query
```
let
    Source = SharePoint.Tables("https://sasint.sharepoint.com/sites/DesignTeamHelpdesk", [ApiVersion = 15]),
    #"0aed6ee7-f297-4f2f-9ec8-3baf9283a9b9" = Source{[Id="0aed6ee7-f297-4f2f-9ec8-3baf9283a9b9"]}[Items]
in
    #"0aed6ee7-f297-4f2f-9ec8-3baf9283a9b9"
```

### Report page
One page, "Product Eng BE - Quality KPI":
- Card: count of `Id`.
- Table: Created, Id, Item#, Job/CustomerOrder#, Priority, QtyonOrder, Status, Title.

**Page filter:** `Status` NOT IN ('Invalid').

### Observations for the rebuild
1. KPI numerator = count of tickets with Status ≠ 'Invalid', bucketed by `Created` date. Rob's email calls the excluded status "Non-valid" while the PBIX filter uses "Invalid", so confirm the exact value.
2. The BOM Helpdesk moved from a Microsoft Forms version to this SharePoint list. Older history (Forms extract) isn't in this file.
3. The model also contains leftover, unused Power Query parameters/functions from an EHS report: a SharePoint "EHS Strategy FY26.xlsx" / "Incident Register" sheet. They aren't loaded tables and aren't relevant.
4. Denominator (items completed) comes from Sarah's daily SyteLine snapshot: Items Completed = Planning Load (yesterday) + New Items (today) − Planning Load (today), for open customer-order lines whose item BOM status is B/D/E/P, warehouse BE.

---

## 4. Product Eng MB - Quality KPI.pbix

**Purpose:** Numerator for the Product Engineering Maybole Quality KPI ("% of quality defects vs items output"). Target 4%, Over Breach.

### Data model
| Table | Type | Columns |
|---|---|---|
| `issues` | SafetyCulture (iAuditor) connector | issue_id, title, description, creator_id, creator_user_name, created_at, due_at, priority, status, template_id, inspection_id, inspection_name, site_id, site_name, location_name, category_id, category_label, modified_at, completed_at, asset_id, unique_id, occurred_at |
| `issue_assignees` | SafetyCulture (iAuditor) connector | id, issue_id, assignee_id, name, organisation_id, modified_at, type |

**Relationship:** `issue_assignees[issue_id]` → `issues[issue_id]`. No DAX measures.

### Source queries
```
let
    Source = iAuditor.Contents("SAS International"),
    Issues = Source{[Name="Issues"]}[Data],
    issues1 = Issues{[Name="issues"]}[Data]
in
    issues1
```
`issue_assignees` is loaded the same way from `Issues{[Name="issue_assignees"]}`.

### Report page
One page, "Product Eng MB - Quality KPI":
- Card: count of `issue_id` (showed 749 at the time of Rob's screenshot).
- Table: unique_id, title, status, priority, modified_at, site_name, created_at.

**Page filters:** `category_label = 'Product Engineering Issue'`, `site_name = 'Maybole'`, and a filter on `created_at`.

### Observations for the rebuild
1. KPI numerator = count of issues where category_label = 'Product Engineering Issue' and site_name = 'Maybole', bucketed by `created_at`. Status isn't filtered, so open and resolved issues both count.
2. The 749 shown on the card is all-time (or limited only by the created_at filter), not weekly.
3. **Denominator ambiguity.** Rob's 07/09 email says number of new lines set to BOM status C in SyteLine on a given day; his 24/09 email says both sites use complaints ÷ items completed. Needs confirming.
4. Same leftover, unused EHS parameters as the BE file, plus "Energy KPI calc.xlsx" TP BE / TP MB sheets.
5. The existing Fabric SafetyCulture feed only ingests inspections. The `issues` table would need a new ingestion.

---

## Cross-cutting notes
- **Week definitions differ:**
  - OTIF PBIX: `WEEKNUM`, Sunday-start.
  - SOP SQL: Sunday–Saturday labelled by Friday.
  - Sarah's Production Value SQL: `SET DATEFIRST 6`, Saturday–Friday ending Friday.
  - The KPI report: "Date (Fri)", the week-ending Friday.
- **RAG rules in the KPI report (Top 4 KPI workbook key):**
  - G = better than target; A = less than 5% worse; R = worse; TBC = missing submission; Blank = no submission.
  - Under Breach (higher is better): A when actual ≥ 95% of target.
  - Over Breach (lower is better): A when actual ≤ target / 0.95.
  - These rules reproduce all 2,074 historical G/A/R values in the wk42 workbook.
- **Connection strings:** the files point at `RBMW_Live` (OTIF) and `RBMW_UAT` (SOP). Ingestion should use UAT until SAS approve Live.
