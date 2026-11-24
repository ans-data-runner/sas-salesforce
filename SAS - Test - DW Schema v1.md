#SAS - Test - DW Schema v1
Generated using [DbSchema](https://dbschema.com)




### SAS - Test - DW Schema v1
![img](./SAS-Test-DWSchemav1.svg)


## Tables

1. [dbo.kpi_result_silver_enriched_v2](#table%20dbo.kpi\_result\_silver\_enriched\_v2) 
2. [elt.dim_date](#table%20elt.dim\_date) 
3. [elt.fact_kpi_result](#table%20elt.fact\_kpi\_result) 
4. [elt.fact_kpi_result_enriched](#table%20elt.fact\_kpi\_result\_enriched) 
5. [freshservice.fact_it_freshservice_survey](#table%20freshservice.fact\_it\_freshservice\_survey) 
6. [freshservice.fact_it_freshservice_survey_weekly](#table%20freshservice.fact\_it\_freshservice\_survey\_weekly) 
7. [freshservice.fact_it_freshservice_ticket](#table%20freshservice.fact\_it\_freshservice\_ticket) 
8. [freshservice.fact_it_freshservice_ticket_weekly](#table%20freshservice.fact\_it\_freshservice\_ticket\_weekly) 
9. [freshservice.fact_kpi_result](#table%20freshservice.fact\_kpi\_result) 
10. [freshservice.kpi_result_it_freshservice](#table%20freshservice.kpi\_result\_it\_freshservice) 
11. [freshservice_staging.surveys](#table%20freshservice\_staging.surveys) 
12. [freshservice_staging.tickets](#table%20freshservice\_staging.tickets) 
13. [metadata.config_import_batch](#table%20metadata.config\_import\_batch) 
14. [metadata.config_import_error](#table%20metadata.config\_import\_error) 
15. [metadata.curation_execution](#table%20metadata.curation\_execution) 
16. [metadata.curation_procedure](#table%20metadata.curation\_procedure) 
17. [metadata.dataset_config](#table%20metadata.dataset\_config) 
18. [metadata.dataset_execution](#table%20metadata.dataset\_execution) 
19. [metadata.dataset_watermark](#table%20metadata.dataset\_watermark) 
20. [metadata.gold_run](#table%20metadata.gold\_run) 
21. [reporting.dim_date](#table%20reporting.dim\_date) 
22. [reporting.fact_kpi_result](#table%20reporting.fact\_kpi\_result) 
23. [safety_culture.fact_ehs_visual_inspection](#table%20safety\_culture.fact\_ehs\_visual\_inspection) 
24. [safety_culture.fact_ehs_visual_inspection_weekly](#table%20safety\_culture.fact\_ehs\_visual\_inspection\_weekly) 
25. [safety_culture.fact_kpi_result](#table%20safety\_culture.fact\_kpi\_result) 
26. [safety_culture.kpi_result_ehs_safetyculture](#table%20safety\_culture.kpi\_result\_ehs\_safetyculture) 
27. [safety_culture_staging.inspections](#table%20safety\_culture\_staging.inspections) 
28. [safety_culture_staging.issues](#table%20safety\_culture\_staging.issues) 
29. [salesforce.dim_kpi](#table%20salesforce.dim\_kpi) 
30. [salesforce.dim_record_type](#table%20salesforce.dim\_record\_type) 
31. [salesforce.fact_estimating](#table%20salesforce.fact\_estimating) 
32. [salesforce.fact_kpi_result](#table%20salesforce.fact\_kpi\_result) 
33. [salesforce.fact_order_tracking](#table%20salesforce.fact\_order\_tracking) 
34. [salesforce.fact_proposal](#table%20salesforce.fact\_proposal) 
35. [salesforce.fact_proposal_delivery](#table%20salesforce.fact\_proposal\_delivery) 
36. [salesforce.fact_quality_weekly](#table%20salesforce.fact\_quality\_weekly) 
37. [salesforce.kpi_result_design_rnd](#table%20salesforce.kpi\_result\_design\_rnd) 
38. [salesforce_staging.account](#table%20salesforce\_staging.account) 
39. [salesforce_staging.contact](#table%20salesforce\_staging.contact) 
40. [salesforce_staging.estimate](#table%20salesforce\_staging.estimate) 
41. [salesforce_staging.estimate_order_line](#table%20salesforce\_staging.estimate\_order\_line) 
42. [salesforce_staging.estimating_request](#table%20salesforce\_staging.estimating\_request) 
43. [salesforce_staging.opportunity](#table%20salesforce\_staging.opportunity) 
44. [salesforce_staging.order_tracking](#table%20salesforce\_staging.order\_tracking) 
45. [salesforce_staging.project_contact](#table%20salesforce\_staging.project\_contact) 
46. [salesforce_staging.proposal_request](#table%20salesforce\_staging.proposal\_request) 
47. [salesforce_staging.record_type](#table%20salesforce\_staging.record\_type) 
48. [salesforce_staging.sbqq__quote](#table%20salesforce\_staging.sbqq\_\_quote) 
49. [salesforce_staging.sbqq__quote_line](#table%20salesforce\_staging.sbqq\_\_quote\_line) 
50. [salesforce_staging.user](#table%20salesforce\_staging.user) 
51. [sharepoint.fabric_staging](#table%20sharepoint.fabric\_staging) 
52. [sharepoint.incident_register](#table%20sharepoint.incident\_register) 
53. [sharepoint.it_purchasing_2026_staging](#table%20sharepoint.it\_purchasing\_2026\_staging) 
54. [sharepoint.mean_time_between_failure](#table%20sharepoint.mean\_time\_between\_failure) 
55. [sharepoint.proactive_reactive_maintenance](#table%20sharepoint.proactive\_reactive\_maintenance) 
56. [sharepoint.tp_be](#table%20sharepoint.tp\_be) 
57. [sharepoint.tp_mb](#table%20sharepoint.tp\_mb) 
58. [sharepoint_staging.fabric_staging](#table%20sharepoint\_staging.fabric\_staging) 
59. [sharepoint_staging.incident_register](#table%20sharepoint\_staging.incident\_register) 
60. [sharepoint_staging.it_purchasing_2026_staging](#table%20sharepoint\_staging.it\_purchasing\_2026\_staging) 
61. [sharepoint_staging.mean_time_between_failure](#table%20sharepoint\_staging.mean\_time\_between\_failure) 
62. [sharepoint_staging.proactive_reactive_maintenance](#table%20sharepoint\_staging.proactive\_reactive\_maintenance) 
63. [sharepoint_staging.tp_be](#table%20sharepoint\_staging.tp\_be) 
64. [sharepoint_staging.tp_mb](#table%20sharepoint\_staging.tp\_mb) 
65. [staging.curation_procedure_import](#table%20staging.curation\_procedure\_import) 
66. [staging.dataset_config_import](#table%20staging.dataset\_config\_import) 
67. [staging.fact_kpi_result_staging](#table%20staging.fact\_kpi\_result\_staging) 
68. [staging.fact_kpi_result_v3](#table%20staging.fact\_kpi\_result\_v3) 
69. [staging.fact_proposal](#table%20staging.fact\_proposal) 
70. [staging.kpi_kpi_result_v3](#table%20staging.kpi\_kpi\_result\_v3) 
71. [staging.kpi_result_silver](#table%20staging.kpi\_result\_silver) 
72. [syteline.fact_kpi_result](#table%20syteline.fact\_kpi\_result) 
73. [syteline.fact_product_engineering_4_week_value_snapshot](#table%20syteline.fact\_product\_engineering\_4\_week\_value\_snapshot) 
74. [syteline.fact_product_engineering_4_week_value_weekly](#table%20syteline.fact\_product\_engineering\_4\_week\_value\_weekly) 
75. [syteline.fact_product_engineering_items_completed_daily](#table%20syteline.fact\_product\_engineering\_items\_completed\_daily) 
76. [syteline.fact_product_engineering_new_items_snapshot](#table%20syteline.fact\_product\_engineering\_new\_items\_snapshot) 
77. [syteline.fact_product_engineering_planning_load_snapshot](#table%20syteline.fact\_product\_engineering\_planning\_load\_snapshot) 
78. [syteline.fact_product_engineering_productivity_daily](#table%20syteline.fact\_product\_engineering\_productivity\_daily) 
79. [syteline.fact_product_engineering_productivity_weekly](#table%20syteline.fact\_product\_engineering\_productivity\_weekly) 
80. [syteline.kpi_result_product_engineering_cost](#table%20syteline.kpi\_result\_product\_engineering\_cost) 
81. [syteline.kpi_result_product_engineering_productivity](#table%20syteline.kpi\_result\_product\_engineering\_productivity) 
82. [syteline.product_engineering_productivity_capacity](#table%20syteline.product\_engineering\_productivity\_capacity) 
83. [syteline_staging.aptrxp_mst](#table%20syteline\_staging.aptrxp\_mst) 
84. [syteline_staging.artran_mst](#table%20syteline\_staging.artran\_mst) 
85. [syteline_staging.chart_mst](#table%20syteline\_staging.chart\_mst) 
86. [syteline_staging.co_mst](#table%20syteline\_staging.co\_mst) 
87. [syteline_staging.co_ship_mst](#table%20syteline\_staging.co\_ship\_mst) 
88. [syteline_staging.coitem_mst](#table%20syteline\_staging.coitem\_mst) 
89. [syteline_staging.currate_mst](#table%20syteline\_staging.currate\_mst) 
90. [syteline_staging.custaddr_mst](#table%20syteline\_staging.custaddr\_mst) 
91. [syteline_staging.customer_mst](#table%20syteline\_staging.customer\_mst) 
92. [syteline_staging.inv_hdr_mst](#table%20syteline\_staging.inv\_hdr\_mst) 
93. [syteline_staging.inv_item_mst](#table%20syteline\_staging.inv\_item\_mst) 
94. [syteline_staging.item_mst](#table%20syteline\_staging.item\_mst) 
95. [syteline_staging.itemprice_mst](#table%20syteline\_staging.itemprice\_mst) 
96. [syteline_staging.job_mst](#table%20syteline\_staging.job\_mst) 
97. [syteline_staging.jobmatl_mst](#table%20syteline\_staging.jobmatl\_mst) 
98. [syteline_staging.jobroute_mst](#table%20syteline\_staging.jobroute\_mst) 
99. [syteline_staging.jobtran_mst](#table%20syteline\_staging.jobtran\_mst) 
100. [syteline_staging.ledger_mst](#table%20syteline\_staging.ledger\_mst) 
101. [syteline_staging.non_inventory_item_mst](#table%20syteline\_staging.non\_inventory\_item\_mst) 
102. [syteline_staging.po_mst](#table%20syteline\_staging.po\_mst) 
103. [syteline_staging.poitem_mst](#table%20syteline\_staging.poitem\_mst) 
104. [syteline_staging.sas_otif_mst](#table%20syteline\_staging.sas\_otif\_mst) 
105. [syteline_staging.sas_otif_sum_mst](#table%20syteline\_staging.sas\_otif\_sum\_mst) 
106. [syteline_staging.vendor_mst](#table%20syteline\_staging.vendor\_mst) 

## Views

1. [metadata.vw_active_dataset_config](#view%20metadata.vw\_active\_dataset\_config) 
2. [metadata.vw_curation_execution_history](#view%20metadata.vw\_curation\_execution\_history) 
3. [metadata.vw_current_run_status](#view%20metadata.vw\_current\_run\_status) 
4. [metadata.vw_dataset_execution_history](#view%20metadata.vw\_dataset\_execution\_history) 
5. [metadata.vw_gold_run_history](#view%20metadata.vw\_gold\_run\_history) 
6. [metadata.vw_recent_failures](#view%20metadata.vw\_recent\_failures) 


### Table salesforce_staging.account 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | master\_record\_id| varchar(8000)  |
| &#128270; | name| varchar(8000)  |
| &#128270; | type| varchar(8000)  |
| &#128270; | record\_type\_id| varchar(8000)  |
| &#128270; | parent\_id| varchar(8000)  |
| &#128270; | billing\_street| varchar(8000)  |
| &#128270; | billing\_city| varchar(8000)  |
| &#128270; | billing\_state| varchar(8000)  |
| &#128270; | billing\_postal\_code| varchar(8000)  |
| &#128270; | billing\_country| varchar(8000)  |
| &#128270; | billing\_state\_code| varchar(8000)  |
| &#128270; | billing\_country\_code| varchar(8000)  |
| &#128270; | billing\_latitude| decimal(38,18)  |
| &#128270; | billing\_longitude| decimal(38,18)  |
| &#128270; | billing\_geocode\_accuracy| varchar(8000)  |
| &#128270; | shipping\_street| varchar(8000)  |
| &#128270; | shipping\_city| varchar(8000)  |
| &#128270; | shipping\_state| varchar(8000)  |
| &#128270; | shipping\_postal\_code| varchar(8000)  |
| &#128270; | shipping\_country| varchar(8000)  |
| &#128270; | shipping\_state\_code| varchar(8000)  |
| &#128270; | shipping\_country\_code| varchar(8000)  |
| &#128270; | shipping\_latitude| decimal(38,18)  |
| &#128270; | shipping\_longitude| decimal(38,18)  |
| &#128270; | shipping\_geocode\_accuracy| varchar(8000)  |
| &#128270; | phone| varchar(8000)  |
| &#128270; | fax| varchar(8000)  |
| &#128270; | account\_number| varchar(8000)  |
| &#128270; | website| varchar(8000)  |
| &#128270; | photo\_url| varchar(8000)  |
| &#128270; | sic| varchar(8000)  |
| &#128270; | industry| varchar(8000)  |
| &#128270; | annual\_revenue| decimal(38,18)  |
| &#128270; | number\_of\_employees| int  |
| &#128270; | ownership| varchar(8000)  |
| &#128270; | ticker\_symbol| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | rating| varchar(8000)  |
| &#128270; | site| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | owner\_id| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | is\_customer\_portal| bit  |
| &#128270; | jigsaw| varchar(8000)  |
| &#128270; | jigsaw\_company\_id| varchar(8000)  |
| &#128270; | account\_source| varchar(8000)  |
| &#128270; | sic\_desc| varchar(8000)  |
| &#128270; | operating\_hours\_id| varchar(8000)  |
| &#128270; | infor\_number| varchar(8000)  |
| &#128270; | account\_description| varchar(8000)  |
| &#128270; | account\_status| varchar(8000)  |
| &#128270; | account\_type| varchar(8000)  |
| &#128270; | accounts\_comments| varchar(8000)  |
| &#128270; | additional\_information| varchar(8000)  |
| &#128270; | alternative\_name| varchar(8000)  |
| &#128270; | associated\_account| varchar(8000)  |
| &#128270; | company\_background| varchar(8000)  |
| &#128270; | company\_sub\_type| varchar(8000)  |
| &#128270; | company\_type| varchar(8000)  |
| &#128270; | credit\_rating\_indicator| varchar(8000)  |
| &#128270; | credit\_rating| varchar(8000)  |
| &#128270; | fast\_track\_customer| varchar(8000)  |
| &#128270; | customer| varchar(8000)  |
| &#128270; | date\_of\_turnover\_estimate| datetime2(26)  |
| &#128270; | divisional\_owner| varchar(8000)  |
| &#128270; | estimated\_turnover| decimal(38,18)  |
| &#128270; | infor\_reference| varchar(8000)  |
| &#128270; | insured\_credit\_limit| decimal(38,18)  |
| &#128270; | lead\_id| varchar(8000)  |
| &#128270; | market\_ranking| varchar(8000)  |
| &#128270; | merged\_status| varchar(8000)  |
| &#128270; | notes| varchar(8000)  |
| &#128270; | on\_order\_balance| decimal(38,18)  |
| &#128270; | parent\_account| varchar(8000)  |
| &#128270; | posted\_balance| varchar(8000)  |
| &#128270; | primary\_currency| varchar(8000)  |
| &#128270; | primary\_infor\_reference| varchar(8000)  |
| &#128270; | primary\_infor\_site| varchar(8000)  |
| &#128270; | record\_type\_name| varchar(8000)  |
| &#128270; | relationship\_ranking| varchar(8000)  |
| &#128270; | sas\_credit\_limit| decimal(38,18)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | sales\_region| varchar(8000)  |
| &#128270; | scheme\_lead\_link| varchar(8000)  |
| &#128270; | scheme\_notes| varchar(8000)  |
| &#128270; | secondary\_owner| varchar(8000)  |
| &#128270; | secondary\_source| varchar(8000)  |
| &#128270; | image| varchar(8000)  |
| &#128270; | interior\_image| varchar(8000)  |
| &#128270; | tenant\_list| varchar(8000)  |
| &#128270; | tenant\_list\_date| datetime2(26)  |
| &#128270; | target\_company| bit  |
| &#128270; | sbqq\_\_asset\_quantities\_combined| bit  |
| &#128270; | customer\_account\_type| varchar(8000)  |
| &#128270; | customer\_credit\_limit| decimal(38,18)  |
| &#128270; | customer\_on\_order\_balance| decimal(38,18)  |
| &#128270; | customer\_posted\_balance| decimal(38,18)  |
| &#128270; | conversion\_rate| decimal(38,18)  |
| &#128270; | number\_of\_related\_company| decimal(38,18)  |
| &#128270; | number\_of\_securing\_manufacturer| decimal(38,18)  |
| &#128270; | strike\_rate| decimal(38,18)  |
| &#128270; | total\_order\_value| decimal(38,18)  |
| &#128270; | total\_transfer\_value| decimal(38,18)  |
| &#128270; | annual\_financial\_report\_date| datetime2(26)  |
| &#128270; | annual\_financial\_report\_percentage| decimal(38,18)  |
| &#128270; | annual\_financial\_report| bit  |
| &#128270; | fabric\_products\_introduced\_percentage| decimal(38,18)  |
| &#128270; | fabric\_products\_introduced| decimal(38,18)  |
| &#128270; | sbqq\_\_co\_termed\_contracts\_combined| bit  |
| &#128270; | competitors\_worked\_with\_knowledge| bit  |
| &#128270; | competitors\_worked\_with\_percentage| decimal(38,18)  |
| &#128270; | corporate\_structure\_date| datetime2(26)  |
| &#128270; | corporate\_structure\_percentage| decimal(38,18)  |
| &#128270; | corporate\_structure| bit  |
| &#128270; | escalation\_contacts\_percentage| decimal(38,18)  |
| &#128270; | escalation\_contacts| decimal(38,18)  |
| &#128270; | hospitality\_major\_percentage| decimal(38,18)  |
| &#128270; | hospitality\_major| decimal(38,18)  |
| &#128270; | hospitality\_minor\_percentage| decimal(38,18)  |
| &#128270; | hospitality\_minor| decimal(38,18)  |
| &#128270; | key\_contacts\_percentage| decimal(38,18)  |
| &#128270; | key\_contacts| decimal(38,18)  |
| &#128270; | sbqq\_\_contract\_co\_termination| varchar(8000)  |
| &#128270; | preffered\_relationships\_percentage| decimal(38,18)  |
| &#128270; | sbqq\_\_default\_opportunity| varchar(8000)  |
| &#128270; | proposals\_issued\_percentage| decimal(38,18)  |
| &#128270; | proposals\_issued| decimal(38,18)  |
| &#128270; | sas\_core\_products\_introduced\_percentage| decimal(38,18)  |
| &#128270; | sas\_core\_products\_introduced| bit  |
| &#128270; | sas\_margin\_profitability\_percentage| decimal(38,18)  |
| &#128270; | sectors\_worked\_in\_percentage| decimal(38,18)  |
| &#128270; | sectors\_worked\_in| bit  |
| &#128270; | special\_projects\_introduced\_percentage| decimal(38,18)  |
| &#128270; | special\_projects\_introduced| decimal(38,18)  |
| &#128270; | specification\_issued\_percentage| decimal(38,18)  |
| &#128270; | specification\_issued| decimal(38,18)  |
| &#128270; | strike\_rate\_checked\_percentage| decimal(38,18)  |
| &#128270; | supply\_chain\_agreements\_percentage| decimal(38,18)  |
| &#128270; | supply\_chain\_agreements| bit  |
| &#128270; | sustainability\_introduction\_percentage| decimal(38,18)  |
| &#128270; | sustainability\_introduction| decimal(38,18)  |
| &#128270; | tsfk\_rating| varchar(8000)  |
| &#128270; | knowledge\_total\_percentage| decimal(38,18)  |
| &#128270; | tsfk\_percentage| decimal(38,18)  |
| &#128270; | total\_financial\_percentage| decimal(38,18)  |
| &#128270; | total\_social\_percentage| decimal(38,18)  |
| &#128270; | total\_technical\_percentage| decimal(38,18)  |
| &#128270; | margin\_profitability\_formula| decimal(38,18)  |
| &#128270; | preferred\_relationships| decimal(38,18)  |
| &#128270; | sbqq\_\_ignore\_parent\_contracted\_prices| bit  |
| &#128270; | sbqq\_\_preserve\_bundle| bit  |
| &#128270; | sbqq\_\_price\_hold\_end| datetime2(26)  |
| &#128270; | sbqq\_\_renewal\_model| varchar(8000)  |
| &#128270; | sbqq\_\_renewal\_pricing\_method| varchar(8000)  |
| &#128270; | sbqq\_\_tax\_exempt| varchar(8000)  |
| &#128270; | sbqq\_\_co\_termination\_event| varchar(8000)  |
| &#128270; | competitor\_specified\_company| varchar(8000)  |
| &#128270; | disable\_quoting| bit  |
| &#128270; | estimated\_metal\_turnover\_uk| decimal(38,18)  |
| &#128270; | last\_account\_management\_date| datetime2(26)  |
| &#128270; | estimated\_fibre\_turnover\_uk| decimal(38,18)  |
| &#128270; | email\_domain| varchar(8000)  |
| &#128270; | estimated\_fabric\_turnover\_uk| decimal(38,18)  |
| &#128270; | call\_frequency| decimal(38,18)  |
| &#128270; | estimated\_metal\_turnover\_non\_uk| decimal(38,18)  |
| &#128270; | estimated\_fibre\_turnover\_non\_uk| decimal(38,18)  |
| &#128270; | estimated\_fabric\_turnover\_non\_uk| decimal(38,18)  |
| &#128270; | open\_account\_management\_tasks| decimal(38,18)  |
| &#128270; | estimated\_other\_turnover\_uk| decimal(38,18)  |
| &#128270; | estimated\_other\_turnover\_non\_uk| decimal(38,18)  |
| &#128270; | estimated\_turnover\_uk| decimal(38,18)  |
| &#128270; | estimated\_turnover\_non\_uk| decimal(38,18)  |
| &#128270; | competitor\_estimated\_turnover| decimal(38,18)  |
| &#128270; | estimated\_metal\_turnover| decimal(38,18)  |
| &#128270; | estimated\_fibre\_turnover| decimal(38,18)  |
| &#128270; | estimated\_fabric\_turnover| decimal(38,18)  |
| &#128270; | estimated\_other\_turnover| decimal(38,18)  |
| &#128270; | other\_tunover\_notes| varchar(8000)  |
| &#128270; | competitor\_strategy\_identified| varchar(8000)  |
| &#128270; | competitor\_sales\_approach| varchar(8000)  |
| &#128270; | primary\_route\_to\_market| varchar(8000)  |
| &#128270; | marketing\_presence| varchar(8000)  |
| &#128270; | sustainability\_profile| varchar(8000)  |
| &#128270; | strengths| varchar(8000)  |
| &#128270; | weaknesses| varchar(8000)  |
| &#128270; | gm\_approval\_required| bit  |
| &#128270; | average\_price\_point\_uk\_sqm| decimal(38,18)  |
| &#128270; | sas\_strategy| varchar(8000)  |
| &#128270; | sales\_team\_size| decimal(38,18)  |
| &#128270; | capacity| varchar(8000)  |
| &#128270; | number\_of\_manufacturing\_locations| decimal(38,18)  |
| &#128270; | no| decimal(38,18)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON master\_record\_id|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON record\_type\_id|
| &#128270;  | ClusteredIndex | ON parent\_id|
| &#128270;  | ClusteredIndex | ON billing\_street|
| &#128270;  | ClusteredIndex | ON billing\_city|
| &#128270;  | ClusteredIndex | ON billing\_state|
| &#128270;  | ClusteredIndex | ON billing\_postal\_code|
| &#128270;  | ClusteredIndex | ON billing\_country|
| &#128270;  | ClusteredIndex | ON billing\_state\_code|
| &#128270;  | ClusteredIndex | ON billing\_country\_code|
| &#128270;  | ClusteredIndex | ON billing\_latitude|
| &#128270;  | ClusteredIndex | ON billing\_longitude|
| &#128270;  | ClusteredIndex | ON billing\_geocode\_accuracy|
| &#128270;  | ClusteredIndex | ON shipping\_street|
| &#128270;  | ClusteredIndex | ON shipping\_city|
| &#128270;  | ClusteredIndex | ON shipping\_state|
| &#128270;  | ClusteredIndex | ON shipping\_postal\_code|
| &#128270;  | ClusteredIndex | ON shipping\_country|
| &#128270;  | ClusteredIndex | ON shipping\_state\_code|
| &#128270;  | ClusteredIndex | ON shipping\_country\_code|
| &#128270;  | ClusteredIndex | ON shipping\_latitude|
| &#128270;  | ClusteredIndex | ON shipping\_longitude|
| &#128270;  | ClusteredIndex | ON shipping\_geocode\_accuracy|
| &#128270;  | ClusteredIndex | ON phone|
| &#128270;  | ClusteredIndex | ON fax|
| &#128270;  | ClusteredIndex | ON account\_number|
| &#128270;  | ClusteredIndex | ON website|
| &#128270;  | ClusteredIndex | ON photo\_url|
| &#128270;  | ClusteredIndex | ON sic|
| &#128270;  | ClusteredIndex | ON industry|
| &#128270;  | ClusteredIndex | ON annual\_revenue|
| &#128270;  | ClusteredIndex | ON number\_of\_employees|
| &#128270;  | ClusteredIndex | ON ownership|
| &#128270;  | ClusteredIndex | ON ticker\_symbol|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON rating|
| &#128270;  | ClusteredIndex | ON site|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON owner\_id|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON is\_customer\_portal|
| &#128270;  | ClusteredIndex | ON jigsaw|
| &#128270;  | ClusteredIndex | ON jigsaw\_company\_id|
| &#128270;  | ClusteredIndex | ON account\_source|
| &#128270;  | ClusteredIndex | ON sic\_desc|
| &#128270;  | ClusteredIndex | ON operating\_hours\_id|
| &#128270;  | ClusteredIndex | ON infor\_number|
| &#128270;  | ClusteredIndex | ON account\_description|
| &#128270;  | ClusteredIndex | ON account\_status|
| &#128270;  | ClusteredIndex | ON account\_type|
| &#128270;  | ClusteredIndex | ON accounts\_comments|
| &#128270;  | ClusteredIndex | ON additional\_information|
| &#128270;  | ClusteredIndex | ON alternative\_name|
| &#128270;  | ClusteredIndex | ON associated\_account|
| &#128270;  | ClusteredIndex | ON company\_background|
| &#128270;  | ClusteredIndex | ON company\_sub\_type|
| &#128270;  | ClusteredIndex | ON company\_type|
| &#128270;  | ClusteredIndex | ON credit\_rating\_indicator|
| &#128270;  | ClusteredIndex | ON credit\_rating|
| &#128270;  | ClusteredIndex | ON fast\_track\_customer|
| &#128270;  | ClusteredIndex | ON customer|
| &#128270;  | ClusteredIndex | ON date\_of\_turnover\_estimate|
| &#128270;  | ClusteredIndex | ON divisional\_owner|
| &#128270;  | ClusteredIndex | ON estimated\_turnover|
| &#128270;  | ClusteredIndex | ON infor\_reference|
| &#128270;  | ClusteredIndex | ON insured\_credit\_limit|
| &#128270;  | ClusteredIndex | ON lead\_id|
| &#128270;  | ClusteredIndex | ON market\_ranking|
| &#128270;  | ClusteredIndex | ON merged\_status|
| &#128270;  | ClusteredIndex | ON notes|
| &#128270;  | ClusteredIndex | ON on\_order\_balance|
| &#128270;  | ClusteredIndex | ON parent\_account|
| &#128270;  | ClusteredIndex | ON posted\_balance|
| &#128270;  | ClusteredIndex | ON primary\_currency|
| &#128270;  | ClusteredIndex | ON primary\_infor\_reference|
| &#128270;  | ClusteredIndex | ON primary\_infor\_site|
| &#128270;  | ClusteredIndex | ON record\_type\_name|
| &#128270;  | ClusteredIndex | ON relationship\_ranking|
| &#128270;  | ClusteredIndex | ON sas\_credit\_limit|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON sales\_region|
| &#128270;  | ClusteredIndex | ON scheme\_lead\_link|
| &#128270;  | ClusteredIndex | ON scheme\_notes|
| &#128270;  | ClusteredIndex | ON secondary\_owner|
| &#128270;  | ClusteredIndex | ON secondary\_source|
| &#128270;  | ClusteredIndex | ON image|
| &#128270;  | ClusteredIndex | ON interior\_image|
| &#128270;  | ClusteredIndex | ON tenant\_list|
| &#128270;  | ClusteredIndex | ON tenant\_list\_date|
| &#128270;  | ClusteredIndex | ON target\_company|
| &#128270;  | ClusteredIndex | ON sbqq\_\_asset\_quantities\_combined|
| &#128270;  | ClusteredIndex | ON customer\_account\_type|
| &#128270;  | ClusteredIndex | ON customer\_credit\_limit|
| &#128270;  | ClusteredIndex | ON customer\_on\_order\_balance|
| &#128270;  | ClusteredIndex | ON customer\_posted\_balance|
| &#128270;  | ClusteredIndex | ON conversion\_rate|
| &#128270;  | ClusteredIndex | ON number\_of\_related\_company|
| &#128270;  | ClusteredIndex | ON number\_of\_securing\_manufacturer|
| &#128270;  | ClusteredIndex | ON strike\_rate|
| &#128270;  | ClusteredIndex | ON total\_order\_value|
| &#128270;  | ClusteredIndex | ON total\_transfer\_value|
| &#128270;  | ClusteredIndex | ON annual\_financial\_report\_date|
| &#128270;  | ClusteredIndex | ON annual\_financial\_report\_percentage|
| &#128270;  | ClusteredIndex | ON annual\_financial\_report|
| &#128270;  | ClusteredIndex | ON fabric\_products\_introduced\_percentage|
| &#128270;  | ClusteredIndex | ON fabric\_products\_introduced|
| &#128270;  | ClusteredIndex | ON sbqq\_\_co\_termed\_contracts\_combined|
| &#128270;  | ClusteredIndex | ON competitors\_worked\_with\_knowledge|
| &#128270;  | ClusteredIndex | ON competitors\_worked\_with\_percentage|
| &#128270;  | ClusteredIndex | ON corporate\_structure\_date|
| &#128270;  | ClusteredIndex | ON corporate\_structure\_percentage|
| &#128270;  | ClusteredIndex | ON corporate\_structure|
| &#128270;  | ClusteredIndex | ON escalation\_contacts\_percentage|
| &#128270;  | ClusteredIndex | ON escalation\_contacts|
| &#128270;  | ClusteredIndex | ON hospitality\_major\_percentage|
| &#128270;  | ClusteredIndex | ON hospitality\_major|
| &#128270;  | ClusteredIndex | ON hospitality\_minor\_percentage|
| &#128270;  | ClusteredIndex | ON hospitality\_minor|
| &#128270;  | ClusteredIndex | ON key\_contacts\_percentage|
| &#128270;  | ClusteredIndex | ON key\_contacts|
| &#128270;  | ClusteredIndex | ON sbqq\_\_contract\_co\_termination|
| &#128270;  | ClusteredIndex | ON preffered\_relationships\_percentage|
| &#128270;  | ClusteredIndex | ON sbqq\_\_default\_opportunity|
| &#128270;  | ClusteredIndex | ON proposals\_issued\_percentage|
| &#128270;  | ClusteredIndex | ON proposals\_issued|
| &#128270;  | ClusteredIndex | ON sas\_core\_products\_introduced\_percentage|
| &#128270;  | ClusteredIndex | ON sas\_core\_products\_introduced|
| &#128270;  | ClusteredIndex | ON sas\_margin\_profitability\_percentage|
| &#128270;  | ClusteredIndex | ON sectors\_worked\_in\_percentage|
| &#128270;  | ClusteredIndex | ON sectors\_worked\_in|
| &#128270;  | ClusteredIndex | ON special\_projects\_introduced\_percentage|
| &#128270;  | ClusteredIndex | ON special\_projects\_introduced|
| &#128270;  | ClusteredIndex | ON specification\_issued\_percentage|
| &#128270;  | ClusteredIndex | ON specification\_issued|
| &#128270;  | ClusteredIndex | ON strike\_rate\_checked\_percentage|
| &#128270;  | ClusteredIndex | ON supply\_chain\_agreements\_percentage|
| &#128270;  | ClusteredIndex | ON supply\_chain\_agreements|
| &#128270;  | ClusteredIndex | ON sustainability\_introduction\_percentage|
| &#128270;  | ClusteredIndex | ON sustainability\_introduction|
| &#128270;  | ClusteredIndex | ON tsfk\_rating|
| &#128270;  | ClusteredIndex | ON knowledge\_total\_percentage|
| &#128270;  | ClusteredIndex | ON tsfk\_percentage|
| &#128270;  | ClusteredIndex | ON total\_financial\_percentage|
| &#128270;  | ClusteredIndex | ON total\_social\_percentage|
| &#128270;  | ClusteredIndex | ON total\_technical\_percentage|
| &#128270;  | ClusteredIndex | ON margin\_profitability\_formula|
| &#128270;  | ClusteredIndex | ON preferred\_relationships|
| &#128270;  | ClusteredIndex | ON sbqq\_\_ignore\_parent\_contracted\_prices|
| &#128270;  | ClusteredIndex | ON sbqq\_\_preserve\_bundle|
| &#128270;  | ClusteredIndex | ON sbqq\_\_price\_hold\_end|
| &#128270;  | ClusteredIndex | ON sbqq\_\_renewal\_model|
| &#128270;  | ClusteredIndex | ON sbqq\_\_renewal\_pricing\_method|
| &#128270;  | ClusteredIndex | ON sbqq\_\_tax\_exempt|
| &#128270;  | ClusteredIndex | ON sbqq\_\_co\_termination\_event|
| &#128270;  | ClusteredIndex | ON competitor\_specified\_company|
| &#128270;  | ClusteredIndex | ON disable\_quoting|
| &#128270;  | ClusteredIndex | ON estimated\_metal\_turnover\_uk|
| &#128270;  | ClusteredIndex | ON last\_account\_management\_date|
| &#128270;  | ClusteredIndex | ON estimated\_fibre\_turnover\_uk|
| &#128270;  | ClusteredIndex | ON email\_domain|
| &#128270;  | ClusteredIndex | ON estimated\_fabric\_turnover\_uk|
| &#128270;  | ClusteredIndex | ON call\_frequency|
| &#128270;  | ClusteredIndex | ON estimated\_metal\_turnover\_non\_uk|
| &#128270;  | ClusteredIndex | ON estimated\_fibre\_turnover\_non\_uk|
| &#128270;  | ClusteredIndex | ON estimated\_fabric\_turnover\_non\_uk|
| &#128270;  | ClusteredIndex | ON open\_account\_management\_tasks|
| &#128270;  | ClusteredIndex | ON estimated\_other\_turnover\_uk|
| &#128270;  | ClusteredIndex | ON estimated\_other\_turnover\_non\_uk|
| &#128270;  | ClusteredIndex | ON estimated\_turnover\_uk|
| &#128270;  | ClusteredIndex | ON estimated\_turnover\_non\_uk|
| &#128270;  | ClusteredIndex | ON competitor\_estimated\_turnover|
| &#128270;  | ClusteredIndex | ON estimated\_metal\_turnover|
| &#128270;  | ClusteredIndex | ON estimated\_fibre\_turnover|
| &#128270;  | ClusteredIndex | ON estimated\_fabric\_turnover|
| &#128270;  | ClusteredIndex | ON estimated\_other\_turnover|
| &#128270;  | ClusteredIndex | ON other\_tunover\_notes|
| &#128270;  | ClusteredIndex | ON competitor\_strategy\_identified|
| &#128270;  | ClusteredIndex | ON competitor\_sales\_approach|
| &#128270;  | ClusteredIndex | ON primary\_route\_to\_market|
| &#128270;  | ClusteredIndex | ON marketing\_presence|
| &#128270;  | ClusteredIndex | ON sustainability\_profile|
| &#128270;  | ClusteredIndex | ON strengths|
| &#128270;  | ClusteredIndex | ON weaknesses|
| &#128270;  | ClusteredIndex | ON gm\_approval\_required|
| &#128270;  | ClusteredIndex | ON average\_price\_point\_uk\_sqm|
| &#128270;  | ClusteredIndex | ON sas\_strategy|
| &#128270;  | ClusteredIndex | ON sales\_team\_size|
| &#128270;  | ClusteredIndex | ON capacity|
| &#128270;  | ClusteredIndex | ON number\_of\_manufacturing\_locations|
| &#128270;  | ClusteredIndex | ON no|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.aptrxp_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | vend\_num| varchar(8000)  |
| &#128270; | voucher| int  |
| &#128270; | active| int  |
| &#128270; | type| varchar(8000)  |
| &#128270; | dist\_date| datetime2(26)  |
| &#128270; | po\_num| varchar(8000)  |
| &#128270; | inv\_num| varchar(8000)  |
| &#128270; | inv\_date| datetime2(26)  |
| &#128270; | inv\_amt| decimal(23,8)  |
| &#128270; | non\_disc\_amt| decimal(23,8)  |
| &#128270; | due\_days| int  |
| &#128270; | due\_date| datetime2(26)  |
| &#128270; | disc\_days| int  |
| &#128270; | disc\_date| datetime2(26)  |
| &#128270; | disc\_pct| decimal(6,3)  |
| &#128270; | disc\_amt| decimal(23,8)  |
| &#128270; | ap\_acct| varchar(8000)  |
| &#128270; | amt\_paid| decimal(23,8)  |
| &#128270; | amt\_disc| decimal(23,8)  |
| &#128270; | hold\_flag| int  |
| &#128270; | check\_num| int  |
| &#128270; | vouch\_seq| int  |
| &#128270; | exch\_rate| decimal(12,7)  |
| &#128270; | purch\_amt| decimal(23,8)  |
| &#128270; | misc\_charges| decimal(23,8)  |
| &#128270; | sales\_tax| decimal(23,8)  |
| &#128270; | sales\_tax\_2| decimal(23,8)  |
| &#128270; | freight| decimal(23,8)  |
| &#128270; | prox\_day| int  |
| &#128270; | duty\_amt| decimal(23,8)  |
| &#128270; | brokerage\_amt| decimal(23,8)  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON vend\_num|
| &#128270;  | ClusteredIndex | ON voucher|
| &#128270;  | ClusteredIndex | ON active|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON dist\_date|
| &#128270;  | ClusteredIndex | ON po\_num|
| &#128270;  | ClusteredIndex | ON inv\_num|
| &#128270;  | ClusteredIndex | ON inv\_date|
| &#128270;  | ClusteredIndex | ON inv\_amt|
| &#128270;  | ClusteredIndex | ON non\_disc\_amt|
| &#128270;  | ClusteredIndex | ON due\_days|
| &#128270;  | ClusteredIndex | ON due\_date|
| &#128270;  | ClusteredIndex | ON disc\_days|
| &#128270;  | ClusteredIndex | ON disc\_date|
| &#128270;  | ClusteredIndex | ON disc\_pct|
| &#128270;  | ClusteredIndex | ON disc\_amt|
| &#128270;  | ClusteredIndex | ON ap\_acct|
| &#128270;  | ClusteredIndex | ON amt\_paid|
| &#128270;  | ClusteredIndex | ON amt\_disc|
| &#128270;  | ClusteredIndex | ON hold\_flag|
| &#128270;  | ClusteredIndex | ON check\_num|
| &#128270;  | ClusteredIndex | ON vouch\_seq|
| &#128270;  | ClusteredIndex | ON exch\_rate|
| &#128270;  | ClusteredIndex | ON purch\_amt|
| &#128270;  | ClusteredIndex | ON misc\_charges|
| &#128270;  | ClusteredIndex | ON sales\_tax|
| &#128270;  | ClusteredIndex | ON sales\_tax\_2|
| &#128270;  | ClusteredIndex | ON freight|
| &#128270;  | ClusteredIndex | ON prox\_day|
| &#128270;  | ClusteredIndex | ON duty\_amt|
| &#128270;  | ClusteredIndex | ON brokerage\_amt|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.artran_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | inv\_num| varchar(8000)  |
| &#128270; | inv\_seq| int  |
| &#128270; | check\_seq| int  |
| &#128270; | type| varchar(8000)  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | inv\_date| datetime2(26)  |
| &#128270; | due\_date| datetime2(26)  |
| &#128270; | acct| varchar(8000)  |
| &#128270; | amount| decimal(23,8)  |
| &#128270; | disc\_amt| decimal(23,8)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | disc\_date| datetime2(26)  |
| &#128270; | issue\_date| datetime2(26)  |
| &#128270; | exch\_rate| decimal(12,7)  |
| &#128270; | misc\_charges| decimal(23,8)  |
| &#128270; | sales\_tax| decimal(23,8)  |
| &#128270; | freight| decimal(23,8)  |
| &#128270; | sales\_tax\_2| decimal(23,8)  |
| &#128270; | bank\_code| varchar(8000)  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | corp\_cust| varchar(8000)  |
| &#128270; | post\_from\_co| int  |
| &#128270; | active| int  |
| &#128270; | acct\_unit1| varchar(8000)  |
| &#128270; | acct\_unit2| varchar(8000)  |
| &#128270; | acct\_unit3| varchar(8000)  |
| &#128270; | acct\_unit4| varchar(8000)  |
| &#128270; | fixed\_rate| int  |
| &#128270; | rma| int  |
| &#128270; | pay\_type| varchar(8000)  |
| &#128270; | ref| varchar(8000)  |
| &#128270; | do\_num| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | apply\_to\_inv\_num| varchar(8000)  |
| &#128270; | approval\_status| varchar(8000)  |
| &#128270; | is\_invoice| int  |
| &#128270; | apply\_to\_inv\_num\_category| int  |
| &#128270; | shipment\_id| decimal(19,0)  |
| &#128270; | builder\_inv\_orig\_site| varchar(8000)  |
| &#128270; | builder\_inv\_num| varchar(8000)  |
| &#128270; | post\_site| varchar(8000)  |
| &#128270; | recpt\_date| datetime2(26)  |
| &#128270; | inv\_batch\_id| decimal(19,0)  |
| &#128270; | cancellation| int  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | au\_payment\_ref\_num| varchar(8000)  |
| &#128270; | orig\_cust\_num| varchar(8000)  |
| &#128270; | orig\_site| varchar(8000)  |
| &#128270; | th\_payment\_number| varchar(8000)  |
| &#128270; | tax\_disc| decimal(23,8)  |
| &#128270; | pl\_delivery\_type| varchar(8000)  |
| &#128270; | pl\_document\_list| varchar(8000)  |
| &#128270; | pl\_manual\_vat\_invoice| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON inv\_num|
| &#128270;  | ClusteredIndex | ON inv\_seq|
| &#128270;  | ClusteredIndex | ON check\_seq|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON inv\_date|
| &#128270;  | ClusteredIndex | ON due\_date|
| &#128270;  | ClusteredIndex | ON acct|
| &#128270;  | ClusteredIndex | ON amount|
| &#128270;  | ClusteredIndex | ON disc\_amt|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON disc\_date|
| &#128270;  | ClusteredIndex | ON issue\_date|
| &#128270;  | ClusteredIndex | ON exch\_rate|
| &#128270;  | ClusteredIndex | ON misc\_charges|
| &#128270;  | ClusteredIndex | ON sales\_tax|
| &#128270;  | ClusteredIndex | ON freight|
| &#128270;  | ClusteredIndex | ON sales\_tax\_2|
| &#128270;  | ClusteredIndex | ON bank\_code|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON corp\_cust|
| &#128270;  | ClusteredIndex | ON post\_from\_co|
| &#128270;  | ClusteredIndex | ON active|
| &#128270;  | ClusteredIndex | ON acct\_unit1|
| &#128270;  | ClusteredIndex | ON acct\_unit2|
| &#128270;  | ClusteredIndex | ON acct\_unit3|
| &#128270;  | ClusteredIndex | ON acct\_unit4|
| &#128270;  | ClusteredIndex | ON fixed\_rate|
| &#128270;  | ClusteredIndex | ON rma|
| &#128270;  | ClusteredIndex | ON pay\_type|
| &#128270;  | ClusteredIndex | ON ref|
| &#128270;  | ClusteredIndex | ON do\_num|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON apply\_to\_inv\_num|
| &#128270;  | ClusteredIndex | ON approval\_status|
| &#128270;  | ClusteredIndex | ON is\_invoice|
| &#128270;  | ClusteredIndex | ON apply\_to\_inv\_num\_category|
| &#128270;  | ClusteredIndex | ON shipment\_id|
| &#128270;  | ClusteredIndex | ON builder\_inv\_orig\_site|
| &#128270;  | ClusteredIndex | ON builder\_inv\_num|
| &#128270;  | ClusteredIndex | ON post\_site|
| &#128270;  | ClusteredIndex | ON recpt\_date|
| &#128270;  | ClusteredIndex | ON inv\_batch\_id|
| &#128270;  | ClusteredIndex | ON cancellation|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON au\_payment\_ref\_num|
| &#128270;  | ClusteredIndex | ON orig\_cust\_num|
| &#128270;  | ClusteredIndex | ON orig\_site|
| &#128270;  | ClusteredIndex | ON th\_payment\_number|
| &#128270;  | ClusteredIndex | ON tax\_disc|
| &#128270;  | ClusteredIndex | ON pl\_delivery\_type|
| &#128270;  | ClusteredIndex | ON pl\_document\_list|
| &#128270;  | ClusteredIndex | ON pl\_manual\_vat\_invoice|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.chart_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | acct| varchar(8000)  |
| &#128270; | type| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | eff\_date| datetime2(26)  |
| &#128270; | obs\_date| datetime2(26)  |
| &#128270; | reports\_to\_acct| varchar(8000)  |
| &#128270; | trans\_method| varchar(8000)  |
| &#128270; | use\_buy\_rate| int  |
| &#128270; | access\_unit1| varchar(8000)  |
| &#128270; | access\_unit2| varchar(8000)  |
| &#128270; | access\_unit3| varchar(8000)  |
| &#128270; | access\_unit4| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | acct\_class| varchar(8000)  |
| &#128270; | is\_control| int  |
| &#128270; | mx\_applies\_to\_ietu| int  |
| &#128270; | mx\_ietu\_deduction\_pct| decimal(5,2)  |
| &#128270; | mx\_diot\_trans\_type| varchar(8000)  |
| &#128270; | mx\_ietu\_class| varchar(8000)  |
| &#128270; | ledger\_dim\_name| varchar(8000)  |
| &#128270; | uf\_account\_group| varchar(8000)  |
| &#128270; | uf\_account\_sub\_group| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON acct|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON eff\_date|
| &#128270;  | ClusteredIndex | ON obs\_date|
| &#128270;  | ClusteredIndex | ON reports\_to\_acct|
| &#128270;  | ClusteredIndex | ON trans\_method|
| &#128270;  | ClusteredIndex | ON use\_buy\_rate|
| &#128270;  | ClusteredIndex | ON access\_unit1|
| &#128270;  | ClusteredIndex | ON access\_unit2|
| &#128270;  | ClusteredIndex | ON access\_unit3|
| &#128270;  | ClusteredIndex | ON access\_unit4|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON acct\_class|
| &#128270;  | ClusteredIndex | ON is\_control|
| &#128270;  | ClusteredIndex | ON mx\_applies\_to\_ietu|
| &#128270;  | ClusteredIndex | ON mx\_ietu\_deduction\_pct|
| &#128270;  | ClusteredIndex | ON mx\_diot\_trans\_type|
| &#128270;  | ClusteredIndex | ON mx\_ietu\_class|
| &#128270;  | ClusteredIndex | ON ledger\_dim\_name|
| &#128270;  | ClusteredIndex | ON uf\_account\_group|
| &#128270;  | ClusteredIndex | ON uf\_account\_sub\_group|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.co_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | type| varchar(8000)  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | est\_num| varchar(8000)  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | cust\_seq| int  |
| &#128270; | contact| varchar(8000)  |
| &#128270; | phone| varchar(8000)  |
| &#128270; | cust\_po| varchar(8000)  |
| &#128270; | order\_date| datetime2(26)  |
| &#128270; | taken\_by| varchar(8000)  |
| &#128270; | terms\_code| varchar(8000)  |
| &#128270; | ship\_code| varchar(8000)  |
| &#128270; | price| decimal(23,8)  |
| &#128270; | weight| decimal(9,2)  |
| &#128270; | qty\_packages| int  |
| &#128270; | freight| decimal(23,8)  |
| &#128270; | misc\_charges| decimal(23,8)  |
| &#128270; | prepaid\_amt| decimal(23,8)  |
| &#128270; | sales\_tax| decimal(23,8)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | cost| decimal(23,8)  |
| &#128270; | close\_date| datetime2(26)  |
| &#128270; | freight\_t| decimal(23,8)  |
| &#128270; | m\_charges\_t| decimal(23,8)  |
| &#128270; | prepaid\_t| decimal(23,8)  |
| &#128270; | sales\_tax\_t| decimal(23,8)  |
| &#128270; | slsman| varchar(8000)  |
| &#128270; | eff\_date| datetime2(26)  |
| &#128270; | exp\_date| datetime2(26)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | sales\_tax\_2| decimal(23,8)  |
| &#128270; | sales\_tax\_t2| decimal(23,8)  |
| &#128270; | edi\_order| int  |
| &#128270; | trans\_nat| varchar(8000)  |
| &#128270; | process\_ind| varchar(8000)  |
| &#128270; | delterm| varchar(8000)  |
| &#128270; | use\_exch\_rate| int  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | frt\_tax\_code1| varchar(8000)  |
| &#128270; | frt\_tax\_code2| varchar(8000)  |
| &#128270; | msc\_tax\_code1| varchar(8000)  |
| &#128270; | msc\_tax\_code2| varchar(8000)  |
| &#128270; | discount\_type| varchar(8000)  |
| &#128270; | disc\_amount| decimal(23,8)  |
| &#128270; | disc| decimal(11,8)  |
| &#128270; | pricecode| varchar(8000)  |
| &#128270; | ship\_partial| int  |
| &#128270; | ship\_early| int  |
| &#128270; | matl\_cost\_t| decimal(23,8)  |
| &#128270; | lbr\_cost\_t| decimal(23,8)  |
| &#128270; | fovhd\_cost\_t| decimal(23,8)  |
| &#128270; | vovhd\_cost\_t| decimal(23,8)  |
| &#128270; | out\_cost\_t| decimal(23,8)  |
| &#128270; | end\_user\_type| varchar(8000)  |
| &#128270; | exch\_rate| decimal(12,7)  |
| &#128270; | fixed\_rate| int  |
| &#128270; | orig\_site| varchar(8000)  |
| &#128270; | lcr\_num| varchar(8000)  |
| &#128270; | edi\_type| varchar(8000)  |
| &#128270; | invoiced| int  |
| &#128270; | credit\_hold| int  |
| &#128270; | credit\_hold\_date| datetime2(26)  |
| &#128270; | credit\_hold\_reason| varchar(8000)  |
| &#128270; | credit\_hold\_user| varchar(8000)  |
| &#128270; | sync\_reqd| int  |
| &#128270; | projected\_date| datetime2(26)  |
| &#128270; | order\_source| varchar(8000)  |
| &#128270; | convert\_type| varchar(8000)  |
| &#128270; | aps\_pull\_up| int  |
| &#128270; | consolidate| int  |
| &#128270; | inv\_freq| varchar(8000)  |
| &#128270; | summarize| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | einvoice| int  |
| &#128270; | charfld1| varchar(8000)  |
| &#128270; | charfld2| varchar(8000)  |
| &#128270; | charfld3| varchar(8000)  |
| &#128270; | datefld| datetime2(26)  |
| &#128270; | decifld1| decimal(10,2)  |
| &#128270; | decifld2| decimal(10,2)  |
| &#128270; | decifld3| decimal(10,2)  |
| &#128270; | logifld| int  |
| &#128270; | ack\_stat| varchar(8000)  |
| &#128270; | config\_id| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | include\_tax\_in\_price| int  |
| &#128270; | trans\_nat\_2| varchar(8000)  |
| &#128270; | apply\_to\_inv\_num| varchar(8000)  |
| &#128270; | export\_type| varchar(8000)  |
| &#128270; | external\_confirmation\_ref| varchar(8000)  |
| &#128270; | is\_external| int  |
| &#128270; | prospect\_id| varchar(8000)  |
| &#128270; | opp\_id| varchar(8000)  |
| &#128270; | lead\_id| varchar(8000)  |
| &#128270; | days\_shipped\_before\_due\_date\_tolerance| int  |
| &#128270; | days\_shipped\_after\_due\_date\_tolerance| int  |
| &#128270; | shipped\_over\_ordered\_qty\_tolerance| decimal(7,4)  |
| &#128270; | shipped\_under\_ordered\_qty\_tolerance| decimal(7,4)  |
| &#128270; | consignment| int  |
| &#128270; | priority| int  |
| &#128270; | demanding\_site| varchar(8000)  |
| &#128270; | demanding\_site\_po\_num| varchar(8000)  |
| &#128270; | shipment\_approval\_required| int  |
| &#128270; | portal\_order| int  |
| &#128270; | ship\_hold| int  |
| &#128270; | payment\_method| varchar(8000)  |
| &#128270; | ship\_method| varchar(8000)  |
| &#128270; | surcharge| decimal(23,8)  |
| &#128270; | surcharge\_t| decimal(23,8)  |
| &#128270; | config\_doc\_id| varchar(8000)  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | external\_whse\_line\_changed| int  |
| &#128270; | order\_bal| decimal(23,8)  |
| &#128270; | withholding\_tax\_amount| decimal(23,8)  |
| &#128270; | withholding\_tax\_amount\_t| decimal(23,8)  |
| &#128270; | external\_freight| decimal(23,8)  |
| &#128270; | carrier\_service\_type| varchar(8000)  |
| &#128270; | bill\_to\_name| varchar(8000)  |
| &#128270; | bill\_to\_city| varchar(8000)  |
| &#128270; | bill\_to\_state| varchar(8000)  |
| &#128270; | bill\_to\_zip| varchar(8000)  |
| &#128270; | bill\_to\_county| varchar(8000)  |
| &#128270; | bill\_to\_country| varchar(8000)  |
| &#128270; | bill\_to\_addr\_1| varchar(8000)  |
| &#128270; | bill\_to\_addr\_2| varchar(8000)  |
| &#128270; | bill\_to\_addr\_3| varchar(8000)  |
| &#128270; | bill\_to\_addr\_4| varchar(8000)  |
| &#128270; | ship\_to\_name| varchar(8000)  |
| &#128270; | ship\_to\_city| varchar(8000)  |
| &#128270; | ship\_to\_state| varchar(8000)  |
| &#128270; | ship\_to\_zip| varchar(8000)  |
| &#128270; | ship\_to\_county| varchar(8000)  |
| &#128270; | ship\_to\_country| varchar(8000)  |
| &#128270; | ship\_to\_addr\_1| varchar(8000)  |
| &#128270; | ship\_to\_addr\_2| varchar(8000)  |
| &#128270; | ship\_to\_addr\_3| varchar(8000)  |
| &#128270; | ship\_to\_addr\_4| varchar(8000)  |
| &#128270; | pl\_document\_type| varchar(8000)  |
| &#128270; | uf\_ack\_date| datetime2(26)  |
| &#128270; | uf\_addendum| varchar(8000)  |
| &#128270; | uf\_admin| varchar(8000)  |
| &#128270; | uf\_approxval| int  |
| &#128270; | uf\_bfi\_cont\_num| varchar(8000)  |
| &#128270; | uf\_bfi\_co\_num| varchar(8000)  |
| &#128270; | uf\_bfi\_cust\_num| varchar(8000)  |
| &#128270; | uf\_budget| int  |
| &#128270; | uf\_budget\_duplicate| int  |
| &#128270; | uf\_cash| int  |
| &#128270; | uf\_category| varchar(8000)  |
| &#128270; | uf\_complexity| varchar(8000)  |
| &#128270; | uf\_concern\_no| varchar(8000)  |
| &#128270; | uf\_consolfrom| varchar(8000)  |
| &#128270; | uf\_cont\_num| varchar(8000)  |
| &#128270; | uf\_co\_revision| int  |
| &#128270; | uf\_co\_stat| varchar(8000)  |
| &#128270; | uf\_credit\_release| int  |
| &#128270; | uf\_credit\_released\_by| varchar(8000)  |
| &#128270; | uf\_credit\_release\_no| varchar(8000)  |
| &#128270; | uf\_customer\_acct\_type| varchar(8000)  |
| &#128270; | uf\_date\_rec| datetime2(26)  |
| &#128270; | uf\_dist\_cost| decimal(23,8)  |
| &#128270; | uf\_dist\_val| decimal(23,8)  |
| &#128270; | uf\_division| varchar(8000)  |
| &#128270; | uf\_est\_dist| decimal(23,8)  |
| &#128270; | uf\_est\_dist\_adj| decimal(23,8)  |
| &#128270; | uf\_estimator| varchar(8000)  |
| &#128270; | uf\_est\_in\_date| datetime2(26)  |
| &#128270; | uf\_est\_lbr| decimal(23,8)  |
| &#128270; | uf\_est\_lbr\_adj| decimal(23,8)  |
| &#128270; | uf\_est\_out\_date| datetime2(26)  |
| &#128270; | uf\_est\_transport| int  |
| &#128270; | uf\_est\_val| decimal(23,8)  |
| &#128270; | uf\_est\_val\_adj| decimal(23,8)  |
| &#128270; | uf\_expiry\_date| datetime2(26)  |
| &#128270; | uf\_export| varchar(8000)  |
| &#128270; | uf\_figures| int  |
| &#128270; | uf\_floor\_on\_label| int  |
| &#128270; | uf\_glass\_notification| int  |
| &#128270; | uf\_gm| decimal(11,8)  |
| &#128270; | uf\_gma| decimal(11,8)  |
| &#128270; | uf\_gmm| decimal(11,8)  |
| &#128270; | uf\_hour\_rec| varchar(8000)  |
| &#128270; | uf\_installpc| decimal(11,8)  |
| &#128270; | uf\_invoice\_to| int  |
| &#128270; | uf\_job\_type| varchar(8000)  |
| &#128270; | uf\_labour| decimal(23,8)  |
| &#128270; | uf\_lbr\_cost| decimal(23,8)  |
| &#128270; | uf\_lbr\_date| datetime2(26)  |
| &#128270; | uf\_lbr\_val| decimal(23,8)  |
| &#128270; | uf\_lc\_bank\_ref| varchar(8000)  |
| &#128270; | uf\_location| varchar(8000)  |
| &#128270; | uf\_m2| decimal(15,4)  |
| &#128270; | uf\_magento\_id| varchar(8000)  |
| &#128270; | uf\_material\_group| varchar(8000)  |
| &#128270; | uf\_micross\_no| varchar(8000)  |
| &#128270; | uf\_min\_rec| varchar(8000)  |
| &#128270; | uf\_name| varchar(8000)  |
| &#128270; | uf\_name2| varchar(8000)  |
| &#128270; | uf\_option| int  |
| &#128270; | uf\_orderxrate| decimal(5,0)  |
| &#128270; | uf\_payment\_days| int  |
| &#128270; | uf\_pending\_amt| decimal(19,4)  |
| &#128270; | uf\_pending\_reason| varchar(8000)  |
| &#128270; | uf\_primary| int  |
| &#128270; | uf\_probability| varchar(8000)  |
| &#128270; | uf\_proforma\_type| varchar(8000)  |
| &#128270; | uf\_project| varchar(8000)  |
| &#128270; | uf\_red\_flag| varchar(8000)  |
| &#128270; | uf\_revision| varchar(8000)  |
| &#128270; | uf\_ship\_to\_phone\_3| varchar(8000)  |
| &#128270; | uf\_ship\_to\_prj\_mgr| varchar(8000)  |
| &#128270; | uf\_spa| varchar(8000)  |
| &#128270; | uf\_status| varchar(8000)  |
| &#128270; | uf\_system| varchar(8000)  |
| &#128270; | uf\_taken\_by| varchar(8000)  |
| &#128270; | uf\_tech\_sales| varchar(8000)  |
| &#128270; | uf\_terms\_code| varchar(8000)  |
| &#128270; | uf\_total\_price\_less\_tax| decimal(21,8)  |
| &#128270; | uf\_trn\_cost\_tot| decimal(23,8)  |
| &#128270; | uf\_trn\_price\_tot| decimal(23,8)  |
| &#128270; | uf\_unknown| varchar(8000)  |
| &#128270; | uf\_validate| int  |
| &#128270; | uf\_validate\_by| varchar(8000)  |
| &#128270; | uf\_volume| int  |
| &#128270; | uf\_warehouse| varchar(8000)  |
| &#128270; | uf\_add\_m2| decimal(15,2)  |
| &#128270; | uf\_est\_by| varchar(8000)  |
| &#128270; | uf\_hide\_line\_m2\_details| int  |
| &#128270; | uf\_m2\_tot\_price| decimal(15,2)  |
| &#128270; | uf\_spec| varchar(8000)  |
| &#128270; | uf\_salesforce\_id| varchar(8000)  |
| &#128270; | uf\_mlt\_date| datetime2(26)  |
| &#128270; | uf\_request\_date| datetime2(26)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON est\_num|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON cust\_seq|
| &#128270;  | ClusteredIndex | ON contact|
| &#128270;  | ClusteredIndex | ON phone|
| &#128270;  | ClusteredIndex | ON cust\_po|
| &#128270;  | ClusteredIndex | ON order\_date|
| &#128270;  | ClusteredIndex | ON taken\_by|
| &#128270;  | ClusteredIndex | ON terms\_code|
| &#128270;  | ClusteredIndex | ON ship\_code|
| &#128270;  | ClusteredIndex | ON price|
| &#128270;  | ClusteredIndex | ON weight|
| &#128270;  | ClusteredIndex | ON qty\_packages|
| &#128270;  | ClusteredIndex | ON freight|
| &#128270;  | ClusteredIndex | ON misc\_charges|
| &#128270;  | ClusteredIndex | ON prepaid\_amt|
| &#128270;  | ClusteredIndex | ON sales\_tax|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON cost|
| &#128270;  | ClusteredIndex | ON close\_date|
| &#128270;  | ClusteredIndex | ON freight\_t|
| &#128270;  | ClusteredIndex | ON m\_charges\_t|
| &#128270;  | ClusteredIndex | ON prepaid\_t|
| &#128270;  | ClusteredIndex | ON sales\_tax\_t|
| &#128270;  | ClusteredIndex | ON slsman|
| &#128270;  | ClusteredIndex | ON eff\_date|
| &#128270;  | ClusteredIndex | ON exp\_date|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON sales\_tax\_2|
| &#128270;  | ClusteredIndex | ON sales\_tax\_t2|
| &#128270;  | ClusteredIndex | ON edi\_order|
| &#128270;  | ClusteredIndex | ON trans\_nat|
| &#128270;  | ClusteredIndex | ON process\_ind|
| &#128270;  | ClusteredIndex | ON delterm|
| &#128270;  | ClusteredIndex | ON use\_exch\_rate|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON frt\_tax\_code1|
| &#128270;  | ClusteredIndex | ON frt\_tax\_code2|
| &#128270;  | ClusteredIndex | ON msc\_tax\_code1|
| &#128270;  | ClusteredIndex | ON msc\_tax\_code2|
| &#128270;  | ClusteredIndex | ON discount\_type|
| &#128270;  | ClusteredIndex | ON disc\_amount|
| &#128270;  | ClusteredIndex | ON disc|
| &#128270;  | ClusteredIndex | ON pricecode|
| &#128270;  | ClusteredIndex | ON ship\_partial|
| &#128270;  | ClusteredIndex | ON ship\_early|
| &#128270;  | ClusteredIndex | ON matl\_cost\_t|
| &#128270;  | ClusteredIndex | ON lbr\_cost\_t|
| &#128270;  | ClusteredIndex | ON fovhd\_cost\_t|
| &#128270;  | ClusteredIndex | ON vovhd\_cost\_t|
| &#128270;  | ClusteredIndex | ON out\_cost\_t|
| &#128270;  | ClusteredIndex | ON end\_user\_type|
| &#128270;  | ClusteredIndex | ON exch\_rate|
| &#128270;  | ClusteredIndex | ON fixed\_rate|
| &#128270;  | ClusteredIndex | ON orig\_site|
| &#128270;  | ClusteredIndex | ON lcr\_num|
| &#128270;  | ClusteredIndex | ON edi\_type|
| &#128270;  | ClusteredIndex | ON invoiced|
| &#128270;  | ClusteredIndex | ON credit\_hold|
| &#128270;  | ClusteredIndex | ON credit\_hold\_date|
| &#128270;  | ClusteredIndex | ON credit\_hold\_reason|
| &#128270;  | ClusteredIndex | ON credit\_hold\_user|
| &#128270;  | ClusteredIndex | ON sync\_reqd|
| &#128270;  | ClusteredIndex | ON projected\_date|
| &#128270;  | ClusteredIndex | ON order\_source|
| &#128270;  | ClusteredIndex | ON convert\_type|
| &#128270;  | ClusteredIndex | ON aps\_pull\_up|
| &#128270;  | ClusteredIndex | ON consolidate|
| &#128270;  | ClusteredIndex | ON inv\_freq|
| &#128270;  | ClusteredIndex | ON summarize|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON einvoice|
| &#128270;  | ClusteredIndex | ON charfld1|
| &#128270;  | ClusteredIndex | ON charfld2|
| &#128270;  | ClusteredIndex | ON charfld3|
| &#128270;  | ClusteredIndex | ON datefld|
| &#128270;  | ClusteredIndex | ON decifld1|
| &#128270;  | ClusteredIndex | ON decifld2|
| &#128270;  | ClusteredIndex | ON decifld3|
| &#128270;  | ClusteredIndex | ON logifld|
| &#128270;  | ClusteredIndex | ON ack\_stat|
| &#128270;  | ClusteredIndex | ON config\_id|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON include\_tax\_in\_price|
| &#128270;  | ClusteredIndex | ON trans\_nat\_2|
| &#128270;  | ClusteredIndex | ON apply\_to\_inv\_num|
| &#128270;  | ClusteredIndex | ON export\_type|
| &#128270;  | ClusteredIndex | ON external\_confirmation\_ref|
| &#128270;  | ClusteredIndex | ON is\_external|
| &#128270;  | ClusteredIndex | ON prospect\_id|
| &#128270;  | ClusteredIndex | ON opp\_id|
| &#128270;  | ClusteredIndex | ON lead\_id|
| &#128270;  | ClusteredIndex | ON days\_shipped\_before\_due\_date\_tolerance|
| &#128270;  | ClusteredIndex | ON days\_shipped\_after\_due\_date\_tolerance|
| &#128270;  | ClusteredIndex | ON shipped\_over\_ordered\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON shipped\_under\_ordered\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON consignment|
| &#128270;  | ClusteredIndex | ON priority|
| &#128270;  | ClusteredIndex | ON demanding\_site|
| &#128270;  | ClusteredIndex | ON demanding\_site\_po\_num|
| &#128270;  | ClusteredIndex | ON shipment\_approval\_required|
| &#128270;  | ClusteredIndex | ON portal\_order|
| &#128270;  | ClusteredIndex | ON ship\_hold|
| &#128270;  | ClusteredIndex | ON payment\_method|
| &#128270;  | ClusteredIndex | ON ship\_method|
| &#128270;  | ClusteredIndex | ON surcharge|
| &#128270;  | ClusteredIndex | ON surcharge\_t|
| &#128270;  | ClusteredIndex | ON config\_doc\_id|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON external\_whse\_line\_changed|
| &#128270;  | ClusteredIndex | ON order\_bal|
| &#128270;  | ClusteredIndex | ON withholding\_tax\_amount|
| &#128270;  | ClusteredIndex | ON withholding\_tax\_amount\_t|
| &#128270;  | ClusteredIndex | ON external\_freight|
| &#128270;  | ClusteredIndex | ON carrier\_service\_type|
| &#128270;  | ClusteredIndex | ON bill\_to\_name|
| &#128270;  | ClusteredIndex | ON bill\_to\_city|
| &#128270;  | ClusteredIndex | ON bill\_to\_state|
| &#128270;  | ClusteredIndex | ON bill\_to\_zip|
| &#128270;  | ClusteredIndex | ON bill\_to\_county|
| &#128270;  | ClusteredIndex | ON bill\_to\_country|
| &#128270;  | ClusteredIndex | ON bill\_to\_addr\_1|
| &#128270;  | ClusteredIndex | ON bill\_to\_addr\_2|
| &#128270;  | ClusteredIndex | ON bill\_to\_addr\_3|
| &#128270;  | ClusteredIndex | ON bill\_to\_addr\_4|
| &#128270;  | ClusteredIndex | ON ship\_to\_name|
| &#128270;  | ClusteredIndex | ON ship\_to\_city|
| &#128270;  | ClusteredIndex | ON ship\_to\_state|
| &#128270;  | ClusteredIndex | ON ship\_to\_zip|
| &#128270;  | ClusteredIndex | ON ship\_to\_county|
| &#128270;  | ClusteredIndex | ON ship\_to\_country|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_1|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_2|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_3|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_4|
| &#128270;  | ClusteredIndex | ON pl\_document\_type|
| &#128270;  | ClusteredIndex | ON uf\_ack\_date|
| &#128270;  | ClusteredIndex | ON uf\_addendum|
| &#128270;  | ClusteredIndex | ON uf\_admin|
| &#128270;  | ClusteredIndex | ON uf\_approxval|
| &#128270;  | ClusteredIndex | ON uf\_bfi\_cont\_num|
| &#128270;  | ClusteredIndex | ON uf\_bfi\_co\_num|
| &#128270;  | ClusteredIndex | ON uf\_bfi\_cust\_num|
| &#128270;  | ClusteredIndex | ON uf\_budget|
| &#128270;  | ClusteredIndex | ON uf\_budget\_duplicate|
| &#128270;  | ClusteredIndex | ON uf\_cash|
| &#128270;  | ClusteredIndex | ON uf\_category|
| &#128270;  | ClusteredIndex | ON uf\_complexity|
| &#128270;  | ClusteredIndex | ON uf\_concern\_no|
| &#128270;  | ClusteredIndex | ON uf\_consolfrom|
| &#128270;  | ClusteredIndex | ON uf\_cont\_num|
| &#128270;  | ClusteredIndex | ON uf\_co\_revision|
| &#128270;  | ClusteredIndex | ON uf\_co\_stat|
| &#128270;  | ClusteredIndex | ON uf\_credit\_release|
| &#128270;  | ClusteredIndex | ON uf\_credit\_released\_by|
| &#128270;  | ClusteredIndex | ON uf\_credit\_release\_no|
| &#128270;  | ClusteredIndex | ON uf\_customer\_acct\_type|
| &#128270;  | ClusteredIndex | ON uf\_date\_rec|
| &#128270;  | ClusteredIndex | ON uf\_dist\_cost|
| &#128270;  | ClusteredIndex | ON uf\_dist\_val|
| &#128270;  | ClusteredIndex | ON uf\_division|
| &#128270;  | ClusteredIndex | ON uf\_est\_dist|
| &#128270;  | ClusteredIndex | ON uf\_est\_dist\_adj|
| &#128270;  | ClusteredIndex | ON uf\_estimator|
| &#128270;  | ClusteredIndex | ON uf\_est\_in\_date|
| &#128270;  | ClusteredIndex | ON uf\_est\_lbr|
| &#128270;  | ClusteredIndex | ON uf\_est\_lbr\_adj|
| &#128270;  | ClusteredIndex | ON uf\_est\_out\_date|
| &#128270;  | ClusteredIndex | ON uf\_est\_transport|
| &#128270;  | ClusteredIndex | ON uf\_est\_val|
| &#128270;  | ClusteredIndex | ON uf\_est\_val\_adj|
| &#128270;  | ClusteredIndex | ON uf\_expiry\_date|
| &#128270;  | ClusteredIndex | ON uf\_export|
| &#128270;  | ClusteredIndex | ON uf\_figures|
| &#128270;  | ClusteredIndex | ON uf\_floor\_on\_label|
| &#128270;  | ClusteredIndex | ON uf\_glass\_notification|
| &#128270;  | ClusteredIndex | ON uf\_gm|
| &#128270;  | ClusteredIndex | ON uf\_gma|
| &#128270;  | ClusteredIndex | ON uf\_gmm|
| &#128270;  | ClusteredIndex | ON uf\_hour\_rec|
| &#128270;  | ClusteredIndex | ON uf\_installpc|
| &#128270;  | ClusteredIndex | ON uf\_invoice\_to|
| &#128270;  | ClusteredIndex | ON uf\_job\_type|
| &#128270;  | ClusteredIndex | ON uf\_labour|
| &#128270;  | ClusteredIndex | ON uf\_lbr\_cost|
| &#128270;  | ClusteredIndex | ON uf\_lbr\_date|
| &#128270;  | ClusteredIndex | ON uf\_lbr\_val|
| &#128270;  | ClusteredIndex | ON uf\_lc\_bank\_ref|
| &#128270;  | ClusteredIndex | ON uf\_location|
| &#128270;  | ClusteredIndex | ON uf\_m2|
| &#128270;  | ClusteredIndex | ON uf\_magento\_id|
| &#128270;  | ClusteredIndex | ON uf\_material\_group|
| &#128270;  | ClusteredIndex | ON uf\_micross\_no|
| &#128270;  | ClusteredIndex | ON uf\_min\_rec|
| &#128270;  | ClusteredIndex | ON uf\_name|
| &#128270;  | ClusteredIndex | ON uf\_name2|
| &#128270;  | ClusteredIndex | ON uf\_option|
| &#128270;  | ClusteredIndex | ON uf\_orderxrate|
| &#128270;  | ClusteredIndex | ON uf\_payment\_days|
| &#128270;  | ClusteredIndex | ON uf\_pending\_amt|
| &#128270;  | ClusteredIndex | ON uf\_pending\_reason|
| &#128270;  | ClusteredIndex | ON uf\_primary|
| &#128270;  | ClusteredIndex | ON uf\_probability|
| &#128270;  | ClusteredIndex | ON uf\_proforma\_type|
| &#128270;  | ClusteredIndex | ON uf\_project|
| &#128270;  | ClusteredIndex | ON uf\_red\_flag|
| &#128270;  | ClusteredIndex | ON uf\_revision|
| &#128270;  | ClusteredIndex | ON uf\_ship\_to\_phone\_3|
| &#128270;  | ClusteredIndex | ON uf\_ship\_to\_prj\_mgr|
| &#128270;  | ClusteredIndex | ON uf\_spa|
| &#128270;  | ClusteredIndex | ON uf\_status|
| &#128270;  | ClusteredIndex | ON uf\_system|
| &#128270;  | ClusteredIndex | ON uf\_taken\_by|
| &#128270;  | ClusteredIndex | ON uf\_tech\_sales|
| &#128270;  | ClusteredIndex | ON uf\_terms\_code|
| &#128270;  | ClusteredIndex | ON uf\_total\_price\_less\_tax|
| &#128270;  | ClusteredIndex | ON uf\_trn\_cost\_tot|
| &#128270;  | ClusteredIndex | ON uf\_trn\_price\_tot|
| &#128270;  | ClusteredIndex | ON uf\_unknown|
| &#128270;  | ClusteredIndex | ON uf\_validate|
| &#128270;  | ClusteredIndex | ON uf\_validate\_by|
| &#128270;  | ClusteredIndex | ON uf\_volume|
| &#128270;  | ClusteredIndex | ON uf\_warehouse|
| &#128270;  | ClusteredIndex | ON uf\_add\_m2|
| &#128270;  | ClusteredIndex | ON uf\_est\_by|
| &#128270;  | ClusteredIndex | ON uf\_hide\_line\_m2\_details|
| &#128270;  | ClusteredIndex | ON uf\_m2\_tot\_price|
| &#128270;  | ClusteredIndex | ON uf\_spec|
| &#128270;  | ClusteredIndex | ON uf\_salesforce\_id|
| &#128270;  | ClusteredIndex | ON uf\_mlt\_date|
| &#128270;  | ClusteredIndex | ON uf\_request\_date|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.co_ship_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | co\_line| int  |
| &#128270; | co\_release| int  |
| &#128270; | date\_seq| int  |
| &#128270; | qty\_invoiced| decimal(19,8)  |
| &#128270; | ship\_date| datetime2(26)  |
| &#128270; | qty\_shipped| decimal(19,8)  |
| &#128270; | qty\_returned| decimal(19,8)  |
| &#128270; | cost| decimal(20,8)  |
| &#128270; | price| decimal(20,8)  |
| &#128270; | unit\_weight| decimal(11,3)  |
| &#128270; | by\_cons| int  |
| &#128270; | matl\_cost| decimal(20,8)  |
| &#128270; | lbr\_cost| decimal(20,8)  |
| &#128270; | fovhd\_cost| decimal(20,8)  |
| &#128270; | vovhd\_cost| decimal(20,8)  |
| &#128270; | out\_cost| decimal(20,8)  |
| &#128270; | shipper\_num| varchar(8000)  |
| &#128270; | do\_num| varchar(8000)  |
| &#128270; | do\_line| int  |
| &#128270; | do\_seq| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | pack\_num| int  |
| &#128270; | orig\_inv\_num| varchar(8000)  |
| &#128270; | reason\_text| varchar(8000)  |
| &#128270; | shipment\_id| decimal(19,0)  |
| &#128270; | external\_shipment\_doc\_id| varchar(8000)  |
| &#128270; | shipment\_line| int  |
| &#128270; | shipment\_seq| int  |
| &#128270; | inv\_num| varchar(8000)  |
| &#128270; | pro\_forma\_inv\_num| varchar(8000)  |
| &#128270; | orig\_pro\_forma\_inv\_num| varchar(8000)  |
| &#128270; | uf\_credit\_release\_no| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON co\_line|
| &#128270;  | ClusteredIndex | ON co\_release|
| &#128270;  | ClusteredIndex | ON date\_seq|
| &#128270;  | ClusteredIndex | ON qty\_invoiced|
| &#128270;  | ClusteredIndex | ON ship\_date|
| &#128270;  | ClusteredIndex | ON qty\_shipped|
| &#128270;  | ClusteredIndex | ON qty\_returned|
| &#128270;  | ClusteredIndex | ON cost|
| &#128270;  | ClusteredIndex | ON price|
| &#128270;  | ClusteredIndex | ON unit\_weight|
| &#128270;  | ClusteredIndex | ON by\_cons|
| &#128270;  | ClusteredIndex | ON matl\_cost|
| &#128270;  | ClusteredIndex | ON lbr\_cost|
| &#128270;  | ClusteredIndex | ON fovhd\_cost|
| &#128270;  | ClusteredIndex | ON vovhd\_cost|
| &#128270;  | ClusteredIndex | ON out\_cost|
| &#128270;  | ClusteredIndex | ON shipper\_num|
| &#128270;  | ClusteredIndex | ON do\_num|
| &#128270;  | ClusteredIndex | ON do\_line|
| &#128270;  | ClusteredIndex | ON do\_seq|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON pack\_num|
| &#128270;  | ClusteredIndex | ON orig\_inv\_num|
| &#128270;  | ClusteredIndex | ON reason\_text|
| &#128270;  | ClusteredIndex | ON shipment\_id|
| &#128270;  | ClusteredIndex | ON external\_shipment\_doc\_id|
| &#128270;  | ClusteredIndex | ON shipment\_line|
| &#128270;  | ClusteredIndex | ON shipment\_seq|
| &#128270;  | ClusteredIndex | ON inv\_num|
| &#128270;  | ClusteredIndex | ON pro\_forma\_inv\_num|
| &#128270;  | ClusteredIndex | ON orig\_pro\_forma\_inv\_num|
| &#128270;  | ClusteredIndex | ON uf\_credit\_release\_no|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.coitem_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | co\_line| int  |
| &#128270; | co\_release| int  |
| &#128270; | item| varchar(8000)  |
| &#128270; | qty\_ordered| decimal(19,8)  |
| &#128270; | qty\_ready| decimal(19,8)  |
| &#128270; | qty\_shipped| decimal(19,8)  |
| &#128270; | qty\_packed| decimal(19,8)  |
| &#128270; | disc| decimal(11,8)  |
| &#128270; | cost| decimal(20,8)  |
| &#128270; | price| decimal(20,8)  |
| &#128270; | ref\_type| varchar(8000)  |
| &#128270; | ref\_num| varchar(8000)  |
| &#128270; | ref\_line\_suf| int  |
| &#128270; | ref\_release| int  |
| &#128270; | due\_date| datetime2(26)  |
| &#128270; | ship\_date| datetime2(26)  |
| &#128270; | reprice| int  |
| &#128270; | cust\_item| varchar(8000)  |
| &#128270; | qty\_invoiced| decimal(19,8)  |
| &#128270; | qty\_returned| decimal(19,8)  |
| &#128270; | cgs\_total| decimal(23,8)  |
| &#128270; | feat\_str| varchar(8000)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | cust\_seq| int  |
| &#128270; | prg\_bill\_tot| decimal(23,8)  |
| &#128270; | prg\_bill\_app| decimal(23,8)  |
| &#128270; | release\_date| datetime2(26)  |
| &#128270; | promise\_date| datetime2(26)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | wks\_basis| varchar(8000)  |
| &#128270; | wks\_value| decimal(23,8)  |
| &#128270; | comm\_code| varchar(8000)  |
| &#128270; | trans\_nat| varchar(8000)  |
| &#128270; | process\_ind| varchar(8000)  |
| &#128270; | delterm| varchar(8000)  |
| &#128270; | unit\_weight| decimal(11,3)  |
| &#128270; | origin| varchar(8000)  |
| &#128270; | cons\_num| int  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | export\_value| decimal(23,8)  |
| &#128270; | ec\_code| varchar(8000)  |
| &#128270; | transport| varchar(8000)  |
| &#128270; | pick\_date| datetime2(26)  |
| &#128270; | pricecode| varchar(8000)  |
| &#128270; | u\_m| varchar(8000)  |
| &#128270; | qty\_ordered\_conv| decimal(19,8)  |
| &#128270; | price\_conv| decimal(20,8)  |
| &#128270; | co\_cust\_num| varchar(8000)  |
| &#128270; | packed| int  |
| &#128270; | bol| int  |
| &#128270; | qty\_rsvd| decimal(19,8)  |
| &#128270; | matl\_cost| decimal(20,8)  |
| &#128270; | lbr\_cost| decimal(20,8)  |
| &#128270; | fovhd\_cost| decimal(20,8)  |
| &#128270; | vovhd\_cost| decimal(20,8)  |
| &#128270; | out\_cost| decimal(20,8)  |
| &#128270; | cgs\_total\_matl| decimal(23,8)  |
| &#128270; | cgs\_total\_lbr| decimal(23,8)  |
| &#128270; | cgs\_total\_fovhd| decimal(23,8)  |
| &#128270; | cgs\_total\_vovhd| decimal(23,8)  |
| &#128270; | cgs\_total\_out| decimal(23,8)  |
| &#128270; | cost\_conv| decimal(20,8)  |
| &#128270; | matl\_cost\_conv| decimal(20,8)  |
| &#128270; | lbr\_cost\_conv| decimal(20,8)  |
| &#128270; | fovhd\_cost\_conv| decimal(20,8)  |
| &#128270; | vovhd\_cost\_conv| decimal(20,8)  |
| &#128270; | out\_cost\_conv| decimal(20,8)  |
| &#128270; | ship\_site| varchar(8000)  |
| &#128270; | sync\_reqd| int  |
| &#128270; | co\_orig\_site| varchar(8000)  |
| &#128270; | cust\_po| varchar(8000)  |
| &#128270; | rma\_num| varchar(8000)  |
| &#128270; | rma\_line| int  |
| &#128270; | projected\_date| datetime2(26)  |
| &#128270; | consolidate| int  |
| &#128270; | inv\_freq| varchar(8000)  |
| &#128270; | summarize| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | config\_id| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | rcpt\_rqmt| varchar(8000)  |
| &#128270; | trans\_nat\_2| varchar(8000)  |
| &#128270; | suppl\_qty\_conv\_factor| float(53)  |
| &#128270; | print\_kit\_components| int  |
| &#128270; | due\_date\_day| datetime2(26)  |
| &#128270; | external\_reservation\_ref| varchar(8000)  |
| &#128270; | non\_inv\_acct| varchar(8000)  |
| &#128270; | non\_inv\_acct\_unit1| varchar(8000)  |
| &#128270; | non\_inv\_acct\_unit2| varchar(8000)  |
| &#128270; | non\_inv\_acct\_unit3| varchar(8000)  |
| &#128270; | non\_inv\_acct\_unit4| varchar(8000)  |
| &#128270; | days\_shipped\_before\_due\_date\_tolerance| int  |
| &#128270; | days\_shipped\_after\_due\_date\_tolerance| int  |
| &#128270; | shipped\_over\_ordered\_qty\_tolerance| decimal(7,4)  |
| &#128270; | shipped\_under\_ordered\_qty\_tolerance| decimal(7,4)  |
| &#128270; | priority| int  |
| &#128270; | invoice\_hold| int  |
| &#128270; | manufacturer\_id| varchar(8000)  |
| &#128270; | manufacturer\_item| varchar(8000)  |
| &#128270; | qty\_picked| decimal(19,8)  |
| &#128270; | fs\_inc\_num| varchar(8000)  |
| &#128270; | promotion\_code| varchar(8000)  |
| &#128270; | external\_shipment\_line\_id| varchar(8000)  |
| &#128270; | last\_external\_shipment\_doc\_id| varchar(8000)  |
| &#128270; | last\_process\_shipment\_doc\_id| varchar(8000)  |
| &#128270; | allow\_on\_pick\_list| int  |
| &#128270; | external\_shipment\_status| varchar(8000)  |
| &#128270; | exclude\_from\_copy\_to\_co| int  |
| &#128270; | ship\_to\_name| varchar(8000)  |
| &#128270; | ship\_to\_city| varchar(8000)  |
| &#128270; | ship\_to\_state| varchar(8000)  |
| &#128270; | ship\_to\_zip| varchar(8000)  |
| &#128270; | ship\_to\_county| varchar(8000)  |
| &#128270; | ship\_to\_country| varchar(8000)  |
| &#128270; | ship\_to\_addr\_1| varchar(8000)  |
| &#128270; | ship\_to\_addr\_2| varchar(8000)  |
| &#128270; | ship\_to\_addr\_3| varchar(8000)  |
| &#128270; | ship\_to\_addr\_4| varchar(8000)  |
| &#128270; | pl\_override\_item\_description| int  |
| &#128270; | pl\_alternate\_item\_description| varchar(8000)  |
| &#128270; | uf\_amend\_route| varchar(8000)  |
| &#128270; | uf\_appc| decimal(18,8)  |
| &#128270; | uf\_bepc| decimal(18,8)  |
| &#128270; | uf\_bfi\_price| decimal(18,8)  |
| &#128270; | uf\_bom\_unit\_price| decimal(18,8)  |
| &#128270; | uf\_comp\_matl| decimal(20,8)  |
| &#128270; | uf\_comp\_run| decimal(20,8)  |
| &#128270; | uf\_comp\_setup| decimal(20,8)  |
| &#128270; | uf\_config\_status| varchar(8000)  |
| &#128270; | uf\_config\_staus| varchar(8000)  |
| &#128270; | uf\_co\_stat| varchar(8000)  |
| &#128270; | uf\_created| datetime2(26)  |
| &#128270; | uf\_cur\_lbr\_cost| decimal(20,8)  |
| &#128270; | uf\_cur\_matl\_cost| decimal(20,8)  |
| &#128270; | uf\_cur\_out\_cost| decimal(20,8)  |
| &#128270; | uf\_curr\_trn\_price| decimal(20,8)  |
| &#128270; | uf\_cust\_del\_date| datetime2(26)  |
| &#128270; | uf\_cust\_req| int  |
| &#128270; | uf\_distribution| int  |
| &#128270; | uf\_division| varchar(8000)  |
| &#128270; | uf\_floor\_zone| varchar(8000)  |
| &#128270; | uf\_floor\_zone\_description| varchar(8000)  |
| &#128270; | uf\_long\_description| varchar(8000)  |
| &#128270; | uf\_m2| decimal(15,4)  |
| &#128270; | uf\_m2\_tot| decimal(15,2)  |
| &#128270; | uf\_m2\_tot\_price| decimal(15,2)  |
| &#128270; | uf\_margin| decimal(11,8)  |
| &#128270; | uf\_mbpc| decimal(18,8)  |
| &#128270; | uf\_old\_ref\_lin\_suf| int  |
| &#128270; | uf\_old\_ref\_num| varchar(8000)  |
| &#128270; | uf\_old\_ref\_release| int  |
| &#128270; | uf\_old\_ref\_type| varchar(8000)  |
| &#128270; | uf\_one\_piece\_route| int  |
| &#128270; | uf\_ordered\_date| datetime2(26)  |
| &#128270; | uf\_orig\_ack\_del\_date| datetime2(26)  |
| &#128270; | uf\_release| int  |
| &#128270; | uf\_release\_date| datetime2(26)  |
| &#128270; | uf\_same\_day| int  |
| &#128270; | uf\_sas\_cost| decimal(18,8)  |
| &#128270; | uf\_sequence| int  |
| &#128270; | uf\_ship\_location| varchar(8000)  |
| &#128270; | uf\_standard| varchar(8000)  |
| &#128270; | uf\_trn\_cost| decimal(20,8)  |
| &#128270; | uf\_trn\_price| decimal(20,8)  |
| &#128270; | uf\_acoustic| varchar(8000)  |
| &#128270; | uf\_additional\_description| varchar(8000)  |
| &#128270; | uf\_angle| varchar(8000)  |
| &#128270; | uf\_aperture\_offset| varchar(8000)  |
| &#128270; | uf\_aperture\_size| varchar(8000)  |
| &#128270; | uf\_aperture\_type| varchar(8000)  |
| &#128270; | uf\_architrave| varchar(8000)  |
| &#128270; | uf\_birdsmouth\_detail| varchar(8000)  |
| &#128270; | uf\_cat\_ref| varchar(8000)  |
| &#128270; | uf\_co\_line\_config\_description| varchar(8000)  |
| &#128270; | uf\_depth| int  |
| &#128270; | uf\_diameter\_offset| varchar(8000)  |
| &#128270; | uf\_diameter\_size| varchar(8000)  |
| &#128270; | uf\_door\_cat| varchar(8000)  |
| &#128270; | uf\_door\_leaf\_type| varchar(8000)  |
| &#128270; | uf\_door\_type| varchar(8000)  |
| &#128270; | uf\_dr\_frm\_config| varchar(8000)  |
| &#128270; | uf\_edge\_config| varchar(8000)  |
| &#128270; | uf\_edgeor\_grid\_size| varchar(8000)  |
| &#128270; | uf\_frame\_finish| varchar(8000)  |
| &#128270; | uf\_frame\_type| varchar(8000)  |
| &#128270; | uf\_galv| int  |
| &#128270; | uf\_gasket| varchar(8000)  |
| &#128270; | uf\_gauge| varchar(8000)  |
| &#128270; | uf\_glaz\_pckt| varchar(8000)  |
| &#128270; | uf\_handing| varchar(8000)  |
| &#128270; | uf\_hinges| varchar(8000)  |
| &#128270; | uf\_insulation\_type| varchar(8000)  |
| &#128270; | uf\_ironmongery| varchar(8000)  |
| &#128270; | uf\_issue\_no| varchar(8000)  |
| &#128270; | uf\_length| varchar(8000)  |
| &#128270; | uf\_linear\_m\_price| decimal(15,2)  |
| &#128270; | uf\_lipping| int  |
| &#128270; | uf\_location| varchar(8000)  |
| &#128270; | uf\_manufacturer| varchar(8000)  |
| &#128270; | uf\_material\_type| varchar(8000)  |
| &#128270; | uf\_module| varchar(8000)  |
| &#128270; | uf\_module\_length| varchar(8000)  |
| &#128270; | uf\_module\_width| varchar(8000)  |
| &#128270; | uf\_nominal\_border| varchar(8000)  |
| &#128270; | uf\_non\_fire\_rated| varchar(8000)  |
| &#128270; | uf\_over\_panel\_h| varchar(8000)  |
| &#128270; | uf\_paint| varchar(8000)  |
| &#128270; | uf\_partion\_system\_type| varchar(8000)  |
| &#128270; | uf\_partit\_glaze| varchar(8000)  |
| &#128270; | uf\_partition| varchar(8000)  |
| &#128270; | uf\_partition\_type| varchar(8000)  |
| &#128270; | uf\_perf| varchar(8000)  |
| &#128270; | uf\_periphery| varchar(8000)  |
| &#128270; | uf\_product\_type1| varchar(8000)  |
| &#128270; | uf\_profile\_type| varchar(8000)  |
| &#128270; | uf\_site| varchar(8000)  |
| &#128270; | uf\_slave\_leaf\_w| varchar(8000)  |
| &#128270; | uf\_snap\_infill| varchar(8000)  |
| &#128270; | uf\_strike\_plate| varchar(8000)  |
| &#128270; | uf\_sustainability| varchar(8000)  |
| &#128270; | uf\_swing\_type| varchar(8000)  |
| &#128270; | uf\_sys| varchar(8000)  |
| &#128270; | uf\_sys\_thickness| varchar(8000)  |
| &#128270; | uf\_sys\_type| varchar(8000)  |
| &#128270; | uf\_thickness| decimal(8,1)  |
| &#128270; | uf\_tile\_flange\_configuration\_a| varchar(8000)  |
| &#128270; | uf\_tubeline\_edit| int  |
| &#128270; | uf\_veneer| varchar(8000)  |
| &#128270; | uf\_vp\_bead\_type| varchar(8000)  |
| &#128270; | uf\_vph\_lower| varchar(8000)  |
| &#128270; | uf\_vp\_length| varchar(8000)  |
| &#128270; | uf\_vp\_position| varchar(8000)  |
| &#128270; | uf\_vp\_qty\_per\_leaf| varchar(8000)  |
| &#128270; | uf\_vp\_shape| varchar(8000)  |
| &#128270; | uf\_vp\_spacing| varchar(8000)  |
| &#128270; | uf\_vp\_type| varchar(8000)  |
| &#128270; | uf\_vp\_width| varchar(8000)  |
| &#128270; | uf\_width| varchar(8000)  |
| &#128270; | uf\_zero\_line\_m2| int  |
| &#128270; | sas\_drawing\_vr\_location| varchar(8000)  |
| &#128270; | uf\_include\_otif| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON co\_line|
| &#128270;  | ClusteredIndex | ON co\_release|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON qty\_ordered|
| &#128270;  | ClusteredIndex | ON qty\_ready|
| &#128270;  | ClusteredIndex | ON qty\_shipped|
| &#128270;  | ClusteredIndex | ON qty\_packed|
| &#128270;  | ClusteredIndex | ON disc|
| &#128270;  | ClusteredIndex | ON cost|
| &#128270;  | ClusteredIndex | ON price|
| &#128270;  | ClusteredIndex | ON ref\_type|
| &#128270;  | ClusteredIndex | ON ref\_num|
| &#128270;  | ClusteredIndex | ON ref\_line\_suf|
| &#128270;  | ClusteredIndex | ON ref\_release|
| &#128270;  | ClusteredIndex | ON due\_date|
| &#128270;  | ClusteredIndex | ON ship\_date|
| &#128270;  | ClusteredIndex | ON reprice|
| &#128270;  | ClusteredIndex | ON cust\_item|
| &#128270;  | ClusteredIndex | ON qty\_invoiced|
| &#128270;  | ClusteredIndex | ON qty\_returned|
| &#128270;  | ClusteredIndex | ON cgs\_total|
| &#128270;  | ClusteredIndex | ON feat\_str|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON cust\_seq|
| &#128270;  | ClusteredIndex | ON prg\_bill\_tot|
| &#128270;  | ClusteredIndex | ON prg\_bill\_app|
| &#128270;  | ClusteredIndex | ON release\_date|
| &#128270;  | ClusteredIndex | ON promise\_date|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON wks\_basis|
| &#128270;  | ClusteredIndex | ON wks\_value|
| &#128270;  | ClusteredIndex | ON comm\_code|
| &#128270;  | ClusteredIndex | ON trans\_nat|
| &#128270;  | ClusteredIndex | ON process\_ind|
| &#128270;  | ClusteredIndex | ON delterm|
| &#128270;  | ClusteredIndex | ON unit\_weight|
| &#128270;  | ClusteredIndex | ON origin|
| &#128270;  | ClusteredIndex | ON cons\_num|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON export\_value|
| &#128270;  | ClusteredIndex | ON ec\_code|
| &#128270;  | ClusteredIndex | ON transport|
| &#128270;  | ClusteredIndex | ON pick\_date|
| &#128270;  | ClusteredIndex | ON pricecode|
| &#128270;  | ClusteredIndex | ON u\_m|
| &#128270;  | ClusteredIndex | ON qty\_ordered\_conv|
| &#128270;  | ClusteredIndex | ON price\_conv|
| &#128270;  | ClusteredIndex | ON co\_cust\_num|
| &#128270;  | ClusteredIndex | ON packed|
| &#128270;  | ClusteredIndex | ON bol|
| &#128270;  | ClusteredIndex | ON qty\_rsvd|
| &#128270;  | ClusteredIndex | ON matl\_cost|
| &#128270;  | ClusteredIndex | ON lbr\_cost|
| &#128270;  | ClusteredIndex | ON fovhd\_cost|
| &#128270;  | ClusteredIndex | ON vovhd\_cost|
| &#128270;  | ClusteredIndex | ON out\_cost|
| &#128270;  | ClusteredIndex | ON cgs\_total\_matl|
| &#128270;  | ClusteredIndex | ON cgs\_total\_lbr|
| &#128270;  | ClusteredIndex | ON cgs\_total\_fovhd|
| &#128270;  | ClusteredIndex | ON cgs\_total\_vovhd|
| &#128270;  | ClusteredIndex | ON cgs\_total\_out|
| &#128270;  | ClusteredIndex | ON cost\_conv|
| &#128270;  | ClusteredIndex | ON matl\_cost\_conv|
| &#128270;  | ClusteredIndex | ON lbr\_cost\_conv|
| &#128270;  | ClusteredIndex | ON fovhd\_cost\_conv|
| &#128270;  | ClusteredIndex | ON vovhd\_cost\_conv|
| &#128270;  | ClusteredIndex | ON out\_cost\_conv|
| &#128270;  | ClusteredIndex | ON ship\_site|
| &#128270;  | ClusteredIndex | ON sync\_reqd|
| &#128270;  | ClusteredIndex | ON co\_orig\_site|
| &#128270;  | ClusteredIndex | ON cust\_po|
| &#128270;  | ClusteredIndex | ON rma\_num|
| &#128270;  | ClusteredIndex | ON rma\_line|
| &#128270;  | ClusteredIndex | ON projected\_date|
| &#128270;  | ClusteredIndex | ON consolidate|
| &#128270;  | ClusteredIndex | ON inv\_freq|
| &#128270;  | ClusteredIndex | ON summarize|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON config\_id|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON rcpt\_rqmt|
| &#128270;  | ClusteredIndex | ON trans\_nat\_2|
| &#128270;  | ClusteredIndex | ON suppl\_qty\_conv\_factor|
| &#128270;  | ClusteredIndex | ON print\_kit\_components|
| &#128270;  | ClusteredIndex | ON due\_date\_day|
| &#128270;  | ClusteredIndex | ON external\_reservation\_ref|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON days\_shipped\_before\_due\_date\_tolerance|
| &#128270;  | ClusteredIndex | ON days\_shipped\_after\_due\_date\_tolerance|
| &#128270;  | ClusteredIndex | ON shipped\_over\_ordered\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON shipped\_under\_ordered\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON priority|
| &#128270;  | ClusteredIndex | ON invoice\_hold|
| &#128270;  | ClusteredIndex | ON manufacturer\_id|
| &#128270;  | ClusteredIndex | ON manufacturer\_item|
| &#128270;  | ClusteredIndex | ON qty\_picked|
| &#128270;  | ClusteredIndex | ON fs\_inc\_num|
| &#128270;  | ClusteredIndex | ON promotion\_code|
| &#128270;  | ClusteredIndex | ON external\_shipment\_line\_id|
| &#128270;  | ClusteredIndex | ON last\_external\_shipment\_doc\_id|
| &#128270;  | ClusteredIndex | ON last\_process\_shipment\_doc\_id|
| &#128270;  | ClusteredIndex | ON allow\_on\_pick\_list|
| &#128270;  | ClusteredIndex | ON external\_shipment\_status|
| &#128270;  | ClusteredIndex | ON exclude\_from\_copy\_to\_co|
| &#128270;  | ClusteredIndex | ON ship\_to\_name|
| &#128270;  | ClusteredIndex | ON ship\_to\_city|
| &#128270;  | ClusteredIndex | ON ship\_to\_state|
| &#128270;  | ClusteredIndex | ON ship\_to\_zip|
| &#128270;  | ClusteredIndex | ON ship\_to\_county|
| &#128270;  | ClusteredIndex | ON ship\_to\_country|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_1|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_2|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_3|
| &#128270;  | ClusteredIndex | ON ship\_to\_addr\_4|
| &#128270;  | ClusteredIndex | ON pl\_override\_item\_description|
| &#128270;  | ClusteredIndex | ON pl\_alternate\_item\_description|
| &#128270;  | ClusteredIndex | ON uf\_amend\_route|
| &#128270;  | ClusteredIndex | ON uf\_appc|
| &#128270;  | ClusteredIndex | ON uf\_bepc|
| &#128270;  | ClusteredIndex | ON uf\_bfi\_price|
| &#128270;  | ClusteredIndex | ON uf\_bom\_unit\_price|
| &#128270;  | ClusteredIndex | ON uf\_comp\_matl|
| &#128270;  | ClusteredIndex | ON uf\_comp\_run|
| &#128270;  | ClusteredIndex | ON uf\_comp\_setup|
| &#128270;  | ClusteredIndex | ON uf\_config\_status|
| &#128270;  | ClusteredIndex | ON uf\_config\_staus|
| &#128270;  | ClusteredIndex | ON uf\_co\_stat|
| &#128270;  | ClusteredIndex | ON uf\_created|
| &#128270;  | ClusteredIndex | ON uf\_cur\_lbr\_cost|
| &#128270;  | ClusteredIndex | ON uf\_cur\_matl\_cost|
| &#128270;  | ClusteredIndex | ON uf\_cur\_out\_cost|
| &#128270;  | ClusteredIndex | ON uf\_curr\_trn\_price|
| &#128270;  | ClusteredIndex | ON uf\_cust\_del\_date|
| &#128270;  | ClusteredIndex | ON uf\_cust\_req|
| &#128270;  | ClusteredIndex | ON uf\_distribution|
| &#128270;  | ClusteredIndex | ON uf\_division|
| &#128270;  | ClusteredIndex | ON uf\_floor\_zone|
| &#128270;  | ClusteredIndex | ON uf\_floor\_zone\_description|
| &#128270;  | ClusteredIndex | ON uf\_long\_description|
| &#128270;  | ClusteredIndex | ON uf\_m2|
| &#128270;  | ClusteredIndex | ON uf\_m2\_tot|
| &#128270;  | ClusteredIndex | ON uf\_m2\_tot\_price|
| &#128270;  | ClusteredIndex | ON uf\_margin|
| &#128270;  | ClusteredIndex | ON uf\_mbpc|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_lin\_suf|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_num|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_release|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_type|
| &#128270;  | ClusteredIndex | ON uf\_one\_piece\_route|
| &#128270;  | ClusteredIndex | ON uf\_ordered\_date|
| &#128270;  | ClusteredIndex | ON uf\_orig\_ack\_del\_date|
| &#128270;  | ClusteredIndex | ON uf\_release|
| &#128270;  | ClusteredIndex | ON uf\_release\_date|
| &#128270;  | ClusteredIndex | ON uf\_same\_day|
| &#128270;  | ClusteredIndex | ON uf\_sas\_cost|
| &#128270;  | ClusteredIndex | ON uf\_sequence|
| &#128270;  | ClusteredIndex | ON uf\_ship\_location|
| &#128270;  | ClusteredIndex | ON uf\_standard|
| &#128270;  | ClusteredIndex | ON uf\_trn\_cost|
| &#128270;  | ClusteredIndex | ON uf\_trn\_price|
| &#128270;  | ClusteredIndex | ON uf\_acoustic|
| &#128270;  | ClusteredIndex | ON uf\_additional\_description|
| &#128270;  | ClusteredIndex | ON uf\_angle|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_offset|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_size|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_type|
| &#128270;  | ClusteredIndex | ON uf\_architrave|
| &#128270;  | ClusteredIndex | ON uf\_birdsmouth\_detail|
| &#128270;  | ClusteredIndex | ON uf\_cat\_ref|
| &#128270;  | ClusteredIndex | ON uf\_co\_line\_config\_description|
| &#128270;  | ClusteredIndex | ON uf\_depth|
| &#128270;  | ClusteredIndex | ON uf\_diameter\_offset|
| &#128270;  | ClusteredIndex | ON uf\_diameter\_size|
| &#128270;  | ClusteredIndex | ON uf\_door\_cat|
| &#128270;  | ClusteredIndex | ON uf\_door\_leaf\_type|
| &#128270;  | ClusteredIndex | ON uf\_door\_type|
| &#128270;  | ClusteredIndex | ON uf\_dr\_frm\_config|
| &#128270;  | ClusteredIndex | ON uf\_edge\_config|
| &#128270;  | ClusteredIndex | ON uf\_edgeor\_grid\_size|
| &#128270;  | ClusteredIndex | ON uf\_frame\_finish|
| &#128270;  | ClusteredIndex | ON uf\_frame\_type|
| &#128270;  | ClusteredIndex | ON uf\_galv|
| &#128270;  | ClusteredIndex | ON uf\_gasket|
| &#128270;  | ClusteredIndex | ON uf\_gauge|
| &#128270;  | ClusteredIndex | ON uf\_glaz\_pckt|
| &#128270;  | ClusteredIndex | ON uf\_handing|
| &#128270;  | ClusteredIndex | ON uf\_hinges|
| &#128270;  | ClusteredIndex | ON uf\_insulation\_type|
| &#128270;  | ClusteredIndex | ON uf\_ironmongery|
| &#128270;  | ClusteredIndex | ON uf\_issue\_no|
| &#128270;  | ClusteredIndex | ON uf\_length|
| &#128270;  | ClusteredIndex | ON uf\_linear\_m\_price|
| &#128270;  | ClusteredIndex | ON uf\_lipping|
| &#128270;  | ClusteredIndex | ON uf\_location|
| &#128270;  | ClusteredIndex | ON uf\_manufacturer|
| &#128270;  | ClusteredIndex | ON uf\_material\_type|
| &#128270;  | ClusteredIndex | ON uf\_module|
| &#128270;  | ClusteredIndex | ON uf\_module\_length|
| &#128270;  | ClusteredIndex | ON uf\_module\_width|
| &#128270;  | ClusteredIndex | ON uf\_nominal\_border|
| &#128270;  | ClusteredIndex | ON uf\_non\_fire\_rated|
| &#128270;  | ClusteredIndex | ON uf\_over\_panel\_h|
| &#128270;  | ClusteredIndex | ON uf\_paint|
| &#128270;  | ClusteredIndex | ON uf\_partion\_system\_type|
| &#128270;  | ClusteredIndex | ON uf\_partit\_glaze|
| &#128270;  | ClusteredIndex | ON uf\_partition|
| &#128270;  | ClusteredIndex | ON uf\_partition\_type|
| &#128270;  | ClusteredIndex | ON uf\_perf|
| &#128270;  | ClusteredIndex | ON uf\_periphery|
| &#128270;  | ClusteredIndex | ON uf\_product\_type1|
| &#128270;  | ClusteredIndex | ON uf\_profile\_type|
| &#128270;  | ClusteredIndex | ON uf\_site|
| &#128270;  | ClusteredIndex | ON uf\_slave\_leaf\_w|
| &#128270;  | ClusteredIndex | ON uf\_snap\_infill|
| &#128270;  | ClusteredIndex | ON uf\_strike\_plate|
| &#128270;  | ClusteredIndex | ON uf\_sustainability|
| &#128270;  | ClusteredIndex | ON uf\_swing\_type|
| &#128270;  | ClusteredIndex | ON uf\_sys|
| &#128270;  | ClusteredIndex | ON uf\_sys\_thickness|
| &#128270;  | ClusteredIndex | ON uf\_sys\_type|
| &#128270;  | ClusteredIndex | ON uf\_thickness|
| &#128270;  | ClusteredIndex | ON uf\_tile\_flange\_configuration\_a|
| &#128270;  | ClusteredIndex | ON uf\_tubeline\_edit|
| &#128270;  | ClusteredIndex | ON uf\_veneer|
| &#128270;  | ClusteredIndex | ON uf\_vp\_bead\_type|
| &#128270;  | ClusteredIndex | ON uf\_vph\_lower|
| &#128270;  | ClusteredIndex | ON uf\_vp\_length|
| &#128270;  | ClusteredIndex | ON uf\_vp\_position|
| &#128270;  | ClusteredIndex | ON uf\_vp\_qty\_per\_leaf|
| &#128270;  | ClusteredIndex | ON uf\_vp\_shape|
| &#128270;  | ClusteredIndex | ON uf\_vp\_spacing|
| &#128270;  | ClusteredIndex | ON uf\_vp\_type|
| &#128270;  | ClusteredIndex | ON uf\_vp\_width|
| &#128270;  | ClusteredIndex | ON uf\_width|
| &#128270;  | ClusteredIndex | ON uf\_zero\_line\_m2|
| &#128270;  | ClusteredIndex | ON sas\_drawing\_vr\_location|
| &#128270;  | ClusteredIndex | ON uf\_include\_otif|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table metadata.config_import_batch 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | batch\_id| varchar(36)  |
| * &#128270; | config\_type| varchar(30)  |
| &#128270; | source\_file| varchar(400)  |
| * &#128270; | status| varchar(30)  |
| &#128270; | row\_count| int  |
| &#128270; | error\_count| int  |
| * &#128270; | started\_at| datetime2(26)  |
| &#128270; | completed\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_config\_import\_batch | ON batch\_id|
| &#128270;  | ClusteredIndex | ON config\_type|
| &#128270;  | ClusteredIndex | ON source\_file|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON row\_count|
| &#128270;  | ClusteredIndex | ON error\_count|
| &#128270;  | ClusteredIndex | ON started\_at|
| &#128270;  | ClusteredIndex | ON completed\_at|



### Table metadata.config_import_error 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | error\_id| bigint identity  |
| * &#128270; | batch\_id| varchar(36)  |
| &#128270; | source\_row\_number| int  |
| &#128270; | business\_key| varchar(400)  |
| &#128270; | column\_name| varchar(128)  |
| * &#128270; | error\_message| varchar(400)  |
| * &#128270; | created\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_config\_import\_error | ON error\_id|
| &#128270;  | ClusteredIndex | ON batch\_id|
| &#128270;  | ClusteredIndex | ON source\_row\_number|
| &#128270;  | ClusteredIndex | ON business\_key|
| &#128270;  | ClusteredIndex | ON column\_name|
| &#128270;  | ClusteredIndex | ON error\_message|
| &#128270;  | ClusteredIndex | ON created\_at|



### Table salesforce_staging.contact 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | master\_record\_id| varchar(8000)  |
| &#128270; | account\_id| varchar(8000)  |
| &#128270; | last\_name| varchar(8000)  |
| &#128270; | first\_name| varchar(8000)  |
| &#128270; | salutation| varchar(8000)  |
| &#128270; | middle\_name| varchar(8000)  |
| &#128270; | suffix| varchar(8000)  |
| &#128270; | name| varchar(8000)  |
| &#128270; | other\_street| varchar(8000)  |
| &#128270; | other\_city| varchar(8000)  |
| &#128270; | other\_state| varchar(8000)  |
| &#128270; | other\_postal\_code| varchar(8000)  |
| &#128270; | other\_country| varchar(8000)  |
| &#128270; | other\_state\_code| varchar(8000)  |
| &#128270; | other\_country\_code| varchar(8000)  |
| &#128270; | other\_latitude| decimal(38,18)  |
| &#128270; | other\_longitude| decimal(38,18)  |
| &#128270; | other\_geocode\_accuracy| varchar(8000)  |
| &#128270; | mailing\_street| varchar(8000)  |
| &#128270; | mailing\_city| varchar(8000)  |
| &#128270; | mailing\_state| varchar(8000)  |
| &#128270; | mailing\_postal\_code| varchar(8000)  |
| &#128270; | mailing\_country| varchar(8000)  |
| &#128270; | mailing\_state\_code| varchar(8000)  |
| &#128270; | mailing\_country\_code| varchar(8000)  |
| &#128270; | mailing\_latitude| decimal(38,18)  |
| &#128270; | mailing\_longitude| decimal(38,18)  |
| &#128270; | mailing\_geocode\_accuracy| varchar(8000)  |
| &#128270; | phone| varchar(8000)  |
| &#128270; | fax| varchar(8000)  |
| &#128270; | mobile\_phone| varchar(8000)  |
| &#128270; | home\_phone| varchar(8000)  |
| &#128270; | other\_phone| varchar(8000)  |
| &#128270; | assistant\_phone| varchar(8000)  |
| &#128270; | reports\_to\_id| varchar(8000)  |
| &#128270; | email| varchar(8000)  |
| &#128270; | title| varchar(8000)  |
| &#128270; | department| varchar(8000)  |
| &#128270; | assistant\_name| varchar(8000)  |
| &#128270; | lead\_source| varchar(8000)  |
| &#128270; | birthdate| datetime2(26)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | owner\_id| varchar(8000)  |
| &#128270; | has\_opted\_out\_of\_email| bit  |
| &#128270; | has\_opted\_out\_of\_fax| bit  |
| &#128270; | do\_not\_call| bit  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_cu\_request\_date| datetime2(26)  |
| &#128270; | last\_cu\_update\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | email\_bounced\_reason| varchar(8000)  |
| &#128270; | email\_bounced\_date| datetime2(26)  |
| &#128270; | is\_email\_bounced| bit  |
| &#128270; | photo\_url| varchar(8000)  |
| &#128270; | jigsaw| varchar(8000)  |
| &#128270; | jigsaw\_contact\_id| varchar(8000)  |
| &#128270; | individual\_id| varchar(8000)  |
| &#128270; | engagement\_score\_id| varchar(8000)  |
| &#128270; | pi\_\_needs\_score\_synced| bit  |
| &#128270; | pi\_\_pardot\_last\_scored\_at| datetime2(26)  |
| &#128270; | pi\_\_campaign| varchar(8000)  |
| &#128270; | pi\_\_comments| varchar(8000)  |
| &#128270; | pi\_\_conversion\_date| datetime2(26)  |
| &#128270; | pi\_\_conversion\_object\_name| varchar(8000)  |
| &#128270; | pi\_\_conversion\_object\_type| varchar(8000)  |
| &#128270; | pi\_\_created\_date| datetime2(26)  |
| &#128270; | pi\_\_first\_activity| datetime2(26)  |
| &#128270; | pi\_\_first\_search\_term| varchar(8000)  |
| &#128270; | pi\_\_first\_search\_type| varchar(8000)  |
| &#128270; | pi\_\_first\_touch\_url| varchar(8000)  |
| &#128270; | pi\_\_grade| varchar(8000)  |
| &#128270; | pi\_\_last\_activity| datetime2(26)  |
| &#128270; | pi\_\_notes| varchar(8000)  |
| &#128270; | pi\_\_pardot\_hard\_bounced| bit  |
| &#128270; | pi\_\_score| decimal(38,18)  |
| &#128270; | pi\_\_url| varchar(8000)  |
| &#128270; | pi\_\_utm\_campaign| varchar(8000)  |
| &#128270; | pi\_\_utm\_content| varchar(8000)  |
| &#128270; | pi\_\_utm\_medium| varchar(8000)  |
| &#128270; | pi\_\_utm\_source| varchar(8000)  |
| &#128270; | pi\_\_utm\_term| varchar(8000)  |
| &#128270; | send\_nps| bit  |
| &#128270; | cpd\_attended\_date| datetime2(26)  |
| &#128270; | cpd\_attended| varchar(8000)  |
| &#128270; | contact\_notes| varchar(8000)  |
| &#128270; | country| varchar(8000)  |
| &#128270; | do\_not\_send\_marketing\_emails| bit  |
| &#128270; | hospitality\_atteneded| datetime2(26)  |
| &#128270; | infor\_contact\_id| varchar(8000)  |
| &#128270; | infor\_reference| varchar(8000)  |
| &#128270; | job\_role\_if\_other| varchar(8000)  |
| &#128270; | job\_role| varchar(8000)  |
| &#128270; | job\_seniority| varchar(8000)  |
| &#128270; | job\_title| varchar(8000)  |
| &#128270; | known\_as| varchar(8000)  |
| &#128270; | line\_manager| varchar(8000)  |
| &#128270; | linked\_in\_profile| varchar(8000)  |
| &#128270; | most\_recent\_nps\_completed| datetime2(26)  |
| &#128270; | most\_recent\_nps\_sent| datetime2(26)  |
| &#128270; | most\_recent\_nps\_score| decimal(38,18)  |
| &#128270; | nps\_improvements\_feedback| varchar(8000)  |
| &#128270; | nps\_positive\_feedback| varchar(8000)  |
| &#128270; | sas\_mailings\_marketing\_activity| varchar(8000)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | sales\_region| varchar(8000)  |
| &#128270; | town| varchar(8000)  |
| &#128270; | twitter\_profile| varchar(8000)  |
| &#128270; | sansancard\_\_created\_by\_scan\_to\_salesforce| bit  |
| &#128270; | hospitality\_notes| varchar(8000)  |
| &#128270; | contact\_summary| varchar(8000)  |
| &#128270; | notes\_completed| bit  |
| &#128270; | marketable\_prospects| bit  |
| &#128270; | last\_form\_submission\_date| datetime2(26)  |
| &#128270; | last\_pardot\_task\_date| datetime2(26)  |
| &#128270; | last\_estimate\_date| datetime2(26)  |
| &#128270; | last\_order\_date| datetime2(26)  |
| &#128270; | infor\_error| varchar(8000)  |
| &#128270; | infor\_last\_updated| datetime2(26)  |
| &#128270; | infor\_status| varchar(8000)  |
| &#128270; | lead\_time\_on\_receiving\_quotation| varchar(8000)  |
| &#128270; | lead\_time\_on\_order\_acknowledgement| varchar(8000)  |
| &#128270; | at\_delivery\_dates\_being\_achieved| varchar(8000)  |
| &#128270; | quality\_of\_product| varchar(8000)  |
| &#128270; | keeping\_in\_touch\_visiting| varchar(8000)  |
| &#128270; | what\_is\_your\_expectation\_of\_communicatio| varchar(8000)  |
| &#128270; | primary\_contact| bit  |
| &#128270; | samples\_requested| varchar(8000)  |
| &#128270; | delivery\_address| varchar(8000)  |
| &#128270; | phone\_extension| varchar(8000)  |
| &#128270; | company\_email| varchar(8000)  |
| &#128270; | company\_legal\_name| varchar(8000)  |
| &#128270; | vat\_tax\_id| varchar(8000)  |
| &#128270; | reseller\_id| varchar(8000)  |
| &#128270; | customer\_infor\_reference| varchar(8000)  |
| &#128270; | target\_contact| bit  |
| &#128270; | chilled\_products\_date| datetime2(26)  |
| &#128270; | chilled\_products\_introduced| bit  |
| &#128270; | escalation\_contact| bit  |
| &#128270; | key\_contact| bit  |
| &#128270; | major\_hospitality\_date| datetime2(26)  |
| &#128270; | major\_hospitality\_event\_attended| bit  |
| &#128270; | minor\_hospitality\_date| datetime2(26)  |
| &#128270; | minor\_hospitality\_event\_attended| bit  |
| &#128270; | proposal\_issued\_date| datetime2(26)  |
| &#128270; | proposal\_issued| bit  |
| &#128270; | special\_projects\_introduced\_date| datetime2(26)  |
| &#128270; | special\_projects\_introduced| bit  |
| &#128270; | specification\_issued\_date| datetime2(26)  |
| &#128270; | specification\_issued| bit  |
| &#128270; | sustainability\_introduction\_date| datetime2(26)  |
| &#128270; | sustainability\_introduction| bit  |
| &#128270; | e\_commerce\_enquiry\_type| varchar(8000)  |
| &#128270; | core\_products\_introduced| bit  |
| &#128270; | latest\_complaint\_nps\_completed| datetime2(26)  |
| &#128270; | latest\_estimate\_nps\_completed| datetime2(26)  |
| &#128270; | latest\_order\_nps\_completed| datetime2(26)  |
| &#128270; | latest\_proposal\_nps\_completed| datetime2(26)  |
| &#128270; | latest\_specification\_nps\_completed| datetime2(26)  |
| &#128270; | company\_type| varchar(8000)  |
| &#128270; | order\_issued\_send\_nps| bit  |
| &#128270; | email\_domain| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON master\_record\_id|
| &#128270;  | ClusteredIndex | ON account\_id|
| &#128270;  | ClusteredIndex | ON last\_name|
| &#128270;  | ClusteredIndex | ON first\_name|
| &#128270;  | ClusteredIndex | ON salutation|
| &#128270;  | ClusteredIndex | ON middle\_name|
| &#128270;  | ClusteredIndex | ON suffix|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON other\_street|
| &#128270;  | ClusteredIndex | ON other\_city|
| &#128270;  | ClusteredIndex | ON other\_state|
| &#128270;  | ClusteredIndex | ON other\_postal\_code|
| &#128270;  | ClusteredIndex | ON other\_country|
| &#128270;  | ClusteredIndex | ON other\_state\_code|
| &#128270;  | ClusteredIndex | ON other\_country\_code|
| &#128270;  | ClusteredIndex | ON other\_latitude|
| &#128270;  | ClusteredIndex | ON other\_longitude|
| &#128270;  | ClusteredIndex | ON other\_geocode\_accuracy|
| &#128270;  | ClusteredIndex | ON mailing\_street|
| &#128270;  | ClusteredIndex | ON mailing\_city|
| &#128270;  | ClusteredIndex | ON mailing\_state|
| &#128270;  | ClusteredIndex | ON mailing\_postal\_code|
| &#128270;  | ClusteredIndex | ON mailing\_country|
| &#128270;  | ClusteredIndex | ON mailing\_state\_code|
| &#128270;  | ClusteredIndex | ON mailing\_country\_code|
| &#128270;  | ClusteredIndex | ON mailing\_latitude|
| &#128270;  | ClusteredIndex | ON mailing\_longitude|
| &#128270;  | ClusteredIndex | ON mailing\_geocode\_accuracy|
| &#128270;  | ClusteredIndex | ON phone|
| &#128270;  | ClusteredIndex | ON fax|
| &#128270;  | ClusteredIndex | ON mobile\_phone|
| &#128270;  | ClusteredIndex | ON home\_phone|
| &#128270;  | ClusteredIndex | ON other\_phone|
| &#128270;  | ClusteredIndex | ON assistant\_phone|
| &#128270;  | ClusteredIndex | ON reports\_to\_id|
| &#128270;  | ClusteredIndex | ON email|
| &#128270;  | ClusteredIndex | ON title|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON assistant\_name|
| &#128270;  | ClusteredIndex | ON lead\_source|
| &#128270;  | ClusteredIndex | ON birthdate|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON owner\_id|
| &#128270;  | ClusteredIndex | ON has\_opted\_out\_of\_email|
| &#128270;  | ClusteredIndex | ON has\_opted\_out\_of\_fax|
| &#128270;  | ClusteredIndex | ON do\_not\_call|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_cu\_request\_date|
| &#128270;  | ClusteredIndex | ON last\_cu\_update\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON email\_bounced\_reason|
| &#128270;  | ClusteredIndex | ON email\_bounced\_date|
| &#128270;  | ClusteredIndex | ON is\_email\_bounced|
| &#128270;  | ClusteredIndex | ON photo\_url|
| &#128270;  | ClusteredIndex | ON jigsaw|
| &#128270;  | ClusteredIndex | ON jigsaw\_contact\_id|
| &#128270;  | ClusteredIndex | ON individual\_id|
| &#128270;  | ClusteredIndex | ON engagement\_score\_id|
| &#128270;  | ClusteredIndex | ON pi\_\_needs\_score\_synced|
| &#128270;  | ClusteredIndex | ON pi\_\_pardot\_last\_scored\_at|
| &#128270;  | ClusteredIndex | ON pi\_\_campaign|
| &#128270;  | ClusteredIndex | ON pi\_\_comments|
| &#128270;  | ClusteredIndex | ON pi\_\_conversion\_date|
| &#128270;  | ClusteredIndex | ON pi\_\_conversion\_object\_name|
| &#128270;  | ClusteredIndex | ON pi\_\_conversion\_object\_type|
| &#128270;  | ClusteredIndex | ON pi\_\_created\_date|
| &#128270;  | ClusteredIndex | ON pi\_\_first\_activity|
| &#128270;  | ClusteredIndex | ON pi\_\_first\_search\_term|
| &#128270;  | ClusteredIndex | ON pi\_\_first\_search\_type|
| &#128270;  | ClusteredIndex | ON pi\_\_first\_touch\_url|
| &#128270;  | ClusteredIndex | ON pi\_\_grade|
| &#128270;  | ClusteredIndex | ON pi\_\_last\_activity|
| &#128270;  | ClusteredIndex | ON pi\_\_notes|
| &#128270;  | ClusteredIndex | ON pi\_\_pardot\_hard\_bounced|
| &#128270;  | ClusteredIndex | ON pi\_\_score|
| &#128270;  | ClusteredIndex | ON pi\_\_url|
| &#128270;  | ClusteredIndex | ON pi\_\_utm\_campaign|
| &#128270;  | ClusteredIndex | ON pi\_\_utm\_content|
| &#128270;  | ClusteredIndex | ON pi\_\_utm\_medium|
| &#128270;  | ClusteredIndex | ON pi\_\_utm\_source|
| &#128270;  | ClusteredIndex | ON pi\_\_utm\_term|
| &#128270;  | ClusteredIndex | ON send\_nps|
| &#128270;  | ClusteredIndex | ON cpd\_attended\_date|
| &#128270;  | ClusteredIndex | ON cpd\_attended|
| &#128270;  | ClusteredIndex | ON contact\_notes|
| &#128270;  | ClusteredIndex | ON country|
| &#128270;  | ClusteredIndex | ON do\_not\_send\_marketing\_emails|
| &#128270;  | ClusteredIndex | ON hospitality\_atteneded|
| &#128270;  | ClusteredIndex | ON infor\_contact\_id|
| &#128270;  | ClusteredIndex | ON infor\_reference|
| &#128270;  | ClusteredIndex | ON job\_role\_if\_other|
| &#128270;  | ClusteredIndex | ON job\_role|
| &#128270;  | ClusteredIndex | ON job\_seniority|
| &#128270;  | ClusteredIndex | ON job\_title|
| &#128270;  | ClusteredIndex | ON known\_as|
| &#128270;  | ClusteredIndex | ON line\_manager|
| &#128270;  | ClusteredIndex | ON linked\_in\_profile|
| &#128270;  | ClusteredIndex | ON most\_recent\_nps\_completed|
| &#128270;  | ClusteredIndex | ON most\_recent\_nps\_sent|
| &#128270;  | ClusteredIndex | ON most\_recent\_nps\_score|
| &#128270;  | ClusteredIndex | ON nps\_improvements\_feedback|
| &#128270;  | ClusteredIndex | ON nps\_positive\_feedback|
| &#128270;  | ClusteredIndex | ON sas\_mailings\_marketing\_activity|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON sales\_region|
| &#128270;  | ClusteredIndex | ON town|
| &#128270;  | ClusteredIndex | ON twitter\_profile|
| &#128270;  | ClusteredIndex | ON sansancard\_\_created\_by\_scan\_to\_salesforce|
| &#128270;  | ClusteredIndex | ON hospitality\_notes|
| &#128270;  | ClusteredIndex | ON contact\_summary|
| &#128270;  | ClusteredIndex | ON notes\_completed|
| &#128270;  | ClusteredIndex | ON marketable\_prospects|
| &#128270;  | ClusteredIndex | ON last\_form\_submission\_date|
| &#128270;  | ClusteredIndex | ON last\_pardot\_task\_date|
| &#128270;  | ClusteredIndex | ON last\_estimate\_date|
| &#128270;  | ClusteredIndex | ON last\_order\_date|
| &#128270;  | ClusteredIndex | ON infor\_error|
| &#128270;  | ClusteredIndex | ON infor\_last\_updated|
| &#128270;  | ClusteredIndex | ON infor\_status|
| &#128270;  | ClusteredIndex | ON lead\_time\_on\_receiving\_quotation|
| &#128270;  | ClusteredIndex | ON lead\_time\_on\_order\_acknowledgement|
| &#128270;  | ClusteredIndex | ON at\_delivery\_dates\_being\_achieved|
| &#128270;  | ClusteredIndex | ON quality\_of\_product|
| &#128270;  | ClusteredIndex | ON keeping\_in\_touch\_visiting|
| &#128270;  | ClusteredIndex | ON what\_is\_your\_expectation\_of\_communicatio|
| &#128270;  | ClusteredIndex | ON primary\_contact|
| &#128270;  | ClusteredIndex | ON samples\_requested|
| &#128270;  | ClusteredIndex | ON delivery\_address|
| &#128270;  | ClusteredIndex | ON phone\_extension|
| &#128270;  | ClusteredIndex | ON company\_email|
| &#128270;  | ClusteredIndex | ON company\_legal\_name|
| &#128270;  | ClusteredIndex | ON vat\_tax\_id|
| &#128270;  | ClusteredIndex | ON reseller\_id|
| &#128270;  | ClusteredIndex | ON customer\_infor\_reference|
| &#128270;  | ClusteredIndex | ON target\_contact|
| &#128270;  | ClusteredIndex | ON chilled\_products\_date|
| &#128270;  | ClusteredIndex | ON chilled\_products\_introduced|
| &#128270;  | ClusteredIndex | ON escalation\_contact|
| &#128270;  | ClusteredIndex | ON key\_contact|
| &#128270;  | ClusteredIndex | ON major\_hospitality\_date|
| &#128270;  | ClusteredIndex | ON major\_hospitality\_event\_attended|
| &#128270;  | ClusteredIndex | ON minor\_hospitality\_date|
| &#128270;  | ClusteredIndex | ON minor\_hospitality\_event\_attended|
| &#128270;  | ClusteredIndex | ON proposal\_issued\_date|
| &#128270;  | ClusteredIndex | ON proposal\_issued|
| &#128270;  | ClusteredIndex | ON special\_projects\_introduced\_date|
| &#128270;  | ClusteredIndex | ON special\_projects\_introduced|
| &#128270;  | ClusteredIndex | ON specification\_issued\_date|
| &#128270;  | ClusteredIndex | ON specification\_issued|
| &#128270;  | ClusteredIndex | ON sustainability\_introduction\_date|
| &#128270;  | ClusteredIndex | ON sustainability\_introduction|
| &#128270;  | ClusteredIndex | ON e\_commerce\_enquiry\_type|
| &#128270;  | ClusteredIndex | ON core\_products\_introduced|
| &#128270;  | ClusteredIndex | ON latest\_complaint\_nps\_completed|
| &#128270;  | ClusteredIndex | ON latest\_estimate\_nps\_completed|
| &#128270;  | ClusteredIndex | ON latest\_order\_nps\_completed|
| &#128270;  | ClusteredIndex | ON latest\_proposal\_nps\_completed|
| &#128270;  | ClusteredIndex | ON latest\_specification\_nps\_completed|
| &#128270;  | ClusteredIndex | ON company\_type|
| &#128270;  | ClusteredIndex | ON order\_issued\_send\_nps|
| &#128270;  | ClusteredIndex | ON email\_domain|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table metadata.curation_execution 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | execution\_id| bigint identity  |
| * &#128270; | run\_id| bigint  |
| * &#128270; | procedure\_id| bigint  |
| * &#128270; | schema\_name| varchar(128)  |
| * &#128270; | procedure\_name| varchar(128)  |
| * &#128270; | execution\_group| int  |
| * &#128270; | execution\_order| int  |
| * &#128270; | status| varchar(30)  |
| * &#128270; | start\_time| datetime2(26)  |
| &#128270; | end\_time| datetime2(26)  |
| &#128270; | error\_number| int  |
| &#128270; | error\_message| varchar(4000)  |
| * &#128270; | created\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_curation\_execution | ON execution\_id|
| &#128270;  | ClusteredIndex | ON run\_id|
| &#128270;  | ClusteredIndex | ON procedure\_id|
| &#128270;  | ClusteredIndex | ON schema\_name|
| &#128270;  | ClusteredIndex | ON procedure\_name|
| &#128270;  | ClusteredIndex | ON execution\_group|
| &#128270;  | ClusteredIndex | ON execution\_order|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON start\_time|
| &#128270;  | ClusteredIndex | ON end\_time|
| &#128270;  | ClusteredIndex | ON error\_number|
| &#128270;  | ClusteredIndex | ON error\_message|
| &#128270;  | ClusteredIndex | ON created\_at|



### Table metadata.curation_procedure 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | procedure\_id| bigint identity  |
| * &#128269; | schema\_name| varchar(128)  |
| * &#128269; | procedure\_name| varchar(128)  |
| * &#128270; | execution\_group| int  |
| * &#128270; | execution\_order| int  |
| * &#128270; | continue\_on\_error| bit  |
| * &#128270; | is\_active| bit  |
| * &#128270; | created\_at| datetime2(26)  |
| * &#128270; | updated\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_curation\_procedure | ON procedure\_id|
| &#128269;  | uq\_curation\_procedure\_name | ON schema\_name, procedure\_name|
| &#128270;  | ClusteredIndex | ON schema\_name|
| &#128270;  | ClusteredIndex | ON procedure\_name|
| &#128270;  | ClusteredIndex | ON execution\_group|
| &#128270;  | ClusteredIndex | ON execution\_order|
| &#128270;  | ClusteredIndex | ON continue\_on\_error|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON created\_at|
| &#128270;  | ClusteredIndex | ON updated\_at|



### Table staging.curation_procedure_import 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | batch\_id| varchar(36)  |
| * &#128270; | source\_row\_number| varchar(20)  |
| &#128270; | schema\_name| varchar(400)  |
| &#128270; | procedure\_name| varchar(400)  |
| &#128270; | execution\_group| varchar(20)  |
| &#128270; | execution\_order| varchar(20)  |
| &#128270; | continue\_on\_error| varchar(10)  |
| &#128270; | is\_active| varchar(10)  |
| * &#128270; | loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON batch\_id|
| &#128270;  | ClusteredIndex | ON source\_row\_number|
| &#128270;  | ClusteredIndex | ON schema\_name|
| &#128270;  | ClusteredIndex | ON procedure\_name|
| &#128270;  | ClusteredIndex | ON execution\_group|
| &#128270;  | ClusteredIndex | ON execution\_order|
| &#128270;  | ClusteredIndex | ON continue\_on\_error|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON loaded\_at|



### Table syteline_staging.currate_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | from\_curr\_code| varchar(8000)  |
| &#128270; | eff\_date| datetime2(26)  |
| &#128270; | buy\_rate| decimal(12,7)  |
| &#128270; | sell\_rate| decimal(12,7)  |
| &#128270; | user\_code| varchar(8000)  |
| &#128270; | to\_curr\_code| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | pl\_bank\_exch\_rate\_table| varchar(8000)  |
| &#128270; | pl\_bank\_exch\_rate\_additional\_info| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON from\_curr\_code|
| &#128270;  | ClusteredIndex | ON eff\_date|
| &#128270;  | ClusteredIndex | ON buy\_rate|
| &#128270;  | ClusteredIndex | ON sell\_rate|
| &#128270;  | ClusteredIndex | ON user\_code|
| &#128270;  | ClusteredIndex | ON to\_curr\_code|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON pl\_bank\_exch\_rate\_table|
| &#128270;  | ClusteredIndex | ON pl\_bank\_exch\_rate\_additional\_info|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.custaddr_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | cust\_seq| int  |
| &#128270; | name| varchar(8000)  |
| &#128270; | city| varchar(8000)  |
| &#128270; | state| varchar(8000)  |
| &#128270; | zip| varchar(8000)  |
| &#128270; | county| varchar(8000)  |
| &#128270; | country| varchar(8000)  |
| &#128270; | fax\_num| varchar(8000)  |
| &#128270; | telex\_num| varchar(8000)  |
| &#128270; | bal\_method| varchar(8000)  |
| &#128270; | addr\_1| varchar(8000)  |
| &#128270; | addr\_2| varchar(8000)  |
| &#128270; | addr\_3| varchar(8000)  |
| &#128270; | addr\_4| varchar(8000)  |
| &#128270; | credit\_hold| int  |
| &#128270; | credit\_hold\_user| varchar(8000)  |
| &#128270; | credit\_hold\_date| datetime2(26)  |
| &#128270; | credit\_hold\_reason| varchar(8000)  |
| &#128270; | credit\_limit| decimal(23,8)  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | corp\_cust| varchar(8000)  |
| &#128270; | corp\_cred| int  |
| &#128270; | corp\_address| int  |
| &#128270; | amt\_over\_inv\_amt| decimal(23,8)  |
| &#128270; | days\_over\_inv\_due\_date| int  |
| &#128270; | ship\_to\_email| varchar(8000)  |
| &#128270; | bill\_to\_email| varchar(8000)  |
| &#128270; | internet\_url| varchar(8000)  |
| &#128270; | internal\_email\_addr| varchar(8000)  |
| &#128270; | external\_email\_addr| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | carrier\_account| varchar(8000)  |
| &#128270; | carrier\_upcharge\_pct| decimal(4,2)  |
| &#128270; | carrier\_residential\_indicator| int  |
| &#128270; | carrier\_bill\_to\_transportation| varchar(8000)  |
| &#128270; | order\_credit\_limit| decimal(23,8)  |
| &#128270; | use\_long\_name| int  |
| &#128270; | long\_name| varchar(8000)  |
| &#128270; | uf\_send\_automated\_pod| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON cust\_seq|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON city|
| &#128270;  | ClusteredIndex | ON state|
| &#128270;  | ClusteredIndex | ON zip|
| &#128270;  | ClusteredIndex | ON county|
| &#128270;  | ClusteredIndex | ON country|
| &#128270;  | ClusteredIndex | ON fax\_num|
| &#128270;  | ClusteredIndex | ON telex\_num|
| &#128270;  | ClusteredIndex | ON bal\_method|
| &#128270;  | ClusteredIndex | ON addr\_1|
| &#128270;  | ClusteredIndex | ON addr\_2|
| &#128270;  | ClusteredIndex | ON addr\_3|
| &#128270;  | ClusteredIndex | ON addr\_4|
| &#128270;  | ClusteredIndex | ON credit\_hold|
| &#128270;  | ClusteredIndex | ON credit\_hold\_user|
| &#128270;  | ClusteredIndex | ON credit\_hold\_date|
| &#128270;  | ClusteredIndex | ON credit\_hold\_reason|
| &#128270;  | ClusteredIndex | ON credit\_limit|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON corp\_cust|
| &#128270;  | ClusteredIndex | ON corp\_cred|
| &#128270;  | ClusteredIndex | ON corp\_address|
| &#128270;  | ClusteredIndex | ON amt\_over\_inv\_amt|
| &#128270;  | ClusteredIndex | ON days\_over\_inv\_due\_date|
| &#128270;  | ClusteredIndex | ON ship\_to\_email|
| &#128270;  | ClusteredIndex | ON bill\_to\_email|
| &#128270;  | ClusteredIndex | ON internet\_url|
| &#128270;  | ClusteredIndex | ON internal\_email\_addr|
| &#128270;  | ClusteredIndex | ON external\_email\_addr|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON carrier\_account|
| &#128270;  | ClusteredIndex | ON carrier\_upcharge\_pct|
| &#128270;  | ClusteredIndex | ON carrier\_residential\_indicator|
| &#128270;  | ClusteredIndex | ON carrier\_bill\_to\_transportation|
| &#128270;  | ClusteredIndex | ON order\_credit\_limit|
| &#128270;  | ClusteredIndex | ON use\_long\_name|
| &#128270;  | ClusteredIndex | ON long\_name|
| &#128270;  | ClusteredIndex | ON uf\_send\_automated\_pod|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.customer_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | cust\_seq| int  |
| &#128270; | contact\_1| varchar(8000)  |
| &#128270; | contact\_2| varchar(8000)  |
| &#128270; | contact\_3| varchar(8000)  |
| &#128270; | phone\_1| varchar(8000)  |
| &#128270; | phone\_2| varchar(8000)  |
| &#128270; | phone\_3| varchar(8000)  |
| &#128270; | cust\_type| varchar(8000)  |
| &#128270; | terms\_code| varchar(8000)  |
| &#128270; | ship\_code| varchar(8000)  |
| &#128270; | slsman| varchar(8000)  |
| &#128270; | state\_cycle| varchar(8000)  |
| &#128270; | fin\_chg| int  |
| &#128270; | last\_inv| datetime2(26)  |
| &#128270; | last\_paid| datetime2(26)  |
| &#128270; | sales\_ytd| decimal(23,8)  |
| &#128270; | sales\_lst\_yr| decimal(23,8)  |
| &#128270; | disc\_ytd| decimal(23,8)  |
| &#128270; | disc\_lst\_yr| decimal(23,8)  |
| &#128270; | last\_fin\_chg| datetime2(26)  |
| &#128270; | sales\_ptd| decimal(23,8)  |
| &#128270; | calc\_date| datetime2(26)  |
| &#128270; | num\_periods| int  |
| &#128270; | avg\_days\_os| int  |
| &#128270; | num\_invoices| int  |
| &#128270; | hist\_days\_os| int  |
| &#128270; | larg\_days\_os| int  |
| &#128270; | last\_days\_os| int  |
| &#128270; | avg\_bal\_os| decimal(23,8)  |
| &#128270; | large\_bal\_os| decimal(23,8)  |
| &#128270; | last\_bal\_os| decimal(23,8)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | charfld1| varchar(8000)  |
| &#128270; | charfld2| varchar(8000)  |
| &#128270; | charfld3| varchar(8000)  |
| &#128270; | decifld1| decimal(10,2)  |
| &#128270; | decifld2| decimal(10,2)  |
| &#128270; | decifld3| decimal(10,2)  |
| &#128270; | logifld| int  |
| &#128270; | datefld| datetime2(26)  |
| &#128270; | tax\_reg\_num1| varchar(8000)  |
| &#128270; | bank\_code| varchar(8000)  |
| &#128270; | tax\_reg\_num2| varchar(8000)  |
| &#128270; | pay\_type| varchar(8000)  |
| &#128270; | edi\_cust| int  |
| &#128270; | branch\_id| varchar(8000)  |
| &#128270; | trans\_nat| varchar(8000)  |
| &#128270; | delterm| varchar(8000)  |
| &#128270; | process\_ind| varchar(8000)  |
| &#128270; | use\_exch\_rate| int  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | pricecode| varchar(8000)  |
| &#128270; | ship\_early| int  |
| &#128270; | ship\_partial| int  |
| &#128270; | lang\_code| varchar(8000)  |
| &#128270; | end\_user\_type| varchar(8000)  |
| &#128270; | ship\_site| varchar(8000)  |
| &#128270; | lcr\_reqd| int  |
| &#128270; | cust\_bank| varchar(8000)  |
| &#128270; | draft\_print\_flag| int  |
| &#128270; | rcv\_internal\_email| int  |
| &#128270; | customer\_email\_addr| varchar(8000)  |
| &#128270; | send\_customer\_email| int  |
| &#128270; | aps\_pull\_up| int  |
| &#128270; | do\_invoice| varchar(8000)  |
| &#128270; | consolidate| int  |
| &#128270; | inv\_freq| varchar(8000)  |
| &#128270; | summarize| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | einvoice| int  |
| &#128270; | order\_bal| decimal(23,8)  |
| &#128270; | posted\_bal| decimal(23,8)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | crm\_guid| varchar(8000)  |
| &#128270; | in\_workflow| int  |
| &#128270; | print\_pack\_inv| int  |
| &#128270; | one\_pack\_inv| int  |
| &#128270; | inv\_category| varchar(8000)  |
| &#128270; | include\_tax\_in\_price| int  |
| &#128270; | trans\_nat\_2| varchar(8000)  |
| &#128270; | use\_revision\_pay\_days| int  |
| &#128270; | revision\_day| int  |
| &#128270; | revision\_day\_start\_time\_1| datetime2(26)  |
| &#128270; | revision\_day\_start\_time\_2| datetime2(26)  |
| &#128270; | revision\_day\_end\_time\_1| datetime2(26)  |
| &#128270; | revision\_day\_end\_time\_2| datetime2(26)  |
| &#128270; | pay\_day| int  |
| &#128270; | pay\_day\_start\_time\_1| datetime2(26)  |
| &#128270; | pay\_day\_start\_time\_2| datetime2(26)  |
| &#128270; | pay\_day\_end\_time\_1| datetime2(26)  |
| &#128270; | pay\_day\_end\_time\_2| datetime2(26)  |
| &#128270; | export\_type| varchar(8000)  |
| &#128270; | active\_for\_data\_integration| int  |
| &#128270; | show\_in\_ship\_to\_drop\_down\_list| int  |
| &#128270; | show\_in\_drop\_down\_list| int  |
| &#128270; | sic\_code| varchar(8000)  |
| &#128270; | number\_of\_employees| int  |
| &#128270; | company\_revenue| decimal(23,8)  |
| &#128270; | territory\_code| varchar(8000)  |
| &#128270; | sales\_team\_id| varchar(8000)  |
| &#128270; | days\_shipped\_before\_due\_date\_tolerance| int  |
| &#128270; | days\_shipped\_after\_due\_date\_tolerance| int  |
| &#128270; | shipped\_over\_ordered\_qty\_tolerance| decimal(7,4)  |
| &#128270; | shipped\_under\_ordered\_qty\_tolerance| decimal(7,4)  |
| &#128270; | default\_ship\_to| int  |
| &#128270; | reseller\_slsman| varchar(8000)  |
| &#128270; | shipment\_approval\_required| int  |
| &#128270; | ship\_hold| int  |
| &#128270; | ship\_method\_group| varchar(8000)  |
| &#128270; | jp\_consumption\_tax\_round\_method| varchar(8000)  |
| &#128270; | jp\_consumption\_tax\_header\_line\_method| varchar(8000)  |
| &#128270; | vrtx\_geocode| varchar(8000)  |
| &#128270; | include\_orders\_in\_tax\_rpt| int  |
| &#128270; | constructive\_sale\_price\_pct| decimal(5,2)  |
| &#128270; | tax\_reg\_num1\_exp\_date| datetime2(26)  |
| &#128270; | inv\_batch\_cutoff\_day| int  |
| &#128270; | bank\_acct\_no| varchar(8000)  |
| &#128270; | international\_bank\_account| varchar(8000)  |
| &#128270; | account\_name| varchar(8000)  |
| &#128270; | picture| varbinary(8000)  |
| &#128270; | sepa\_mandate\_ref| varchar(8000)  |
| &#128270; | sepa\_mandate\_creation\_date| datetime2(26)  |
| &#128270; | sepa\_mandate\_expiration\_date| datetime2(26)  |
| &#128270; | sepa\_mandate\_last\_used\_date| datetime2(26)  |
| &#128270; | sepa\_core\_direct\_debit| int  |
| &#128270; | sepa\_one\_off\_mandate| int  |
| &#128270; | catalog\_id| varchar(8000)  |
| &#128270; | au\_contract\_price\_method| varchar(8000)  |
| &#128270; | au\_price\_by| varchar(8000)  |
| &#128270; | bank\_authority\_party\_id| varchar(8000)  |
| &#128270; | dunning\_group| varchar(8000)  |
| &#128270; | last\_dunning\_date| datetime2(26)  |
| &#128270; | dunning\_stage| int  |
| &#128270; | one\_inv\_per\_shipment\_per\_order| int  |
| &#128270; | cn\_long\_bank\_acct\_no| varchar(8000)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | external\_entity| varchar(8000)  |
| &#128270; | prospect\_id| varchar(8000)  |
| &#128270; | head\_office| int  |
| &#128270; | branch\_name| varchar(8000)  |
| &#128270; | cust\_serial\_format\_code| varchar(8000)  |
| &#128270; | active\_for\_anonymization| int  |
| &#128270; | cust\_lot\_format\_code| varchar(8000)  |
| &#128270; | uf\_send\_automated\_pod| int  |
| &#128270; | uf\_branch| varchar(8000)  |
| &#128270; | uf\_cash| int  |
| &#128270; | uf\_co\_reg| varchar(8000)  |
| &#128270; | uf\_cpd\_anti\_bacterial| int  |
| &#128270; | uf\_cpd\_architectural\_metalwork| int  |
| &#128270; | uf\_cpd\_chilled\_beams\_isms| int  |
| &#128270; | uf\_cpd\_chilled\_ceilings| int  |
| &#128270; | uf\_cpd\_factory\_tour| int  |
| &#128270; | uf\_cpd\_metal\_ceilings| int  |
| &#128270; | uf\_cpd\_partitioning| int  |
| &#128270; | uf\_credit\_rating| varchar(8000)  |
| &#128270; | uf\_credit\_check| int  |
| &#128270; | uf\_credit\_source| varchar(8000)  |
| &#128270; | uf\_cust\_num\_prim| varchar(8000)  |
| &#128270; | uf\_customer\_acct\_type| varchar(8000)  |
| &#128270; | uf\_eff\_date\_cr\_limit| datetime2(26)  |
| &#128270; | uf\_eori\_no| varchar(8000)  |
| &#128270; | uf\_exclude| int  |
| &#128270; | uf\_expiry\_date| datetime2(26)  |
| &#128270; | uf\_ex\_std\_report| varchar(8000)  |
| &#128270; | uf\_on\_stop| int  |
| &#128270; | uf\_on\_stop\_order| int  |
| &#128270; | uf\_sas\_credit\_limit| decimal(21,8)  |
| &#128270; | uf\_sector| varchar(8000)  |
| &#128270; | uf\_ship\_to\_phone\_3| varchar(8000)  |
| &#128270; | uf\_ship\_to\_prj\_mgr| varchar(8000)  |
| &#128270; | uf\_taken\_by| varchar(8000)  |
| &#128270; | uf\_uk\_region| varchar(8000)  |
| &#128270; | uf\_user| varchar(8000)  |
| &#128270; | uf\_web| int  |
| &#128270; | uf\_salesforce\_id| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON cust\_seq|
| &#128270;  | ClusteredIndex | ON contact\_1|
| &#128270;  | ClusteredIndex | ON contact\_2|
| &#128270;  | ClusteredIndex | ON contact\_3|
| &#128270;  | ClusteredIndex | ON phone\_1|
| &#128270;  | ClusteredIndex | ON phone\_2|
| &#128270;  | ClusteredIndex | ON phone\_3|
| &#128270;  | ClusteredIndex | ON cust\_type|
| &#128270;  | ClusteredIndex | ON terms\_code|
| &#128270;  | ClusteredIndex | ON ship\_code|
| &#128270;  | ClusteredIndex | ON slsman|
| &#128270;  | ClusteredIndex | ON state\_cycle|
| &#128270;  | ClusteredIndex | ON fin\_chg|
| &#128270;  | ClusteredIndex | ON last\_inv|
| &#128270;  | ClusteredIndex | ON last\_paid|
| &#128270;  | ClusteredIndex | ON sales\_ytd|
| &#128270;  | ClusteredIndex | ON sales\_lst\_yr|
| &#128270;  | ClusteredIndex | ON disc\_ytd|
| &#128270;  | ClusteredIndex | ON disc\_lst\_yr|
| &#128270;  | ClusteredIndex | ON last\_fin\_chg|
| &#128270;  | ClusteredIndex | ON sales\_ptd|
| &#128270;  | ClusteredIndex | ON calc\_date|
| &#128270;  | ClusteredIndex | ON num\_periods|
| &#128270;  | ClusteredIndex | ON avg\_days\_os|
| &#128270;  | ClusteredIndex | ON num\_invoices|
| &#128270;  | ClusteredIndex | ON hist\_days\_os|
| &#128270;  | ClusteredIndex | ON larg\_days\_os|
| &#128270;  | ClusteredIndex | ON last\_days\_os|
| &#128270;  | ClusteredIndex | ON avg\_bal\_os|
| &#128270;  | ClusteredIndex | ON large\_bal\_os|
| &#128270;  | ClusteredIndex | ON last\_bal\_os|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON charfld1|
| &#128270;  | ClusteredIndex | ON charfld2|
| &#128270;  | ClusteredIndex | ON charfld3|
| &#128270;  | ClusteredIndex | ON decifld1|
| &#128270;  | ClusteredIndex | ON decifld2|
| &#128270;  | ClusteredIndex | ON decifld3|
| &#128270;  | ClusteredIndex | ON logifld|
| &#128270;  | ClusteredIndex | ON datefld|
| &#128270;  | ClusteredIndex | ON tax\_reg\_num1|
| &#128270;  | ClusteredIndex | ON bank\_code|
| &#128270;  | ClusteredIndex | ON tax\_reg\_num2|
| &#128270;  | ClusteredIndex | ON pay\_type|
| &#128270;  | ClusteredIndex | ON edi\_cust|
| &#128270;  | ClusteredIndex | ON branch\_id|
| &#128270;  | ClusteredIndex | ON trans\_nat|
| &#128270;  | ClusteredIndex | ON delterm|
| &#128270;  | ClusteredIndex | ON process\_ind|
| &#128270;  | ClusteredIndex | ON use\_exch\_rate|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON pricecode|
| &#128270;  | ClusteredIndex | ON ship\_early|
| &#128270;  | ClusteredIndex | ON ship\_partial|
| &#128270;  | ClusteredIndex | ON lang\_code|
| &#128270;  | ClusteredIndex | ON end\_user\_type|
| &#128270;  | ClusteredIndex | ON ship\_site|
| &#128270;  | ClusteredIndex | ON lcr\_reqd|
| &#128270;  | ClusteredIndex | ON cust\_bank|
| &#128270;  | ClusteredIndex | ON draft\_print\_flag|
| &#128270;  | ClusteredIndex | ON rcv\_internal\_email|
| &#128270;  | ClusteredIndex | ON customer\_email\_addr|
| &#128270;  | ClusteredIndex | ON send\_customer\_email|
| &#128270;  | ClusteredIndex | ON aps\_pull\_up|
| &#128270;  | ClusteredIndex | ON do\_invoice|
| &#128270;  | ClusteredIndex | ON consolidate|
| &#128270;  | ClusteredIndex | ON inv\_freq|
| &#128270;  | ClusteredIndex | ON summarize|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON einvoice|
| &#128270;  | ClusteredIndex | ON order\_bal|
| &#128270;  | ClusteredIndex | ON posted\_bal|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON crm\_guid|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON print\_pack\_inv|
| &#128270;  | ClusteredIndex | ON one\_pack\_inv|
| &#128270;  | ClusteredIndex | ON inv\_category|
| &#128270;  | ClusteredIndex | ON include\_tax\_in\_price|
| &#128270;  | ClusteredIndex | ON trans\_nat\_2|
| &#128270;  | ClusteredIndex | ON use\_revision\_pay\_days|
| &#128270;  | ClusteredIndex | ON revision\_day|
| &#128270;  | ClusteredIndex | ON revision\_day\_start\_time\_1|
| &#128270;  | ClusteredIndex | ON revision\_day\_start\_time\_2|
| &#128270;  | ClusteredIndex | ON revision\_day\_end\_time\_1|
| &#128270;  | ClusteredIndex | ON revision\_day\_end\_time\_2|
| &#128270;  | ClusteredIndex | ON pay\_day|
| &#128270;  | ClusteredIndex | ON pay\_day\_start\_time\_1|
| &#128270;  | ClusteredIndex | ON pay\_day\_start\_time\_2|
| &#128270;  | ClusteredIndex | ON pay\_day\_end\_time\_1|
| &#128270;  | ClusteredIndex | ON pay\_day\_end\_time\_2|
| &#128270;  | ClusteredIndex | ON export\_type|
| &#128270;  | ClusteredIndex | ON active\_for\_data\_integration|
| &#128270;  | ClusteredIndex | ON show\_in\_ship\_to\_drop\_down\_list|
| &#128270;  | ClusteredIndex | ON show\_in\_drop\_down\_list|
| &#128270;  | ClusteredIndex | ON sic\_code|
| &#128270;  | ClusteredIndex | ON number\_of\_employees|
| &#128270;  | ClusteredIndex | ON company\_revenue|
| &#128270;  | ClusteredIndex | ON territory\_code|
| &#128270;  | ClusteredIndex | ON sales\_team\_id|
| &#128270;  | ClusteredIndex | ON days\_shipped\_before\_due\_date\_tolerance|
| &#128270;  | ClusteredIndex | ON days\_shipped\_after\_due\_date\_tolerance|
| &#128270;  | ClusteredIndex | ON shipped\_over\_ordered\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON shipped\_under\_ordered\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON default\_ship\_to|
| &#128270;  | ClusteredIndex | ON reseller\_slsman|
| &#128270;  | ClusteredIndex | ON shipment\_approval\_required|
| &#128270;  | ClusteredIndex | ON ship\_hold|
| &#128270;  | ClusteredIndex | ON ship\_method\_group|
| &#128270;  | ClusteredIndex | ON jp\_consumption\_tax\_round\_method|
| &#128270;  | ClusteredIndex | ON jp\_consumption\_tax\_header\_line\_method|
| &#128270;  | ClusteredIndex | ON vrtx\_geocode|
| &#128270;  | ClusteredIndex | ON include\_orders\_in\_tax\_rpt|
| &#128270;  | ClusteredIndex | ON constructive\_sale\_price\_pct|
| &#128270;  | ClusteredIndex | ON tax\_reg\_num1\_exp\_date|
| &#128270;  | ClusteredIndex | ON inv\_batch\_cutoff\_day|
| &#128270;  | ClusteredIndex | ON bank\_acct\_no|
| &#128270;  | ClusteredIndex | ON international\_bank\_account|
| &#128270;  | ClusteredIndex | ON account\_name|
| &#128270;  | ClusteredIndex | ON picture|
| &#128270;  | ClusteredIndex | ON sepa\_mandate\_ref|
| &#128270;  | ClusteredIndex | ON sepa\_mandate\_creation\_date|
| &#128270;  | ClusteredIndex | ON sepa\_mandate\_expiration\_date|
| &#128270;  | ClusteredIndex | ON sepa\_mandate\_last\_used\_date|
| &#128270;  | ClusteredIndex | ON sepa\_core\_direct\_debit|
| &#128270;  | ClusteredIndex | ON sepa\_one\_off\_mandate|
| &#128270;  | ClusteredIndex | ON catalog\_id|
| &#128270;  | ClusteredIndex | ON au\_contract\_price\_method|
| &#128270;  | ClusteredIndex | ON au\_price\_by|
| &#128270;  | ClusteredIndex | ON bank\_authority\_party\_id|
| &#128270;  | ClusteredIndex | ON dunning\_group|
| &#128270;  | ClusteredIndex | ON last\_dunning\_date|
| &#128270;  | ClusteredIndex | ON dunning\_stage|
| &#128270;  | ClusteredIndex | ON one\_inv\_per\_shipment\_per\_order|
| &#128270;  | ClusteredIndex | ON cn\_long\_bank\_acct\_no|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON external\_entity|
| &#128270;  | ClusteredIndex | ON prospect\_id|
| &#128270;  | ClusteredIndex | ON head\_office|
| &#128270;  | ClusteredIndex | ON branch\_name|
| &#128270;  | ClusteredIndex | ON cust\_serial\_format\_code|
| &#128270;  | ClusteredIndex | ON active\_for\_anonymization|
| &#128270;  | ClusteredIndex | ON cust\_lot\_format\_code|
| &#128270;  | ClusteredIndex | ON uf\_send\_automated\_pod|
| &#128270;  | ClusteredIndex | ON uf\_branch|
| &#128270;  | ClusteredIndex | ON uf\_cash|
| &#128270;  | ClusteredIndex | ON uf\_co\_reg|
| &#128270;  | ClusteredIndex | ON uf\_cpd\_anti\_bacterial|
| &#128270;  | ClusteredIndex | ON uf\_cpd\_architectural\_metalwork|
| &#128270;  | ClusteredIndex | ON uf\_cpd\_chilled\_beams\_isms|
| &#128270;  | ClusteredIndex | ON uf\_cpd\_chilled\_ceilings|
| &#128270;  | ClusteredIndex | ON uf\_cpd\_factory\_tour|
| &#128270;  | ClusteredIndex | ON uf\_cpd\_metal\_ceilings|
| &#128270;  | ClusteredIndex | ON uf\_cpd\_partitioning|
| &#128270;  | ClusteredIndex | ON uf\_credit\_rating|
| &#128270;  | ClusteredIndex | ON uf\_credit\_check|
| &#128270;  | ClusteredIndex | ON uf\_credit\_source|
| &#128270;  | ClusteredIndex | ON uf\_cust\_num\_prim|
| &#128270;  | ClusteredIndex | ON uf\_customer\_acct\_type|
| &#128270;  | ClusteredIndex | ON uf\_eff\_date\_cr\_limit|
| &#128270;  | ClusteredIndex | ON uf\_eori\_no|
| &#128270;  | ClusteredIndex | ON uf\_exclude|
| &#128270;  | ClusteredIndex | ON uf\_expiry\_date|
| &#128270;  | ClusteredIndex | ON uf\_ex\_std\_report|
| &#128270;  | ClusteredIndex | ON uf\_on\_stop|
| &#128270;  | ClusteredIndex | ON uf\_on\_stop\_order|
| &#128270;  | ClusteredIndex | ON uf\_sas\_credit\_limit|
| &#128270;  | ClusteredIndex | ON uf\_sector|
| &#128270;  | ClusteredIndex | ON uf\_ship\_to\_phone\_3|
| &#128270;  | ClusteredIndex | ON uf\_ship\_to\_prj\_mgr|
| &#128270;  | ClusteredIndex | ON uf\_taken\_by|
| &#128270;  | ClusteredIndex | ON uf\_uk\_region|
| &#128270;  | ClusteredIndex | ON uf\_user|
| &#128270;  | ClusteredIndex | ON uf\_web|
| &#128270;  | ClusteredIndex | ON uf\_salesforce\_id|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table metadata.dataset_config 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | dataset\_id| bigint identity  |
| * &#128270; | dataset\_name| varchar(128)  |
| * &#128270; | is\_active| bit  |
| * &#128270; | execution\_order| int  |
| * &#128270; | load\_mode| varchar(20)  |
| * &#128270; | source\_lakehouse| varchar(128)  |
| * &#128270; | source\_schema| varchar(128)  |
| * &#128270; | source\_table| varchar(128)  |
| * &#128270; | staging\_schema| varchar(128)  |
| * &#128270; | staging\_table| varchar(128)  |
| &#128270; | staging\_inbound\_table| varchar(128)  |
| &#128270; | watermark\_column| varchar(128)  |
| &#128270; | initial\_watermark| datetime2(26)  |
| &#128270; | merge\_keys| varchar(400)  |
| * &#128270; | created\_at| datetime2(26)  |
| * &#128270; | updated\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_dataset\_config | ON dataset\_id|
| &#128270;  | ClusteredIndex | ON dataset\_name|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON execution\_order|
| &#128270;  | ClusteredIndex | ON load\_mode|
| &#128270;  | ClusteredIndex | ON source\_lakehouse|
| &#128270;  | ClusteredIndex | ON source\_schema|
| &#128270;  | ClusteredIndex | ON source\_table|
| &#128270;  | ClusteredIndex | ON staging\_schema|
| &#128270;  | ClusteredIndex | ON staging\_table|
| &#128270;  | ClusteredIndex | ON staging\_inbound\_table|
| &#128270;  | ClusteredIndex | ON watermark\_column|
| &#128270;  | ClusteredIndex | ON initial\_watermark|
| &#128270;  | ClusteredIndex | ON merge\_keys|
| &#128270;  | ClusteredIndex | ON created\_at|
| &#128270;  | ClusteredIndex | ON updated\_at|



### Table staging.dataset_config_import 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | batch\_id| varchar(36)  |
| * &#128270; | source\_row\_number| varchar(20)  |
| &#128270; | dataset\_name| varchar(400)  |
| &#128270; | is\_active| varchar(10)  |
| &#128270; | execution\_order| varchar(20)  |
| &#128270; | load\_mode| varchar(50)  |
| &#128270; | source\_lakehouse| varchar(400)  |
| &#128270; | source\_schema| varchar(400)  |
| &#128270; | source\_table| varchar(400)  |
| &#128270; | staging\_schema| varchar(400)  |
| &#128270; | staging\_table| varchar(400)  |
| &#128270; | watermark\_column| varchar(400)  |
| &#128270; | initial\_watermark| varchar(50)  |
| &#128270; | merge\_keys| varchar(400)  |
| * &#128270; | loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON batch\_id|
| &#128270;  | ClusteredIndex | ON source\_row\_number|
| &#128270;  | ClusteredIndex | ON dataset\_name|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON execution\_order|
| &#128270;  | ClusteredIndex | ON load\_mode|
| &#128270;  | ClusteredIndex | ON source\_lakehouse|
| &#128270;  | ClusteredIndex | ON source\_schema|
| &#128270;  | ClusteredIndex | ON source\_table|
| &#128270;  | ClusteredIndex | ON staging\_schema|
| &#128270;  | ClusteredIndex | ON staging\_table|
| &#128270;  | ClusteredIndex | ON watermark\_column|
| &#128270;  | ClusteredIndex | ON initial\_watermark|
| &#128270;  | ClusteredIndex | ON merge\_keys|
| &#128270;  | ClusteredIndex | ON loaded\_at|



### Table metadata.dataset_execution 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | execution\_id| bigint identity  |
| * &#128270; | run\_id| bigint  |
| * &#128270; | dataset\_id| bigint  |
| * &#128270; | dataset\_name| varchar(128)  |
| * &#128270; | load\_mode| varchar(20)  |
| &#128270; | data\_from\_timestamp| datetime2(26)  |
| &#128270; | data\_to\_timestamp| datetime2(26)  |
| * &#128270; | status| varchar(30)  |
| &#128270; | row\_count| bigint  |
| * &#128270; | start\_time| datetime2(26)  |
| &#128270; | end\_time| datetime2(26)  |
| &#128270; | error\_number| int  |
| &#128270; | error\_message| varchar(4000)  |
| * &#128270; | created\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_dataset\_execution | ON execution\_id|
| &#128270;  | ClusteredIndex | ON run\_id|
| &#128270;  | ClusteredIndex | ON dataset\_id|
| &#128270;  | ClusteredIndex | ON dataset\_name|
| &#128270;  | ClusteredIndex | ON load\_mode|
| &#128270;  | ClusteredIndex | ON data\_from\_timestamp|
| &#128270;  | ClusteredIndex | ON data\_to\_timestamp|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON row\_count|
| &#128270;  | ClusteredIndex | ON start\_time|
| &#128270;  | ClusteredIndex | ON end\_time|
| &#128270;  | ClusteredIndex | ON error\_number|
| &#128270;  | ClusteredIndex | ON error\_message|
| &#128270;  | ClusteredIndex | ON created\_at|



### Table metadata.dataset_watermark 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | dataset\_id| bigint  |
| &#128270; | last\_successful\_watermark| datetime2(26)  |
| &#128270; | last\_successful\_run\_id| bigint  |
| * &#128270; | updated\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_dataset\_watermark | ON dataset\_id|
| &#128270;  | ClusteredIndex | ON last\_successful\_watermark|
| &#128270;  | ClusteredIndex | ON last\_successful\_run\_id|
| &#128270;  | ClusteredIndex | ON updated\_at|



### Table elt.dim_date 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | date\_key| int  |
| &#128270; | calendar\_date| date  |
| &#128270; | day\_of\_week| int  |
| &#128270; | day\_name| varchar(8000)  |
| &#128270; | is\_weekday| bit  |
| &#128270; | customer\_week\_no| int  |
| &#128270; | customer\_year| int  |
| &#128270; | customer\_period| int  |
| &#128270; | week\_start\_date| date  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON calendar\_date|
| &#128270;  | ClusteredIndex | ON day\_of\_week|
| &#128270;  | ClusteredIndex | ON day\_name|
| &#128270;  | ClusteredIndex | ON is\_weekday|
| &#128270;  | ClusteredIndex | ON customer\_week\_no|
| &#128270;  | ClusteredIndex | ON customer\_year|
| &#128270;  | ClusteredIndex | ON customer\_period|
| &#128270;  | ClusteredIndex | ON week\_start\_date|



### Table reporting.dim_date 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | date\_key| int  |
| * &#128270; | calendar\_date| datetime2(26)  |
| * &#128270; | day\_of\_week| int  |
| * &#128270; | day\_name| varchar(20)  |
| * &#128270; | is\_weekday| bit  |
| * &#128270; | customer\_week\_no| int  |
| * &#128270; | customer\_year| int  |
| * &#128270; | customer\_period| int  |
| * &#128270; | calendar\_quarter| int  |
| * &#128270; | calendar\_quarter\_name| varchar(2)  |
| * &#128270; | week\_start\_date| datetime2(26)  |
| * &#128270; | week\_end\_date| datetime2(26)  |
| * &#128270; | week\_key| int  |
| * &#128270; | created\_ts| datetime2(26)  |
| * &#128270; | updated\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON calendar\_date|
| &#128270;  | ClusteredIndex | ON day\_of\_week|
| &#128270;  | ClusteredIndex | ON day\_name|
| &#128270;  | ClusteredIndex | ON is\_weekday|
| &#128270;  | ClusteredIndex | ON customer\_week\_no|
| &#128270;  | ClusteredIndex | ON customer\_year|
| &#128270;  | ClusteredIndex | ON customer\_period|
| &#128270;  | ClusteredIndex | ON calendar\_quarter|
| &#128270;  | ClusteredIndex | ON calendar\_quarter\_name|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_end\_date|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON created\_ts|
| &#128270;  | ClusteredIndex | ON updated\_ts|



### Table salesforce.dim_kpi 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | kpi\_id| bigint  |
| * &#128270; | kpi\_code| varchar(50)  |
| * &#128270; | category| varchar(50)  |
| * &#128270; | kpi\_name| varchar(100)  |
| &#128270; | description| varchar(500)  |
| * &#128270; | uom| varchar(50)  |
| * &#128270; | breach\_direction| varchar(10)  |
| &#128270; | target\_value| decimal(18,4)  |
| &#128270; | rag\_threshold\_low| decimal(18,4)  |
| &#128270; | rag\_threshold\_high| decimal(18,4)  |
| * &#128270; | is\_active| bit  |
| * &#128270; | created\_utc| datetime2(26)  |
| * &#128270; | updated\_utc| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON category|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON rag\_threshold\_low|
| &#128270;  | ClusteredIndex | ON rag\_threshold\_high|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON created\_utc|
| &#128270;  | ClusteredIndex | ON updated\_utc|



### Table salesforce.dim_record_type 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | record\_type\_key| bigint  |
| * &#128270; | record\_type\_id| varchar(18)  |
| &#128270; | record\_type\_name| varchar(255)  |
| &#128270; | developer\_name| varchar(255)  |
| &#128270; | subject\_type| varchar(255)  |
| * &#128270; | is\_active| bit  |
| &#128270; | description| varchar(1000)  |
| * &#128270; | created\_ts| datetime2(26)  |
| * &#128270; | updated\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON record\_type\_key|
| &#128270;  | ClusteredIndex | ON record\_type\_id|
| &#128270;  | ClusteredIndex | ON record\_type\_name|
| &#128270;  | ClusteredIndex | ON developer\_name|
| &#128270;  | ClusteredIndex | ON subject\_type|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON created\_ts|
| &#128270;  | ClusteredIndex | ON updated\_ts|



### Table salesforce_staging.estimate 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | project\_name| varchar(8000)  |
| &#128270; | account| varchar(8000)  |
| &#128270; | budget| bit  |
| &#128270; | complexity| varchar(8000)  |
| &#128270; | contact| varchar(8000)  |
| &#128270; | estimate\_number| varchar(8000)  |
| &#128270; | estimator| varchar(8000)  |
| &#128270; | exchange\_rate| decimal(38,18)  |
| &#128270; | figures| bit  |
| &#128270; | non\_project| bit  |
| &#128270; | primary| bit  |
| &#128270; | lost\_reason| varchar(8000)  |
| &#128270; | quote\_date| datetime2(26)  |
| &#128270; | quote\_sqm| decimal(38,18)  |
| &#128270; | quote\_status| varchar(8000)  |
| &#128270; | quoted\_value\_database\_currency| varchar(8000)  |
| &#128270; | customer\_quote| varchar(8000)  |
| &#128270; | quoted\_value\_transfer\_price\_layout| varchar(8000)  |
| &#128270; | quoted\_value\_database\_currency\_del| decimal(38,18)  |
| &#128270; | quoted\_value\_quoted\_currency| decimal(38,18)  |
| &#128270; | quoted\_value\_transfer\_price| decimal(38,18)  |
| &#128270; | rev| varchar(8000)  |
| &#128270; | site\_reference| varchar(8000)  |
| &#128270; | database\_currency| varchar(8000)  |
| &#128270; | spa\_agreed| bit  |
| &#128270; | order\_by| datetime2(26)  |
| &#128270; | deliver\_by| datetime2(26)  |
| &#128270; | discount\_type| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | dependencies| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON account|
| &#128270;  | ClusteredIndex | ON budget|
| &#128270;  | ClusteredIndex | ON complexity|
| &#128270;  | ClusteredIndex | ON contact|
| &#128270;  | ClusteredIndex | ON estimate\_number|
| &#128270;  | ClusteredIndex | ON estimator|
| &#128270;  | ClusteredIndex | ON exchange\_rate|
| &#128270;  | ClusteredIndex | ON figures|
| &#128270;  | ClusteredIndex | ON non\_project|
| &#128270;  | ClusteredIndex | ON primary|
| &#128270;  | ClusteredIndex | ON lost\_reason|
| &#128270;  | ClusteredIndex | ON quote\_date|
| &#128270;  | ClusteredIndex | ON quote\_sqm|
| &#128270;  | ClusteredIndex | ON quote\_status|
| &#128270;  | ClusteredIndex | ON quoted\_value\_database\_currency|
| &#128270;  | ClusteredIndex | ON customer\_quote|
| &#128270;  | ClusteredIndex | ON quoted\_value\_transfer\_price\_layout|
| &#128270;  | ClusteredIndex | ON quoted\_value\_database\_currency\_del|
| &#128270;  | ClusteredIndex | ON quoted\_value\_quoted\_currency|
| &#128270;  | ClusteredIndex | ON quoted\_value\_transfer\_price|
| &#128270;  | ClusteredIndex | ON rev|
| &#128270;  | ClusteredIndex | ON site\_reference|
| &#128270;  | ClusteredIndex | ON database\_currency|
| &#128270;  | ClusteredIndex | ON spa\_agreed|
| &#128270;  | ClusteredIndex | ON order\_by|
| &#128270;  | ClusteredIndex | ON deliver\_by|
| &#128270;  | ClusteredIndex | ON discount\_type|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON dependencies|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.estimate_order_line 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | external\_id| varchar(8000)  |
| &#128270; | display\_url| varchar(8000)  |
| &#128270; | uf\_m2\_tot| decimal(38,18)  |
| &#128270; | uf\_additional\_description| varchar(8000)  |
| &#128270; | uf\_cust\_del\_date| datetime2(26)  |
| &#128270; | uf\_depth| decimal(38,18)  |
| &#128270; | uf\_gauge| varchar(8000)  |
| &#128270; | uf\_insulation\_type| varchar(8000)  |
| &#128270; | uf\_length| varchar(8000)  |
| &#128270; | uf\_long\_description| varchar(8000)  |
| &#128270; | uf\_m2| decimal(38,18)  |
| &#128270; | uf\_material\_type| varchar(8000)  |
| &#128270; | uf\_module\_length| varchar(8000)  |
| &#128270; | uf\_module\_width| varchar(8000)  |
| &#128270; | uf\_nominal\_border| varchar(8000)  |
| &#128270; | uf\_paint| varchar(8000)  |
| &#128270; | uf\_perf| varchar(8000)  |
| &#128270; | uf\_product\_type1| varchar(8000)  |
| &#128270; | uf\_sys\_type| varchar(8000)  |
| &#128270; | uf\_trn\_price| decimal(38,18)  |
| &#128270; | uf\_width| varchar(8000)  |
| &#128270; | co\_line| decimal(38,18)  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | item| varchar(8000)  |
| &#128270; | price| decimal(38,18)  |
| &#128270; | promise\_date| datetime2(26)  |
| &#128270; | qty\_invoiced| decimal(38,18)  |
| &#128270; | qty\_ordered| decimal(38,18)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | u\_m| varchar(8000)  |
| &#128270; | ship\_site| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON external\_id|
| &#128270;  | ClusteredIndex | ON display\_url|
| &#128270;  | ClusteredIndex | ON uf\_m2\_tot|
| &#128270;  | ClusteredIndex | ON uf\_additional\_description|
| &#128270;  | ClusteredIndex | ON uf\_cust\_del\_date|
| &#128270;  | ClusteredIndex | ON uf\_depth|
| &#128270;  | ClusteredIndex | ON uf\_gauge|
| &#128270;  | ClusteredIndex | ON uf\_insulation\_type|
| &#128270;  | ClusteredIndex | ON uf\_length|
| &#128270;  | ClusteredIndex | ON uf\_long\_description|
| &#128270;  | ClusteredIndex | ON uf\_m2|
| &#128270;  | ClusteredIndex | ON uf\_material\_type|
| &#128270;  | ClusteredIndex | ON uf\_module\_length|
| &#128270;  | ClusteredIndex | ON uf\_module\_width|
| &#128270;  | ClusteredIndex | ON uf\_nominal\_border|
| &#128270;  | ClusteredIndex | ON uf\_paint|
| &#128270;  | ClusteredIndex | ON uf\_perf|
| &#128270;  | ClusteredIndex | ON uf\_product\_type1|
| &#128270;  | ClusteredIndex | ON uf\_sys\_type|
| &#128270;  | ClusteredIndex | ON uf\_trn\_price|
| &#128270;  | ClusteredIndex | ON uf\_width|
| &#128270;  | ClusteredIndex | ON co\_line|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON price|
| &#128270;  | ClusteredIndex | ON promise\_date|
| &#128270;  | ClusteredIndex | ON qty\_invoiced|
| &#128270;  | ClusteredIndex | ON qty\_ordered|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON u\_m|
| &#128270;  | ClusteredIndex | ON ship\_site|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.estimating_request 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | owner\_id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | record\_type\_id| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | company\_name| varchar(8000)  |
| &#128270; | complete\_by\_date| datetime2(26)  |
| &#128270; | complexity| varchar(8000)  |
| &#128270; | contact\_email| varchar(8000)  |
| &#128270; | contact\_name| varchar(8000)  |
| &#128270; | copy\_quote\_required| varchar(8000)  |
| &#128270; | major\_project| bit  |
| &#128270; | requested\_return\_date| datetime2(26)  |
| &#128270; | estimate\_value| decimal(38,18)  |
| &#128270; | freight\_type| varchar(8000)  |
| &#128270; | infor\_estimate\_number| varchar(8000)  |
| &#128270; | infor\_reference\_number\_account| varchar(8000)  |
| &#128270; | infor\_reference\_number\_project| varchar(8000)  |
| &#128270; | lighting| bit  |
| &#128270; | opportunity\_review\_by| varchar(8000)  |
| &#128270; | opportunity\_review\_reason| varchar(8000)  |
| &#128270; | order\_date| datetime2(26)  |
| &#128270; | project\_country| varchar(8000)  |
| &#128270; | project\_name| varchar(8000)  |
| &#128270; | project\_owner| varchar(8000)  |
| &#128270; | project\_probability| varchar(8000)  |
| &#128270; | pre\_bcr\_required| bit  |
| &#128270; | project\_secondary\_owner| varchar(8000)  |
| &#128270; | project\_specification| varchar(8000)  |
| &#128270; | project\_stage| varchar(8000)  |
| &#128270; | project\_town| varchar(8000)  |
| &#128270; | quantity\_m2| decimal(38,18)  |
| &#128270; | quote\_type| varchar(8000)  |
| &#128270; | review\_date| datetime2(26)  |
| &#128270; | review| varchar(8000)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | sharepoint| varchar(8000)  |
| &#128270; | status| varchar(8000)  |
| &#128270; | take\_off\_required| bit  |
| &#128270; | project\_name2| varchar(8000)  |
| &#128270; | priority| varchar(8000)  |
| &#128270; | bcr\_estimated\_divisional\_margin| varchar(8000)  |
| &#128270; | bcr\_estimated\_through\_margin| varchar(8000)  |
| &#128270; | bcr\_notes\_for\_review\_meeting| varchar(8000)  |
| &#128270; | bcr\_sign\_off\_date| datetime2(26)  |
| &#128270; | bcr\_signed\_off| bit  |
| &#128270; | bcr\_value\_to\_be\_reviewed| varchar(8000)  |
| &#128270; | business\_commercial\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_3rd\_party\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_3rd\_party\_review| bit  |
| &#128270; | dfm\_finishes\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_finishes\_review| bit  |
| &#128270; | dfm\_manufacturing\_process\_notes| varchar(8000)  |
| &#128270; | dfm\_manufacturing\_process\_review| bit  |
| &#128270; | dfm\_materials\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_materials\_review| bit  |
| &#128270; | dfm\_required| bit  |
| &#128270; | dfm\_samples\_mock\_up\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_samples\_mock\_up\_review| bit  |
| &#128270; | dfm\_sign\_off\_date| datetime2(26)  |
| &#128270; | dfm\_signed\_off| bit  |
| &#128270; | dfm\_summary\_notes| varchar(8000)  |
| &#128270; | dfm\_tooling\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_tooling\_review| bit  |
| &#128270; | factory\_design\_notes| varchar(8000)  |
| &#128270; | factory\_notes\_advised| bit  |
| &#128270; | financial\_review\_notes| varchar(8000)  |
| &#128270; | financial\_review| bit  |
| &#128270; | last\_dfm\_request\_no\_dfm| varchar(8000)  |
| &#128270; | last\_estimate\_request\_no| varchar(8000)  |
| &#128270; | npi\_required| bit  |
| &#128270; | other\_considerations| bit  |
| &#128270; | previous\_bcr\_date| datetime2(26)  |
| &#128270; | previous\_bcr\_signed\_off| bit  |
| &#128270; | previous\_dfm\_date| datetime2(26)  |
| &#128270; | previous\_dfm\_signed\_off| bit  |
| &#128270; | project\_risk\_notes| varchar(8000)  |
| &#128270; | project\_risk| bit  |
| &#128270; | selling\_price\_review\_notes| varchar(8000)  |
| &#128270; | selling\_price\_review| bit  |
| &#128270; | specification\_drawing\_notes| varchar(8000)  |
| &#128270; | specification\_drawing\_review| bit  |
| &#128270; | bcr\_required| bit  |
| &#128270; | dfm\_signed\_off\_by| varchar(8000)  |
| &#128270; | design\_review| bit  |
| &#128270; | design\_review\_notes| varchar(8000)  |
| &#128270; | costing\_completion\_date| datetime2(26)  |
| &#128270; | estimating\_request| varchar(8000)  |
| &#128270; | status\_costing| varchar(8000)  |
| &#128270; | days\_taken\_to\_complete| decimal(38,18)  |
| &#128270; | copy\_quotes\_sent| bit  |
| &#128270; | subject| varchar(8000)  |
| &#128270; | tacca\_status| varchar(8000)  |
| &#128270; | area\_of\_improvement| varchar(8000)  |
| &#128270; | awaiting\_info\_reason| varchar(8000)  |
| &#128270; | closed| decimal(38,18)  |
| &#128270; | in\_progress| decimal(38,18)  |
| &#128270; | proposal\_issued| varchar(8000)  |
| &#128270; | proposal\_number| varchar(8000)  |
| &#128270; | overdue| varchar(8000)  |
| &#128270; | overdue\_colour| varchar(8000)  |
| &#128270; | margin| varchar(8000)  |
| &#128270; | total\_value| varchar(8000)  |
| &#128270; | awaiting\_info| decimal(38,18)  |
| &#128270; | awaiting\_quote| decimal(38,18)  |
| &#128270; | dfm| decimal(38,18)  |
| &#128270; | cleansed| decimal(38,18)  |
| &#128270; | open| decimal(38,18)  |
| &#128270; | drawings\_received| bit  |
| &#128270; | specification\_seen| bit  |
| &#128270; | take\_off\_received| bit  |
| &#128270; | sign\_off\_notes| varchar(8000)  |
| &#128270; | validated| bit  |
| &#128270; | validated\_user| varchar(8000)  |
| &#128270; | to\_approve| varchar(8000)  |
| &#128270; | potential\_1\_m| bit  |
| &#128270; | square\_meter\_rate\_per\_system| varchar(8000)  |
| &#128270; | take\_off| varchar(8000)  |
| &#128270; | investment\_machines\_tools| varchar(8000)  |
| &#128270; | special\_materials| varchar(8000)  |
| &#128270; | cost\_vs\_tp\_vs\_sell| varchar(8000)  |
| &#128270; | value\_of\_design| varchar(8000)  |
| &#128270; | value\_of\_carriage| varchar(8000)  |
| &#128270; | value\_of\_shop\_drawings| varchar(8000)  |
| &#128270; | date\_time\_closed| datetime2(26)  |
| &#128270; | date\_time\_opened| datetime2(26)  |
| &#128270; | horizon\_specification\_issued| bit  |
| &#128270; | change\_order| bit  |
| &#128270; | drawings\_available| bit  |
| &#128270; | boq\_available| bit  |
| &#128270; | construction\_stage| varchar(8000)  |
| &#128270; | order\_date\_percent| decimal(38,18)  |
| &#128270; | sector\_percentage| decimal(38,18)  |
| &#128270; | build\_type\_percentage| decimal(38,18)  |
| &#128270; | specification\_percentage| decimal(38,18)  |
| &#128270; | specification\_seen\_percentage| decimal(38,18)  |
| &#128270; | drawings\_percentage| decimal(38,18)  |
| &#128270; | boq\_available\_percentage| decimal(38,18)  |
| &#128270; | construction\_stage\_percentage| decimal(38,18)  |
| &#128270; | proposal\_percentage| decimal(38,18)  |
| &#128270; | concept\_image\_percentage| decimal(38,18)  |
| &#128270; | target\_price\_percentage| decimal(38,18)  |
| &#128270; | project\_sector| varchar(8000)  |
| &#128270; | project\_build\_type| varchar(8000)  |
| &#128270; | concept\_image| bit  |
| &#128270; | target\_price| decimal(38,18)  |
| &#128270; | total\_percentage| decimal(38,18)  |
| &#128270; | construction\_drawings| decimal(38,18)  |
| &#128270; | cleansed\_date| datetime2(26)  |
| &#128270; | date\_closed| datetime2(26)  |
| &#128270; | hours\_taken\_to\_close| decimal(38,18)  |
| &#128270; | project\_infor\_reference| varchar(8000)  |
| &#128270; | account\_infor\_reference| varchar(8000)  |
| &#128270; | project\_probability\_formula| varchar(8000)  |
| &#128270; | project\_stage\_formula| varchar(8000)  |
| &#128270; | construction\_stage\_formula| varchar(8000)  |
| &#128270; | order\_date\_formula| datetime2(26)  |
| &#128270; | opportunity\_review\_notes| varchar(8000)  |
| &#128270; | project\_region| varchar(8000)  |
| &#128270; | pre\_bcr\_risk\_notes| varchar(8000)  |
| &#128270; | opportunity\_review| bit  |
| &#128270; | opportunity\_review\_completed| bit  |
| &#128270; | date\_time\_into\_costing| datetime2(26)  |
| &#128270; | date\_time\_out\_costing| datetime2(26)  |
| &#128270; | project\_id| varchar(8000)  |
| &#128270; | days\_overdue| decimal(38,18)  |
| &#128270; | lines\_with\_no\_item\_tp| decimal(38,18)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON owner\_id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON record\_type\_id|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON company\_name|
| &#128270;  | ClusteredIndex | ON complete\_by\_date|
| &#128270;  | ClusteredIndex | ON complexity|
| &#128270;  | ClusteredIndex | ON contact\_email|
| &#128270;  | ClusteredIndex | ON contact\_name|
| &#128270;  | ClusteredIndex | ON copy\_quote\_required|
| &#128270;  | ClusteredIndex | ON major\_project|
| &#128270;  | ClusteredIndex | ON requested\_return\_date|
| &#128270;  | ClusteredIndex | ON estimate\_value|
| &#128270;  | ClusteredIndex | ON freight\_type|
| &#128270;  | ClusteredIndex | ON infor\_estimate\_number|
| &#128270;  | ClusteredIndex | ON infor\_reference\_number\_account|
| &#128270;  | ClusteredIndex | ON infor\_reference\_number\_project|
| &#128270;  | ClusteredIndex | ON lighting|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_by|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_reason|
| &#128270;  | ClusteredIndex | ON order\_date|
| &#128270;  | ClusteredIndex | ON project\_country|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON project\_owner|
| &#128270;  | ClusteredIndex | ON project\_probability|
| &#128270;  | ClusteredIndex | ON pre\_bcr\_required|
| &#128270;  | ClusteredIndex | ON project\_secondary\_owner|
| &#128270;  | ClusteredIndex | ON project\_specification|
| &#128270;  | ClusteredIndex | ON project\_stage|
| &#128270;  | ClusteredIndex | ON project\_town|
| &#128270;  | ClusteredIndex | ON quantity\_m2|
| &#128270;  | ClusteredIndex | ON quote\_type|
| &#128270;  | ClusteredIndex | ON review\_date|
| &#128270;  | ClusteredIndex | ON review|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON sharepoint|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON take\_off\_required|
| &#128270;  | ClusteredIndex | ON project\_name2|
| &#128270;  | ClusteredIndex | ON priority|
| &#128270;  | ClusteredIndex | ON bcr\_estimated\_divisional\_margin|
| &#128270;  | ClusteredIndex | ON bcr\_estimated\_through\_margin|
| &#128270;  | ClusteredIndex | ON bcr\_notes\_for\_review\_meeting|
| &#128270;  | ClusteredIndex | ON bcr\_sign\_off\_date|
| &#128270;  | ClusteredIndex | ON bcr\_signed\_off|
| &#128270;  | ClusteredIndex | ON bcr\_value\_to\_be\_reviewed|
| &#128270;  | ClusteredIndex | ON business\_commercial\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_3rd\_party\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_3rd\_party\_review|
| &#128270;  | ClusteredIndex | ON dfm\_finishes\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_finishes\_review|
| &#128270;  | ClusteredIndex | ON dfm\_manufacturing\_process\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_manufacturing\_process\_review|
| &#128270;  | ClusteredIndex | ON dfm\_materials\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_materials\_review|
| &#128270;  | ClusteredIndex | ON dfm\_required|
| &#128270;  | ClusteredIndex | ON dfm\_samples\_mock\_up\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_samples\_mock\_up\_review|
| &#128270;  | ClusteredIndex | ON dfm\_sign\_off\_date|
| &#128270;  | ClusteredIndex | ON dfm\_signed\_off|
| &#128270;  | ClusteredIndex | ON dfm\_summary\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_tooling\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_tooling\_review|
| &#128270;  | ClusteredIndex | ON factory\_design\_notes|
| &#128270;  | ClusteredIndex | ON factory\_notes\_advised|
| &#128270;  | ClusteredIndex | ON financial\_review\_notes|
| &#128270;  | ClusteredIndex | ON financial\_review|
| &#128270;  | ClusteredIndex | ON last\_dfm\_request\_no\_dfm|
| &#128270;  | ClusteredIndex | ON last\_estimate\_request\_no|
| &#128270;  | ClusteredIndex | ON npi\_required|
| &#128270;  | ClusteredIndex | ON other\_considerations|
| &#128270;  | ClusteredIndex | ON previous\_bcr\_date|
| &#128270;  | ClusteredIndex | ON previous\_bcr\_signed\_off|
| &#128270;  | ClusteredIndex | ON previous\_dfm\_date|
| &#128270;  | ClusteredIndex | ON previous\_dfm\_signed\_off|
| &#128270;  | ClusteredIndex | ON project\_risk\_notes|
| &#128270;  | ClusteredIndex | ON project\_risk|
| &#128270;  | ClusteredIndex | ON selling\_price\_review\_notes|
| &#128270;  | ClusteredIndex | ON selling\_price\_review|
| &#128270;  | ClusteredIndex | ON specification\_drawing\_notes|
| &#128270;  | ClusteredIndex | ON specification\_drawing\_review|
| &#128270;  | ClusteredIndex | ON bcr\_required|
| &#128270;  | ClusteredIndex | ON dfm\_signed\_off\_by|
| &#128270;  | ClusteredIndex | ON design\_review|
| &#128270;  | ClusteredIndex | ON design\_review\_notes|
| &#128270;  | ClusteredIndex | ON costing\_completion\_date|
| &#128270;  | ClusteredIndex | ON estimating\_request|
| &#128270;  | ClusteredIndex | ON status\_costing|
| &#128270;  | ClusteredIndex | ON days\_taken\_to\_complete|
| &#128270;  | ClusteredIndex | ON copy\_quotes\_sent|
| &#128270;  | ClusteredIndex | ON subject|
| &#128270;  | ClusteredIndex | ON tacca\_status|
| &#128270;  | ClusteredIndex | ON area\_of\_improvement|
| &#128270;  | ClusteredIndex | ON awaiting\_info\_reason|
| &#128270;  | ClusteredIndex | ON closed|
| &#128270;  | ClusteredIndex | ON in\_progress|
| &#128270;  | ClusteredIndex | ON proposal\_issued|
| &#128270;  | ClusteredIndex | ON proposal\_number|
| &#128270;  | ClusteredIndex | ON overdue|
| &#128270;  | ClusteredIndex | ON overdue\_colour|
| &#128270;  | ClusteredIndex | ON margin|
| &#128270;  | ClusteredIndex | ON total\_value|
| &#128270;  | ClusteredIndex | ON awaiting\_info|
| &#128270;  | ClusteredIndex | ON awaiting\_quote|
| &#128270;  | ClusteredIndex | ON dfm|
| &#128270;  | ClusteredIndex | ON cleansed|
| &#128270;  | ClusteredIndex | ON open|
| &#128270;  | ClusteredIndex | ON drawings\_received|
| &#128270;  | ClusteredIndex | ON specification\_seen|
| &#128270;  | ClusteredIndex | ON take\_off\_received|
| &#128270;  | ClusteredIndex | ON sign\_off\_notes|
| &#128270;  | ClusteredIndex | ON validated|
| &#128270;  | ClusteredIndex | ON validated\_user|
| &#128270;  | ClusteredIndex | ON to\_approve|
| &#128270;  | ClusteredIndex | ON potential\_1\_m|
| &#128270;  | ClusteredIndex | ON square\_meter\_rate\_per\_system|
| &#128270;  | ClusteredIndex | ON take\_off|
| &#128270;  | ClusteredIndex | ON investment\_machines\_tools|
| &#128270;  | ClusteredIndex | ON special\_materials|
| &#128270;  | ClusteredIndex | ON cost\_vs\_tp\_vs\_sell|
| &#128270;  | ClusteredIndex | ON value\_of\_design|
| &#128270;  | ClusteredIndex | ON value\_of\_carriage|
| &#128270;  | ClusteredIndex | ON value\_of\_shop\_drawings|
| &#128270;  | ClusteredIndex | ON date\_time\_closed|
| &#128270;  | ClusteredIndex | ON date\_time\_opened|
| &#128270;  | ClusteredIndex | ON horizon\_specification\_issued|
| &#128270;  | ClusteredIndex | ON change\_order|
| &#128270;  | ClusteredIndex | ON drawings\_available|
| &#128270;  | ClusteredIndex | ON boq\_available|
| &#128270;  | ClusteredIndex | ON construction\_stage|
| &#128270;  | ClusteredIndex | ON order\_date\_percent|
| &#128270;  | ClusteredIndex | ON sector\_percentage|
| &#128270;  | ClusteredIndex | ON build\_type\_percentage|
| &#128270;  | ClusteredIndex | ON specification\_percentage|
| &#128270;  | ClusteredIndex | ON specification\_seen\_percentage|
| &#128270;  | ClusteredIndex | ON drawings\_percentage|
| &#128270;  | ClusteredIndex | ON boq\_available\_percentage|
| &#128270;  | ClusteredIndex | ON construction\_stage\_percentage|
| &#128270;  | ClusteredIndex | ON proposal\_percentage|
| &#128270;  | ClusteredIndex | ON concept\_image\_percentage|
| &#128270;  | ClusteredIndex | ON target\_price\_percentage|
| &#128270;  | ClusteredIndex | ON project\_sector|
| &#128270;  | ClusteredIndex | ON project\_build\_type|
| &#128270;  | ClusteredIndex | ON concept\_image|
| &#128270;  | ClusteredIndex | ON target\_price|
| &#128270;  | ClusteredIndex | ON total\_percentage|
| &#128270;  | ClusteredIndex | ON construction\_drawings|
| &#128270;  | ClusteredIndex | ON cleansed\_date|
| &#128270;  | ClusteredIndex | ON date\_closed|
| &#128270;  | ClusteredIndex | ON hours\_taken\_to\_close|
| &#128270;  | ClusteredIndex | ON project\_infor\_reference|
| &#128270;  | ClusteredIndex | ON account\_infor\_reference|
| &#128270;  | ClusteredIndex | ON project\_probability\_formula|
| &#128270;  | ClusteredIndex | ON project\_stage\_formula|
| &#128270;  | ClusteredIndex | ON construction\_stage\_formula|
| &#128270;  | ClusteredIndex | ON order\_date\_formula|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_notes|
| &#128270;  | ClusteredIndex | ON project\_region|
| &#128270;  | ClusteredIndex | ON pre\_bcr\_risk\_notes|
| &#128270;  | ClusteredIndex | ON opportunity\_review|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_completed|
| &#128270;  | ClusteredIndex | ON date\_time\_into\_costing|
| &#128270;  | ClusteredIndex | ON date\_time\_out\_costing|
| &#128270;  | ClusteredIndex | ON project\_id|
| &#128270;  | ClusteredIndex | ON days\_overdue|
| &#128270;  | ClusteredIndex | ON lines\_with\_no\_item\_tp|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table sharepoint.fabric_staging 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | week\_ending\_friday| date  |
| &#128270; | fte\_headcount| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON week\_ending\_friday|
| &#128270;  | ClusteredIndex | ON fte\_headcount|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint_staging.fabric_staging 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | week\_ending\_friday| date  |
| &#128270; | fte\_headcount| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON week\_ending\_friday|
| &#128270;  | ClusteredIndex | ON fte\_headcount|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table safety_culture.fact_ehs_visual_inspection 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | inspection\_id| varchar(255)  |
| &#128270; | conducted\_timestamp| datetime2(26)  |
| &#128270; | conducted\_date| date  |
| &#128270; | score\_percentage| decimal(18,6)  |
| &#128270; | template\_id| varchar(255)  |
| &#128270; | template\_name| varchar(500)  |
| &#128270; | site\_id| varchar(255)  |
| &#128270; | site\_name| varchar(500)  |
| &#128270; | archived| bit  |
| &#128270; | date\_key| int  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | created\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON inspection\_id|
| &#128270;  | ClusteredIndex | ON conducted\_timestamp|
| &#128270;  | ClusteredIndex | ON conducted\_date|
| &#128270;  | ClusteredIndex | ON score\_percentage|
| &#128270;  | ClusteredIndex | ON template\_id|
| &#128270;  | ClusteredIndex | ON template\_name|
| &#128270;  | ClusteredIndex | ON site\_id|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON archived|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON created\_timestamp|



### Table safety_culture.fact_ehs_visual_inspection_weekly 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | closed\_year| int  |
| * &#128270; | closed\_week| int  |
| * &#128270; | week\_key| int  |
| * &#128270; | week\_start\_date| date  |
| * &#128270; | week\_ending\_date| date  |
| * &#128270; | inspection\_count| bigint  |
| * &#128270; | scored\_inspection\_count| bigint  |
| &#128270; | average\_pass\_rate| decimal(18,6)  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON inspection\_count|
| &#128270;  | ClusteredIndex | ON scored\_inspection\_count|
| &#128270;  | ClusteredIndex | ON average\_pass\_rate|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table salesforce.fact_estimating 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | estimating\_request\_id| varchar(8000)  |
| &#128270; | estimating\_request\_no| varchar(8000)  |
| &#128270; | project\_name| varchar(8000)  |
| &#128270; | source\_owner\_id| varchar(8000)  |
| &#128270; | source\_owner\_name| varchar(8000)  |
| &#128270; | record\_type\_name| varchar(8000)  |
| &#128270; | complete\_by\_date| date  |
| &#128270; | closed\_timestamp| datetime2(26)  |
| &#128270; | closed\_date| date  |
| &#128270; | hours\_taken\_to\_close| decimal(18,4)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | project\_region| varchar(8000)  |
| &#128270; | request\_status| varchar(8000)  |
| &#128270; | currency\_code| varchar(8000)  |
| * &#128270; | is\_closed| bit  |
| &#128270; | on\_time\_flag| int  |
| &#128270; | closed\_date\_key| int  |
| &#128270; | closed\_customer\_year| int  |
| &#128270; | closed\_customer\_week\_no| int  |
| &#128270; | closed\_week\_start\_date| date  |
| &#128270; | closed\_week\_end\_date| date  |
| &#128270; | closed\_week\_key| int  |
| &#128270; | source\_created\_ts| datetime2(26)  |
| &#128270; | source\_modified\_ts| datetime2(26)  |
| * &#128270; | created\_ts| datetime2(26)  |
| * &#128270; | updated\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON estimating\_request\_id|
| &#128270;  | ClusteredIndex | ON estimating\_request\_no|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON source\_owner\_id|
| &#128270;  | ClusteredIndex | ON source\_owner\_name|
| &#128270;  | ClusteredIndex | ON record\_type\_name|
| &#128270;  | ClusteredIndex | ON complete\_by\_date|
| &#128270;  | ClusteredIndex | ON closed\_timestamp|
| &#128270;  | ClusteredIndex | ON closed\_date|
| &#128270;  | ClusteredIndex | ON hours\_taken\_to\_close|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON project\_region|
| &#128270;  | ClusteredIndex | ON request\_status|
| &#128270;  | ClusteredIndex | ON currency\_code|
| &#128270;  | ClusteredIndex | ON is\_closed|
| &#128270;  | ClusteredIndex | ON on\_time\_flag|
| &#128270;  | ClusteredIndex | ON closed\_date\_key|
| &#128270;  | ClusteredIndex | ON closed\_customer\_year|
| &#128270;  | ClusteredIndex | ON closed\_customer\_week\_no|
| &#128270;  | ClusteredIndex | ON closed\_week\_start\_date|
| &#128270;  | ClusteredIndex | ON closed\_week\_end\_date|
| &#128270;  | ClusteredIndex | ON closed\_week\_key|
| &#128270;  | ClusteredIndex | ON source\_created\_ts|
| &#128270;  | ClusteredIndex | ON source\_modified\_ts|
| &#128270;  | ClusteredIndex | ON created\_ts|
| &#128270;  | ClusteredIndex | ON updated\_ts|



### Table freshservice.fact_it_freshservice_survey 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | survey\_response\_id| varchar(255)  |
| &#128270; | ticket\_id| varchar(255)  |
| &#128270; | survey\_name| varchar(500)  |
| &#128270; | question| varchar(2000)  |
| &#128270; | question\_type| varchar(255)  |
| &#128270; | response\_timestamp| datetime2(26)  |
| &#128270; | reporting\_date| date  |
| &#128270; | score\_value| decimal(18,6)  |
| &#128270; | maximum\_score| decimal(18,6)  |
| &#128270; | satisfaction\_percentage| decimal(18,6)  |
| &#128270; | score\_source| varchar(100)  |
| &#128270; | nps\_rating| varchar(255)  |
| &#128270; | date\_key| int  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | created\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON survey\_response\_id|
| &#128270;  | ClusteredIndex | ON ticket\_id|
| &#128270;  | ClusteredIndex | ON survey\_name|
| &#128270;  | ClusteredIndex | ON question|
| &#128270;  | ClusteredIndex | ON question\_type|
| &#128270;  | ClusteredIndex | ON response\_timestamp|
| &#128270;  | ClusteredIndex | ON reporting\_date|
| &#128270;  | ClusteredIndex | ON score\_value|
| &#128270;  | ClusteredIndex | ON maximum\_score|
| &#128270;  | ClusteredIndex | ON satisfaction\_percentage|
| &#128270;  | ClusteredIndex | ON score\_source|
| &#128270;  | ClusteredIndex | ON nps\_rating|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON created\_ts|



### Table freshservice.fact_it_freshservice_survey_weekly 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | closed\_year| int  |
| * &#128270; | closed\_week| int  |
| * &#128270; | week\_key| int  |
| * &#128270; | week\_start\_date| date  |
| * &#128270; | week\_ending\_date| date  |
| * &#128270; | scored\_survey\_responses| bigint  |
| &#128270; | average\_satisfaction\_percentage| decimal(18,6)  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON scored\_survey\_responses|
| &#128270;  | ClusteredIndex | ON average\_satisfaction\_percentage|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table freshservice.fact_it_freshservice_ticket 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | ticket\_id| varchar(255)  |
| &#128270; | ticket\_type| varchar(255)  |
| &#128270; | category| varchar(500)  |
| &#128270; | service\_item| varchar(500)  |
| &#128270; | department\_name| varchar(500)  |
| &#128270; | agent\_group\_name| varchar(500)  |
| &#128270; | priority| varchar(100)  |
| &#128270; | ticket\_status| varchar(255)  |
| &#128270; | resolution\_status| varchar(500)  |
| &#128270; | created\_timestamp| datetime2(26)  |
| &#128270; | resolved\_timestamp| datetime2(26)  |
| &#128270; | closed\_timestamp| datetime2(26)  |
| &#128270; | reporting\_date| date  |
| &#128270; | is\_closed| bit  |
| &#128270; | is\_closed\_on\_time| bit  |
| &#128270; | sla\_classification| varchar(50)  |
| &#128270; | resolution\_time\_in\_bhrs| decimal(18,6)  |
| &#128270; | first\_response\_status| varchar(255)  |
| &#128270; | first\_response\_time\_in\_bhrs| decimal(18,6)  |
| &#128270; | date\_key| int  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | created\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON ticket\_id|
| &#128270;  | ClusteredIndex | ON ticket\_type|
| &#128270;  | ClusteredIndex | ON category|
| &#128270;  | ClusteredIndex | ON service\_item|
| &#128270;  | ClusteredIndex | ON department\_name|
| &#128270;  | ClusteredIndex | ON agent\_group\_name|
| &#128270;  | ClusteredIndex | ON priority|
| &#128270;  | ClusteredIndex | ON ticket\_status|
| &#128270;  | ClusteredIndex | ON resolution\_status|
| &#128270;  | ClusteredIndex | ON created\_timestamp|
| &#128270;  | ClusteredIndex | ON resolved\_timestamp|
| &#128270;  | ClusteredIndex | ON closed\_timestamp|
| &#128270;  | ClusteredIndex | ON reporting\_date|
| &#128270;  | ClusteredIndex | ON is\_closed|
| &#128270;  | ClusteredIndex | ON is\_closed\_on\_time|
| &#128270;  | ClusteredIndex | ON sla\_classification|
| &#128270;  | ClusteredIndex | ON resolution\_time\_in\_bhrs|
| &#128270;  | ClusteredIndex | ON first\_response\_status|
| &#128270;  | ClusteredIndex | ON first\_response\_time\_in\_bhrs|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON created\_ts|



### Table freshservice.fact_it_freshservice_ticket_weekly 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | closed\_year| int  |
| * &#128270; | closed\_week| int  |
| * &#128270; | week\_key| int  |
| * &#128270; | week\_start\_date| date  |
| * &#128270; | week\_ending\_date| date  |
| * &#128270; | closed\_tickets| bigint  |
| * &#128270; | sla\_classified\_tickets| bigint  |
| * &#128270; | closed\_on\_time\_tickets| bigint  |
| * &#128270; | late\_tickets| bigint  |
| * &#128270; | unclassified\_tickets| bigint  |
| &#128270; | closed\_on\_time\_percentage| decimal(18,6)  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON closed\_tickets|
| &#128270;  | ClusteredIndex | ON sla\_classified\_tickets|
| &#128270;  | ClusteredIndex | ON closed\_on\_time\_tickets|
| &#128270;  | ClusteredIndex | ON late\_tickets|
| &#128270;  | ClusteredIndex | ON unclassified\_tickets|
| &#128270;  | ClusteredIndex | ON closed\_on\_time\_percentage|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table elt.fact_kpi_result 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | calendar\_year| int  |
| &#128270; | week\_number| int  |
| * &#128270; | kpi\_name| varchar(200)  |
| * &#128270; | kpi\_category| varchar(100)  |
| * &#128270; | organisational\_unit| varchar(200)  |
| &#128270; | kpi\_value| decimal(18,4)  |
| &#128270; | target\_value| decimal(18,4)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | rag\_status| varchar(20)  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON calendar\_year|
| &#128270;  | ClusteredIndex | ON week\_number|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table freshservice.fact_kpi_result 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(255)  |
| &#128270; | kpi\_value| decimal(18,6)  |
| &#128270; | organisational\_unit| varchar(255)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(100)  |
| &#128270; | target\_value| decimal(18,6)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_code| varchar(100)  |
| &#128270; | department| varchar(255)  |
| &#128270; | measure| varchar(500)  |
| &#128270; | measure\_name| varchar(500)  |
| &#128270; | uom| varchar(50)  |
| &#128270; | sign| varchar(100)  |
| &#128270; | sign\_label| varchar(100)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | variance\_value| decimal(18,6)  |
| &#128270; | performance\_variance\_value| decimal(18,6)  |
| &#128270; | rag\_status| varchar(20)  |
| &#128270; | data\_status| varchar(50)  |
| &#128270; | source\_system| varchar(100)  |
| &#128270; | source\_object| varchar(500)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table reporting.fact_kpi_result 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_code| varchar(1000)  |
| &#128270; | kpi\_name| varchar(1000)  |
| &#128270; | kpi\_category| varchar(1000)  |
| &#128270; | organisational\_unit| varchar(1000)  |
| &#128270; | department| varchar(1000)  |
| &#128270; | measure| varchar(1000)  |
| &#128270; | measure\_name| varchar(1000)  |
| &#128270; | uom| varchar(1000)  |
| &#128270; | sign| varchar(1000)  |
| &#128270; | sign\_label| varchar(1000)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | breach\_direction| varchar(1000)  |
| &#128270; | kpi\_value| decimal(18,4)  |
| &#128270; | target\_value| decimal(18,4)  |
| &#128270; | variance\_value| decimal(18,4)  |
| &#128270; | performance\_variance\_value| decimal(18,4)  |
| &#128270; | rag\_status| varchar(1000)  |
| &#128270; | data\_status| varchar(1000)  |
| &#128270; | source\_system| varchar(1000)  |
| &#128270; | source\_object| varchar(1000)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table safety_culture.fact_kpi_result 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(255)  |
| &#128270; | kpi\_value| decimal(18,6)  |
| &#128270; | organisational\_unit| varchar(255)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(100)  |
| &#128270; | target\_value| decimal(18,6)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_code| varchar(100)  |
| &#128270; | department| varchar(255)  |
| &#128270; | measure| varchar(500)  |
| &#128270; | measure\_name| varchar(500)  |
| &#128270; | uom| varchar(50)  |
| &#128270; | sign| varchar(100)  |
| &#128270; | sign\_label| varchar(100)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | variance\_value| decimal(18,6)  |
| &#128270; | performance\_variance\_value| decimal(18,6)  |
| &#128270; | rag\_status| varchar(20)  |
| &#128270; | data\_status| varchar(50)  |
| &#128270; | source\_system| varchar(100)  |
| &#128270; | source\_object| varchar(500)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table salesforce.fact_kpi_result 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_code| varchar(1000)  |
| &#128270; | kpi\_name| varchar(1000)  |
| &#128270; | kpi\_category| varchar(1000)  |
| &#128270; | organisational\_unit| varchar(1000)  |
| &#128270; | department| varchar(1000)  |
| &#128270; | measure| varchar(1000)  |
| &#128270; | measure\_name| varchar(1000)  |
| &#128270; | uom| varchar(1000)  |
| &#128270; | sign| varchar(1000)  |
| &#128270; | sign\_label| varchar(1000)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | breach\_direction| varchar(1000)  |
| &#128270; | kpi\_value| decimal(18,4)  |
| &#128270; | target\_value| decimal(18,4)  |
| &#128270; | variance\_value| decimal(18,4)  |
| &#128270; | performance\_variance\_value| decimal(18,4)  |
| &#128270; | rag\_status| varchar(1000)  |
| &#128270; | data\_status| varchar(1000)  |
| &#128270; | source\_system| varchar(1000)  |
| &#128270; | source\_object| varchar(1000)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table syteline.fact_kpi_result 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_code| varchar(1000)  |
| &#128270; | kpi\_name| varchar(1000)  |
| &#128270; | kpi\_category| varchar(1000)  |
| &#128270; | organisational\_unit| varchar(1000)  |
| &#128270; | department| varchar(1000)  |
| &#128270; | measure| varchar(1000)  |
| &#128270; | measure\_name| varchar(1000)  |
| &#128270; | uom| varchar(1000)  |
| &#128270; | sign| varchar(1000)  |
| &#128270; | sign\_label| varchar(1000)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | breach\_direction| varchar(1000)  |
| &#128270; | kpi\_value| decimal(18,4)  |
| &#128270; | target\_value| decimal(18,4)  |
| &#128270; | variance\_value| decimal(18,4)  |
| &#128270; | performance\_variance\_value| decimal(18,4)  |
| &#128270; | rag\_status| varchar(1000)  |
| &#128270; | data\_status| varchar(1000)  |
| &#128270; | source\_system| varchar(1000)  |
| &#128270; | source\_object| varchar(1000)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table elt.fact_kpi_result_enriched 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | kpi\_id| bigint  |
| &#128270; | calendar\_year| int  |
| &#128270; | week\_number| int  |
| * &#128270; | kpi\_name| varchar(200)  |
| &#128270; | kpi\_category| varchar(200)  |
| * &#128270; | organisational\_unit| varchar(200)  |
| &#128270; | kpi\_value| decimal(18,4)  |
| &#128270; | target\_value| decimal(18,4)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | rag\_status| varchar(10)  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON calendar\_year|
| &#128270;  | ClusteredIndex | ON week\_number|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table staging.fact_kpi_result_staging 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | date\_key| int  |
| &#128270; | week\_ending\_date| date  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_end\_date| date  |
| &#128270; | calendar\_year| int  |
| &#128270; | week\_number| int  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_name| varchar(8000)  |
| &#128270; | kpi\_category| varchar(8000)  |
| &#128270; | organisational\_unit| varchar(8000)  |
| &#128270; | actual\_value| decimal(18,4)  |
| &#128270; | target\_value| decimal(18,4)  |
| &#128270; | variance\_value| decimal(19,4)  |
| &#128270; | breach\_direction| varchar(8000)  |
| &#128270; | rag\_status| varchar(8000)  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_end\_date|
| &#128270;  | ClusteredIndex | ON calendar\_year|
| &#128270;  | ClusteredIndex | ON week\_number|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON actual\_value|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table staging.fact_kpi_result_v3 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(8000)  |
| &#128270; | kpi\_value| float(53)  |
| &#128270; | organisational\_unit| varchar(8000)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(8000)  |
| &#128270; | target\_value| float(53)  |
| &#128270; | breach\_direction| varchar(8000)  |
| &#128270; | week\_key| varchar(8000)  |
| &#128270; | kpi\_code| varchar(8000)  |
| &#128270; | department| varchar(8000)  |
| &#128270; | measure| varchar(8000)  |
| &#128270; | measure\_name| varchar(8000)  |
| &#128270; | uom| varchar(8000)  |
| &#128270; | sign| varchar(8000)  |
| &#128270; | sign\_label| varchar(8000)  |
| &#128270; | commentary| varchar(8000)  |
| &#128270; | variance\_value| float(53)  |
| &#128270; | performance\_variance\_value| float(53)  |
| &#128270; | rag\_status| varchar(8000)  |
| &#128270; | data\_status| varchar(8000)  |
| &#128270; | source\_system| varchar(8000)  |
| &#128270; | source\_object| varchar(8000)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table salesforce.fact_order_tracking 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | order\_id| bigint  |
| * &#128270; | order\_tracking\_no| varchar(8000)  |
| &#128270; | project\_name| varchar(1000)  |
| &#128270; | infor\_order\_reference| varchar(1000)  |
| &#128270; | created\_date| date  |
| &#128270; | created\_date\_key| int  |
| &#128270; | created\_week\_key| int  |
| &#128270; | days\_in\_cleansing| decimal(18,4)  |
| &#128270; | days\_in\_signoff| decimal(18,4)  |
| &#128270; | days\_in\_engineering| decimal(18,4)  |
| &#128270; | days\_in\_scheduling| decimal(18,4)  |
| * &#128270; | created\_ts| datetime2(26)  |
| * &#128270; | updated\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON order\_id|
| &#128270;  | ClusteredIndex | ON order\_tracking\_no|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON infor\_order\_reference|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_date\_key|
| &#128270;  | ClusteredIndex | ON created\_week\_key|
| &#128270;  | ClusteredIndex | ON days\_in\_cleansing|
| &#128270;  | ClusteredIndex | ON days\_in\_signoff|
| &#128270;  | ClusteredIndex | ON days\_in\_engineering|
| &#128270;  | ClusteredIndex | ON days\_in\_scheduling|
| &#128270;  | ClusteredIndex | ON created\_ts|
| &#128270;  | ClusteredIndex | ON updated\_ts|



### Table syteline.fact_product_engineering_4_week_value_snapshot 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | snapshot\_date| date  |
| * &#128270; | snapshot\_timestamp| datetime2(26)  |
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | site\_name| varchar(100)  |
| * &#128270; | open\_order\_lines| bigint  |
| &#128270; | four\_week\_value\_k| decimal(18,6)  |
| * &#128270; | horizon\_weeks| int  |
| &#128270; | date\_key| int  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | calculation\_source| varchar(100)  |
| * &#128270; | created\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON snapshot\_date|
| &#128270;  | ClusteredIndex | ON snapshot\_timestamp|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON open\_order\_lines|
| &#128270;  | ClusteredIndex | ON four\_week\_value\_k|
| &#128270;  | ClusteredIndex | ON horizon\_weeks|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_source|
| &#128270;  | ClusteredIndex | ON created\_ts|



### Table syteline.fact_product_engineering_4_week_value_weekly 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | closed\_year| int  |
| * &#128270; | closed\_week| int  |
| * &#128270; | week\_key| int  |
| * &#128270; | week\_start\_date| date  |
| * &#128270; | week\_ending\_date| date  |
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | site\_name| varchar(100)  |
| * &#128270; | snapshot\_days| int  |
| &#128270; | average\_four\_week\_value\_k| decimal(18,6)  |
| &#128270; | minimum\_four\_week\_value\_k| decimal(18,6)  |
| &#128270; | maximum\_four\_week\_value\_k| decimal(18,6)  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | data\_status| varchar(50)  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON snapshot\_days|
| &#128270;  | ClusteredIndex | ON average\_four\_week\_value\_k|
| &#128270;  | ClusteredIndex | ON minimum\_four\_week\_value\_k|
| &#128270;  | ClusteredIndex | ON maximum\_four\_week\_value\_k|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table syteline.fact_product_engineering_items_completed_daily 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | snapshot\_date| date  |
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | site\_name| varchar(100)  |
| &#128270; | prior\_snapshot\_date| date  |
| &#128270; | snapshot\_gap\_days| int  |
| &#128270; | prior\_planning\_load| decimal(18,6)  |
| &#128270; | new\_items| decimal(18,6)  |
| &#128270; | current\_planning\_load| decimal(18,6)  |
| &#128270; | items\_completed| decimal(18,6)  |
| * &#128270; | calculation\_source| varchar(100)  |
| * &#128270; | data\_status| varchar(100)  |
| &#128270; | date\_key| int  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON snapshot\_date|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON prior\_snapshot\_date|
| &#128270;  | ClusteredIndex | ON snapshot\_gap\_days|
| &#128270;  | ClusteredIndex | ON prior\_planning\_load|
| &#128270;  | ClusteredIndex | ON new\_items|
| &#128270;  | ClusteredIndex | ON current\_planning\_load|
| &#128270;  | ClusteredIndex | ON items\_completed|
| &#128270;  | ClusteredIndex | ON calculation\_source|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table syteline.fact_product_engineering_new_items_snapshot 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | snapshot\_date| date  |
| * &#128270; | snapshot\_timestamp| datetime2(26)  |
| * &#128270; | snapshot\_hour| int  |
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | site\_name| varchar(100)  |
| &#128270; | new\_items| decimal(18,6)  |
| * &#128270; | source\_row\_count| bigint  |
| &#128270; | date\_key| int  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | created\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON snapshot\_date|
| &#128270;  | ClusteredIndex | ON snapshot\_timestamp|
| &#128270;  | ClusteredIndex | ON snapshot\_hour|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON new\_items|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON created\_ts|



### Table syteline.fact_product_engineering_planning_load_snapshot 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | snapshot\_date| date  |
| * &#128270; | snapshot\_timestamp| datetime2(26)  |
| * &#128270; | snapshot\_hour| int  |
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | site\_name| varchar(100)  |
| &#128270; | planning\_load| decimal(18,6)  |
| * &#128270; | source\_row\_count| bigint  |
| &#128270; | date\_key| int  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | created\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON snapshot\_date|
| &#128270;  | ClusteredIndex | ON snapshot\_timestamp|
| &#128270;  | ClusteredIndex | ON snapshot\_hour|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON planning\_load|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON date\_key|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON created\_ts|



### Table syteline.fact_product_engineering_productivity_daily 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | snapshot\_date| date  |
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | site\_name| varchar(100)  |
| &#128270; | items\_completed| decimal(18,6)  |
| &#128270; | daily\_capacity| decimal(18,6)  |
| &#128270; | productivity\_percentage| decimal(18,6)  |
| * &#128270; | capacity\_approved| bit  |
| * &#128270; | calculation\_source| varchar(100)  |
| * &#128270; | data\_status| varchar(100)  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | week\_key| int  |
| &#128270; | week\_start\_date| date  |
| &#128270; | week\_ending\_date| date  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON snapshot\_date|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON items\_completed|
| &#128270;  | ClusteredIndex | ON daily\_capacity|
| &#128270;  | ClusteredIndex | ON productivity\_percentage|
| &#128270;  | ClusteredIndex | ON capacity\_approved|
| &#128270;  | ClusteredIndex | ON calculation\_source|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table syteline.fact_product_engineering_productivity_weekly 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | closed\_year| int  |
| * &#128270; | closed\_week| int  |
| * &#128270; | week\_key| int  |
| * &#128270; | week\_start\_date| date  |
| * &#128270; | week\_ending\_date| date  |
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | site\_name| varchar(100)  |
| * &#128270; | snapshot\_days| int  |
| * &#128270; | complete\_days| int  |
| &#128270; | productivity\_percentage| decimal(18,6)  |
| &#128270; | items\_completed\_total| decimal(18,6)  |
| &#128270; | daily\_capacity| decimal(18,6)  |
| * &#128270; | capacity\_approved| bit  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | data\_status| varchar(100)  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON week\_start\_date|
| &#128270;  | ClusteredIndex | ON week\_ending\_date|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON snapshot\_days|
| &#128270;  | ClusteredIndex | ON complete\_days|
| &#128270;  | ClusteredIndex | ON productivity\_percentage|
| &#128270;  | ClusteredIndex | ON items\_completed\_total|
| &#128270;  | ClusteredIndex | ON daily\_capacity|
| &#128270;  | ClusteredIndex | ON capacity\_approved|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table salesforce.fact_proposal 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | proposal\_id| bigint  |
| * &#128270; | proposal\_request\_no| varchar(255)  |
| &#128270; | project\_name| varchar(500)  |
| &#128270; | record\_type| varchar(100)  |
| &#128270; | sales\_division| varchar(255)  |
| &#128270; | geography| varchar(255)  |
| &#128270; | opened\_date| datetime2(26)  |
| &#128270; | closed\_date| datetime2(26)  |
| &#128270; | closed\_date\_key| int  |
| &#128270; | week\_key| int  |
| &#128270; | currency\_code| varchar(10)  |
| &#128270; | estimated\_value\_native| decimal(18,2)  |
| &#128270; | exchange\_rate\_to\_gbp| decimal(18,8)  |
| &#128270; | estimated\_value\_gbp| decimal(18,2)  |
| * &#128270; | rejected\_drawings\_count| int  |
| * &#128270; | is\_closed| bit  |
| * &#128270; | created\_utc| datetime2(26)  |
| * &#128270; | updated\_utc| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON proposal\_id|
| &#128270;  | ClusteredIndex | ON proposal\_request\_no|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON record\_type|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON geography|
| &#128270;  | ClusteredIndex | ON opened\_date|
| &#128270;  | ClusteredIndex | ON closed\_date|
| &#128270;  | ClusteredIndex | ON closed\_date\_key|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON currency\_code|
| &#128270;  | ClusteredIndex | ON estimated\_value\_native|
| &#128270;  | ClusteredIndex | ON exchange\_rate\_to\_gbp|
| &#128270;  | ClusteredIndex | ON estimated\_value\_gbp|
| &#128270;  | ClusteredIndex | ON rejected\_drawings\_count|
| &#128270;  | ClusteredIndex | ON is\_closed|
| &#128270;  | ClusteredIndex | ON created\_utc|
| &#128270;  | ClusteredIndex | ON updated\_utc|



### Table staging.fact_proposal 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | proposal\_id| bigint  |
| &#128270; | proposal\_request\_no| varchar(8000)  |
| &#128270; | project\_name| varchar(8000)  |
| &#128270; | record\_type| varchar(8000)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | geography| varchar(8000)  |
| &#128270; | opened\_date| date  |
| &#128270; | closed\_date| date  |
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | closed\_month| int  |
| &#128270; | currency\_code| varchar(8000)  |
| &#128270; | estimated\_value\_native| decimal(18,2)  |
| &#128270; | exchange\_rate\_to\_gbp| decimal(18,8)  |
| &#128270; | estimated\_value\_gbp| decimal(18,2)  |
| &#128270; | is\_closed| bit  |
| &#128270; | rejected\_drawings\_count| int  |
| &#128270; | created\_utc| datetime2(26)  |
| &#128270; | updated\_utc| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON proposal\_id|
| &#128270;  | ClusteredIndex | ON proposal\_request\_no|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON record\_type|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON geography|
| &#128270;  | ClusteredIndex | ON opened\_date|
| &#128270;  | ClusteredIndex | ON closed\_date|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON closed\_month|
| &#128270;  | ClusteredIndex | ON currency\_code|
| &#128270;  | ClusteredIndex | ON estimated\_value\_native|
| &#128270;  | ClusteredIndex | ON exchange\_rate\_to\_gbp|
| &#128270;  | ClusteredIndex | ON estimated\_value\_gbp|
| &#128270;  | ClusteredIndex | ON is\_closed|
| &#128270;  | ClusteredIndex | ON rejected\_drawings\_count|
| &#128270;  | ClusteredIndex | ON created\_utc|
| &#128270;  | ClusteredIndex | ON updated\_utc|



### Table salesforce.fact_proposal_delivery 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | proposal\_id| bigint  |
| * &#128270; | proposal\_request\_no| varchar(255)  |
| &#128270; | due\_date| date  |
| &#128270; | due\_date\_key| int  |
| &#128270; | completed\_date| date  |
| &#128270; | completed\_date\_key| int  |
| * &#128270; | on\_time\_flag| int  |
| * &#128270; | is\_on\_time| bit  |
| * &#128270; | created\_utc| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON proposal\_id|
| &#128270;  | ClusteredIndex | ON proposal\_request\_no|
| &#128270;  | ClusteredIndex | ON due\_date|
| &#128270;  | ClusteredIndex | ON due\_date\_key|
| &#128270;  | ClusteredIndex | ON completed\_date|
| &#128270;  | ClusteredIndex | ON completed\_date\_key|
| &#128270;  | ClusteredIndex | ON on\_time\_flag|
| &#128270;  | ClusteredIndex | ON is\_on\_time|
| &#128270;  | ClusteredIndex | ON created\_utc|



### Table salesforce.fact_quality_weekly 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | customer\_year| int  |
| &#128270; | customer\_week\_no| int  |
| &#128270; | week\_key| int  |
| &#128270; | rejected\_drawings\_count| int  |
| * &#128270; | source| varchar(50)  |
| * &#128270; | record\_count| bigint  |
| * &#128270; | created\_utc| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON customer\_year|
| &#128270;  | ClusteredIndex | ON customer\_week\_no|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON rejected\_drawings\_count|
| &#128270;  | ClusteredIndex | ON source|
| &#128270;  | ClusteredIndex | ON record\_count|
| &#128270;  | ClusteredIndex | ON created\_utc|



### Table metadata.gold_run 
|Idx |Name |Data Type |
|---|---|---|
| * &#128273;  | run\_id| bigint identity  |
| &#128270; | pipeline\_run\_id| varchar(100)  |
| * &#128270; | trigger\_time| datetime2(26)  |
| * &#128270; | start\_time| datetime2(26)  |
| &#128270; | end\_time| datetime2(26)  |
| * &#128270; | status| varchar(30)  |
| * &#128270; | created\_at| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128273;  | pk\_gold\_run | ON run\_id|
| &#128270;  | ClusteredIndex | ON pipeline\_run\_id|
| &#128270;  | ClusteredIndex | ON trigger\_time|
| &#128270;  | ClusteredIndex | ON start\_time|
| &#128270;  | ClusteredIndex | ON end\_time|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON created\_at|



### Table sharepoint.incident_register 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | date| varchar(8000)  |
| &#128270; | site| varchar(8000)  |
| &#128270; | location| varchar(8000)  |
| &#128270; | brief\_description| varchar(8000)  |
| &#128270; | accident\_level| varchar(8000)  |
| &#128270; | investigation\_number| varchar(8000)  |
| &#128270; | injury\_type| varchar(8000)  |
| &#128270; | body\_part| varchar(8000)  |
| &#128270; | task\_undertaken| varchar(8000)  |
| &#128270; | systems\_cause| varchar(8000)  |
| &#128270; | tools\_cause| varchar(8000)  |
| &#128270; | environment\_cause| varchar(8000)  |
| &#128270; | people\_cause| varchar(8000)  |
| &#128270; | root\_cause| varchar(8000)  |
| &#128270; | containment\_action| varchar(8000)  |
| &#128270; | corrective\_action| varchar(8000)  |
| &#128270; | status| varchar(8000)  |
| &#128270; | lost\_days| varchar(8000)  |
| &#128270; | riddor\_date| varchar(8000)  |
| &#128270; | target\_ca\_completion\_date| varchar(8000)  |
| &#128270; | actual\_ca\_completion\_date| varchar(8000)  |
| &#128270; | unnamed\_21| varchar(8000)  |
| &#128270; | system\_causes| varchar(8000)  |
| &#128270; | unnamed\_23| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON date|
| &#128270;  | ClusteredIndex | ON site|
| &#128270;  | ClusteredIndex | ON location|
| &#128270;  | ClusteredIndex | ON brief\_description|
| &#128270;  | ClusteredIndex | ON accident\_level|
| &#128270;  | ClusteredIndex | ON investigation\_number|
| &#128270;  | ClusteredIndex | ON injury\_type|
| &#128270;  | ClusteredIndex | ON body\_part|
| &#128270;  | ClusteredIndex | ON task\_undertaken|
| &#128270;  | ClusteredIndex | ON systems\_cause|
| &#128270;  | ClusteredIndex | ON tools\_cause|
| &#128270;  | ClusteredIndex | ON environment\_cause|
| &#128270;  | ClusteredIndex | ON people\_cause|
| &#128270;  | ClusteredIndex | ON root\_cause|
| &#128270;  | ClusteredIndex | ON containment\_action|
| &#128270;  | ClusteredIndex | ON corrective\_action|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON lost\_days|
| &#128270;  | ClusteredIndex | ON riddor\_date|
| &#128270;  | ClusteredIndex | ON target\_ca\_completion\_date|
| &#128270;  | ClusteredIndex | ON actual\_ca\_completion\_date|
| &#128270;  | ClusteredIndex | ON unnamed\_21|
| &#128270;  | ClusteredIndex | ON system\_causes|
| &#128270;  | ClusteredIndex | ON unnamed\_23|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint_staging.incident_register 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | date| varchar(8000)  |
| &#128270; | site| varchar(8000)  |
| &#128270; | location| varchar(8000)  |
| &#128270; | brief\_description| varchar(8000)  |
| &#128270; | accident\_level| varchar(8000)  |
| &#128270; | investigation\_number| varchar(8000)  |
| &#128270; | injury\_type| varchar(8000)  |
| &#128270; | body\_part| varchar(8000)  |
| &#128270; | task\_undertaken| varchar(8000)  |
| &#128270; | systems\_cause| varchar(8000)  |
| &#128270; | tools\_cause| varchar(8000)  |
| &#128270; | environment\_cause| varchar(8000)  |
| &#128270; | people\_cause| varchar(8000)  |
| &#128270; | root\_cause| varchar(8000)  |
| &#128270; | containment\_action| varchar(8000)  |
| &#128270; | corrective\_action| varchar(8000)  |
| &#128270; | status| varchar(8000)  |
| &#128270; | lost\_days| varchar(8000)  |
| &#128270; | riddor\_date| varchar(8000)  |
| &#128270; | target\_ca\_completion\_date| varchar(8000)  |
| &#128270; | actual\_ca\_completion\_date| varchar(8000)  |
| &#128270; | unnamed\_21| varchar(8000)  |
| &#128270; | system\_causes| varchar(8000)  |
| &#128270; | unnamed\_23| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON date|
| &#128270;  | ClusteredIndex | ON site|
| &#128270;  | ClusteredIndex | ON location|
| &#128270;  | ClusteredIndex | ON brief\_description|
| &#128270;  | ClusteredIndex | ON accident\_level|
| &#128270;  | ClusteredIndex | ON investigation\_number|
| &#128270;  | ClusteredIndex | ON injury\_type|
| &#128270;  | ClusteredIndex | ON body\_part|
| &#128270;  | ClusteredIndex | ON task\_undertaken|
| &#128270;  | ClusteredIndex | ON systems\_cause|
| &#128270;  | ClusteredIndex | ON tools\_cause|
| &#128270;  | ClusteredIndex | ON environment\_cause|
| &#128270;  | ClusteredIndex | ON people\_cause|
| &#128270;  | ClusteredIndex | ON root\_cause|
| &#128270;  | ClusteredIndex | ON containment\_action|
| &#128270;  | ClusteredIndex | ON corrective\_action|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON lost\_days|
| &#128270;  | ClusteredIndex | ON riddor\_date|
| &#128270;  | ClusteredIndex | ON target\_ca\_completion\_date|
| &#128270;  | ClusteredIndex | ON actual\_ca\_completion\_date|
| &#128270;  | ClusteredIndex | ON unnamed\_21|
| &#128270;  | ClusteredIndex | ON system\_causes|
| &#128270;  | ClusteredIndex | ON unnamed\_23|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table safety_culture_staging.inspections 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | archived| bit  |
| &#128270; | asset\_id| varchar(8000)  |
| &#128270; | author\_id| varchar(8000)  |
| &#128270; | author\_name| varchar(8000)  |
| &#128270; | client\_site| varchar(8000)  |
| &#128270; | conducted\_on| datetime2(26)  |
| &#128270; | created\_at| datetime2(26)  |
| &#128270; | date\_completed| datetime2(26)  |
| &#128270; | date\_modified| datetime2(26)  |
| &#128270; | date\_started| datetime2(26)  |
| &#128270; | document\_no| varchar(8000)  |
| &#128270; | duration| varchar(8000)  |
| &#128270; | id| varchar(8000)  |
| &#128270; | latitude| varchar(8000)  |
| &#128270; | location| varchar(8000)  |
| &#128270; | longitude| varchar(8000)  |
| &#128270; | max\_score| bigint  |
| &#128270; | modified\_at| datetime2(26)  |
| &#128270; | name| varchar(8000)  |
| &#128270; | organisation\_id| varchar(8000)  |
| &#128270; | owner\_id| varchar(8000)  |
| &#128270; | owner\_name| varchar(8000)  |
| &#128270; | personnel| varchar(8000)  |
| &#128270; | prepared\_by| varchar(8000)  |
| &#128270; | score| varchar(8000)  |
| &#128270; | score\_percentage| varchar(8000)  |
| &#128270; | site\_id| varchar(8000)  |
| &#128270; | template\_author| varchar(8000)  |
| &#128270; | template\_id| varchar(8000)  |
| &#128270; | template\_name| varchar(8000)  |
| &#128270; | web\_report\_link| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON archived|
| &#128270;  | ClusteredIndex | ON asset\_id|
| &#128270;  | ClusteredIndex | ON author\_id|
| &#128270;  | ClusteredIndex | ON author\_name|
| &#128270;  | ClusteredIndex | ON client\_site|
| &#128270;  | ClusteredIndex | ON conducted\_on|
| &#128270;  | ClusteredIndex | ON created\_at|
| &#128270;  | ClusteredIndex | ON date\_completed|
| &#128270;  | ClusteredIndex | ON date\_modified|
| &#128270;  | ClusteredIndex | ON date\_started|
| &#128270;  | ClusteredIndex | ON document\_no|
| &#128270;  | ClusteredIndex | ON duration|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON latitude|
| &#128270;  | ClusteredIndex | ON location|
| &#128270;  | ClusteredIndex | ON longitude|
| &#128270;  | ClusteredIndex | ON max\_score|
| &#128270;  | ClusteredIndex | ON modified\_at|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON organisation\_id|
| &#128270;  | ClusteredIndex | ON owner\_id|
| &#128270;  | ClusteredIndex | ON owner\_name|
| &#128270;  | ClusteredIndex | ON personnel|
| &#128270;  | ClusteredIndex | ON prepared\_by|
| &#128270;  | ClusteredIndex | ON score|
| &#128270;  | ClusteredIndex | ON score\_percentage|
| &#128270;  | ClusteredIndex | ON site\_id|
| &#128270;  | ClusteredIndex | ON template\_author|
| &#128270;  | ClusteredIndex | ON template\_id|
| &#128270;  | ClusteredIndex | ON template\_name|
| &#128270;  | ClusteredIndex | ON web\_report\_link|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.inv_hdr_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | inv\_num| varchar(8000)  |
| &#128270; | inv\_seq| int  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | cust\_seq| int  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | inv\_date| datetime2(26)  |
| &#128270; | terms\_code| varchar(8000)  |
| &#128270; | ship\_code| varchar(8000)  |
| &#128270; | cust\_po| varchar(8000)  |
| &#128270; | weight| decimal(9,2)  |
| &#128270; | qty\_packages| int  |
| &#128270; | ship\_date| datetime2(26)  |
| &#128270; | misc\_charges| decimal(23,8)  |
| &#128270; | prepaid\_amt| decimal(23,8)  |
| &#128270; | freight| decimal(23,8)  |
| &#128270; | cost| decimal(23,8)  |
| &#128270; | price| decimal(23,8)  |
| &#128270; | slsman| varchar(8000)  |
| &#128270; | comm\_calc| decimal(23,8)  |
| &#128270; | comm\_due| decimal(23,8)  |
| &#128270; | comm\_paid| decimal(23,8)  |
| &#128270; | comm\_base| decimal(23,8)  |
| &#128270; | state| varchar(8000)  |
| &#128270; | misc\_acct| varchar(8000)  |
| &#128270; | freight\_acct| varchar(8000)  |
| &#128270; | tot\_comm\_due| decimal(23,8)  |
| &#128270; | tot\_comm\_pd| decimal(23,8)  |
| &#128270; | mgr\_comm\_cal| decimal(23,8)  |
| &#128270; | mgr\_comm\_bse| decimal(23,8)  |
| &#128270; | bill\_type| varchar(8000)  |
| &#128270; | exch\_rate| decimal(12,7)  |
| &#128270; | use\_exch\_rate| int  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | tax\_date| datetime2(26)  |
| &#128270; | ec\_code| varchar(8000)  |
| &#128270; | frt\_tax\_code1| varchar(8000)  |
| &#128270; | frt\_tax\_code2| varchar(8000)  |
| &#128270; | msc\_tax\_code1| varchar(8000)  |
| &#128270; | msc\_tax\_code2| varchar(8000)  |
| &#128270; | disc| decimal(11,8)  |
| &#128270; | misc\_acct\_unit1| varchar(8000)  |
| &#128270; | misc\_acct\_unit2| varchar(8000)  |
| &#128270; | misc\_acct\_unit3| varchar(8000)  |
| &#128270; | misc\_acct\_unit4| varchar(8000)  |
| &#128270; | freight\_acct\_unit1| varchar(8000)  |
| &#128270; | freight\_acct\_unit2| varchar(8000)  |
| &#128270; | freight\_acct\_unit3| varchar(8000)  |
| &#128270; | freight\_acct\_unit4| varchar(8000)  |
| &#128270; | do\_num| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | disc\_amount| decimal(23,8)  |
| &#128270; | shipment\_id| decimal(19,0)  |
| &#128270; | builder\_inv\_orig\_site| varchar(8000)  |
| &#128270; | builder\_inv\_num| varchar(8000)  |
| &#128270; | vtxexempted| int  |
| &#128270; | cn\_vat\_inv\_num| varchar(8000)  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | cn\_comment| varchar(8000)  |
| &#128270; | uf\_concern\_no| varchar(8000)  |
| &#128270; | uf\_invoice\_note| varchar(8000)  |
| &#128270; | uf\_query\_reason| varchar(8000)  |
| &#128270; | uf\_whse| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON inv\_num|
| &#128270;  | ClusteredIndex | ON inv\_seq|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON cust\_seq|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON inv\_date|
| &#128270;  | ClusteredIndex | ON terms\_code|
| &#128270;  | ClusteredIndex | ON ship\_code|
| &#128270;  | ClusteredIndex | ON cust\_po|
| &#128270;  | ClusteredIndex | ON weight|
| &#128270;  | ClusteredIndex | ON qty\_packages|
| &#128270;  | ClusteredIndex | ON ship\_date|
| &#128270;  | ClusteredIndex | ON misc\_charges|
| &#128270;  | ClusteredIndex | ON prepaid\_amt|
| &#128270;  | ClusteredIndex | ON freight|
| &#128270;  | ClusteredIndex | ON cost|
| &#128270;  | ClusteredIndex | ON price|
| &#128270;  | ClusteredIndex | ON slsman|
| &#128270;  | ClusteredIndex | ON comm\_calc|
| &#128270;  | ClusteredIndex | ON comm\_due|
| &#128270;  | ClusteredIndex | ON comm\_paid|
| &#128270;  | ClusteredIndex | ON comm\_base|
| &#128270;  | ClusteredIndex | ON state|
| &#128270;  | ClusteredIndex | ON misc\_acct|
| &#128270;  | ClusteredIndex | ON freight\_acct|
| &#128270;  | ClusteredIndex | ON tot\_comm\_due|
| &#128270;  | ClusteredIndex | ON tot\_comm\_pd|
| &#128270;  | ClusteredIndex | ON mgr\_comm\_cal|
| &#128270;  | ClusteredIndex | ON mgr\_comm\_bse|
| &#128270;  | ClusteredIndex | ON bill\_type|
| &#128270;  | ClusteredIndex | ON exch\_rate|
| &#128270;  | ClusteredIndex | ON use\_exch\_rate|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON tax\_date|
| &#128270;  | ClusteredIndex | ON ec\_code|
| &#128270;  | ClusteredIndex | ON frt\_tax\_code1|
| &#128270;  | ClusteredIndex | ON frt\_tax\_code2|
| &#128270;  | ClusteredIndex | ON msc\_tax\_code1|
| &#128270;  | ClusteredIndex | ON msc\_tax\_code2|
| &#128270;  | ClusteredIndex | ON disc|
| &#128270;  | ClusteredIndex | ON misc\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON misc\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON misc\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON misc\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON freight\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON freight\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON freight\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON freight\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON do\_num|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON disc\_amount|
| &#128270;  | ClusteredIndex | ON shipment\_id|
| &#128270;  | ClusteredIndex | ON builder\_inv\_orig\_site|
| &#128270;  | ClusteredIndex | ON builder\_inv\_num|
| &#128270;  | ClusteredIndex | ON vtxexempted|
| &#128270;  | ClusteredIndex | ON cn\_vat\_inv\_num|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON cn\_comment|
| &#128270;  | ClusteredIndex | ON uf\_concern\_no|
| &#128270;  | ClusteredIndex | ON uf\_invoice\_note|
| &#128270;  | ClusteredIndex | ON uf\_query\_reason|
| &#128270;  | ClusteredIndex | ON uf\_whse|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.inv_item_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | inv\_num| varchar(8000)  |
| &#128270; | inv\_seq| int  |
| &#128270; | inv\_line| int  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | co\_line| int  |
| &#128270; | co\_release| int  |
| &#128270; | item| varchar(8000)  |
| &#128270; | qty\_invoiced| decimal(19,8)  |
| &#128270; | disc| decimal(11,8)  |
| &#128270; | cost| decimal(20,8)  |
| &#128270; | price| decimal(20,8)  |
| &#128270; | sales\_acct| varchar(8000)  |
| &#128270; | old\_price| decimal(20,8)  |
| &#128270; | new\_price| decimal(20,8)  |
| &#128270; | process\_ind| varchar(8000)  |
| &#128270; | cons\_num| int  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | tax\_date| datetime2(26)  |
| &#128270; | sales\_acct\_unit1| varchar(8000)  |
| &#128270; | sales\_acct\_unit2| varchar(8000)  |
| &#128270; | sales\_acct\_unit3| varchar(8000)  |
| &#128270; | sales\_acct\_unit4| varchar(8000)  |
| &#128270; | cust\_po| varchar(8000)  |
| &#128270; | restock\_fee\_amt| decimal(23,8)  |
| &#128270; | do\_num| varchar(8000)  |
| &#128270; | do\_line| int  |
| &#128270; | do\_seq| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | orig\_inv\_num| varchar(8000)  |
| &#128270; | reason\_text| varchar(8000)  |
| &#128270; | excise\_tax\_percent| decimal(4,2)  |
| &#128270; | pl\_inv\_line\_num| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON inv\_num|
| &#128270;  | ClusteredIndex | ON inv\_seq|
| &#128270;  | ClusteredIndex | ON inv\_line|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON co\_line|
| &#128270;  | ClusteredIndex | ON co\_release|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON qty\_invoiced|
| &#128270;  | ClusteredIndex | ON disc|
| &#128270;  | ClusteredIndex | ON cost|
| &#128270;  | ClusteredIndex | ON price|
| &#128270;  | ClusteredIndex | ON sales\_acct|
| &#128270;  | ClusteredIndex | ON old\_price|
| &#128270;  | ClusteredIndex | ON new\_price|
| &#128270;  | ClusteredIndex | ON process\_ind|
| &#128270;  | ClusteredIndex | ON cons\_num|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON tax\_date|
| &#128270;  | ClusteredIndex | ON sales\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON sales\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON sales\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON sales\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON cust\_po|
| &#128270;  | ClusteredIndex | ON restock\_fee\_amt|
| &#128270;  | ClusteredIndex | ON do\_num|
| &#128270;  | ClusteredIndex | ON do\_line|
| &#128270;  | ClusteredIndex | ON do\_seq|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON orig\_inv\_num|
| &#128270;  | ClusteredIndex | ON reason\_text|
| &#128270;  | ClusteredIndex | ON excise\_tax\_percent|
| &#128270;  | ClusteredIndex | ON pl\_inv\_line\_num|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table safety_culture_staging.issues 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | asset\_id| varchar(100)  |
| &#128270; | category\_description| varchar(5000)  |
| &#128270; | category\_id| varchar(100)  |
| &#128270; | category\_label| varchar(100)  |
| &#128270; | completed\_at| varchar(100)  |
| &#128270; | created\_at| varchar(100)  |
| &#128270; | creator\_id| varchar(100)  |
| &#128270; | creator\_user\_name| varchar(100)  |
| &#128270; | description| varchar(100)  |
| &#128270; | due\_at| varchar(100)  |
| &#128270; | id| varchar(100)  |
| &#128270; | inspection\_id| varchar(100)  |
| &#128270; | inspection\_name| varchar(100)  |
| &#128270; | location\_name| varchar(100)  |
| &#128270; | modified\_at| varchar(100)  |
| &#128270; | occurred\_at| varchar(100)  |
| &#128270; | priority| varchar(100)  |
| &#128270; | site\_id| varchar(100)  |
| &#128270; | site\_name| varchar(100)  |
| &#128270; | status| varchar(100)  |
| &#128270; | template\_id| varchar(100)  |
| &#128270; | title| varchar(100)  |
| &#128270; | unique\_id| varchar(100)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON asset\_id|
| &#128270;  | ClusteredIndex | ON category\_description|
| &#128270;  | ClusteredIndex | ON category\_id|
| &#128270;  | ClusteredIndex | ON category\_label|
| &#128270;  | ClusteredIndex | ON completed\_at|
| &#128270;  | ClusteredIndex | ON created\_at|
| &#128270;  | ClusteredIndex | ON creator\_id|
| &#128270;  | ClusteredIndex | ON creator\_user\_name|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON due\_at|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON inspection\_id|
| &#128270;  | ClusteredIndex | ON inspection\_name|
| &#128270;  | ClusteredIndex | ON location\_name|
| &#128270;  | ClusteredIndex | ON modified\_at|
| &#128270;  | ClusteredIndex | ON occurred\_at|
| &#128270;  | ClusteredIndex | ON priority|
| &#128270;  | ClusteredIndex | ON site\_id|
| &#128270;  | ClusteredIndex | ON site\_name|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON template\_id|
| &#128270;  | ClusteredIndex | ON title|
| &#128270;  | ClusteredIndex | ON unique\_id|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table sharepoint.it_purchasing_2026_staging 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | users\_names| varchar(8000)  |
| &#128270; | item| varchar(8000)  |
| &#128270; | url| varchar(8000)  |
| &#128270; | quantity| varchar(8000)  |
| &#128270; | vendor\_id| varchar(8000)  |
| &#128270; | total\_each| varchar(8000)  |
| &#128270; | total\_excluding\_vat\_each| varchar(8000)  |
| &#128270; | final\_total| varchar(8000)  |
| &#128270; | site| varchar(8000)  |
| &#128270; | budgeted| varchar(8000)  |
| &#128270; | date\_ordered| varchar(8000)  |
| &#128270; | requisition\_number| varchar(8000)  |
| &#128270; | purchase\_order\_number| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON users\_names|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON url|
| &#128270;  | ClusteredIndex | ON quantity|
| &#128270;  | ClusteredIndex | ON vendor\_id|
| &#128270;  | ClusteredIndex | ON total\_each|
| &#128270;  | ClusteredIndex | ON total\_excluding\_vat\_each|
| &#128270;  | ClusteredIndex | ON final\_total|
| &#128270;  | ClusteredIndex | ON site|
| &#128270;  | ClusteredIndex | ON budgeted|
| &#128270;  | ClusteredIndex | ON date\_ordered|
| &#128270;  | ClusteredIndex | ON requisition\_number|
| &#128270;  | ClusteredIndex | ON purchase\_order\_number|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint_staging.it_purchasing_2026_staging 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | users\_names| varchar(8000)  |
| &#128270; | item| varchar(8000)  |
| &#128270; | url| varchar(8000)  |
| &#128270; | quantity| varchar(8000)  |
| &#128270; | vendor\_id| varchar(8000)  |
| &#128270; | total\_each| varchar(8000)  |
| &#128270; | total\_excluding\_vat\_each| varchar(8000)  |
| &#128270; | final\_total| varchar(8000)  |
| &#128270; | site| varchar(8000)  |
| &#128270; | budgeted| varchar(8000)  |
| &#128270; | date\_ordered| varchar(8000)  |
| &#128270; | requisition\_number| varchar(8000)  |
| &#128270; | purchase\_order\_number| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON users\_names|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON url|
| &#128270;  | ClusteredIndex | ON quantity|
| &#128270;  | ClusteredIndex | ON vendor\_id|
| &#128270;  | ClusteredIndex | ON total\_each|
| &#128270;  | ClusteredIndex | ON total\_excluding\_vat\_each|
| &#128270;  | ClusteredIndex | ON final\_total|
| &#128270;  | ClusteredIndex | ON site|
| &#128270;  | ClusteredIndex | ON budgeted|
| &#128270;  | ClusteredIndex | ON date\_ordered|
| &#128270;  | ClusteredIndex | ON requisition\_number|
| &#128270;  | ClusteredIndex | ON purchase\_order\_number|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.item_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | item| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | qty\_allocjob| decimal(20,8)  |
| &#128270; | u\_m| varchar(8000)  |
| &#128270; | lead\_time| int  |
| &#128270; | lot\_size| decimal(18,8)  |
| &#128270; | qty\_used\_ytd| decimal(20,8)  |
| &#128270; | qty\_mfg\_ytd| decimal(20,8)  |
| &#128270; | abc\_code| varchar(8000)  |
| &#128270; | drawing\_nbr| varchar(8000)  |
| &#128270; | product\_code| varchar(8000)  |
| &#128270; | p\_m\_t\_code| varchar(8000)  |
| &#128270; | cost\_method| varchar(8000)  |
| &#128270; | lst\_lot\_size| decimal(9,3)  |
| &#128270; | unit\_cost| decimal(20,8)  |
| &#128270; | lst\_u\_cost| decimal(20,8)  |
| &#128270; | avg\_u\_cost| decimal(20,8)  |
| &#128270; | job| varchar(8000)  |
| &#128270; | suffix| int  |
| &#128270; | stocked| int  |
| &#128270; | matl\_type| varchar(8000)  |
| &#128270; | family\_code| varchar(8000)  |
| &#128270; | low\_level| int  |
| &#128270; | last\_inv| datetime2(26)  |
| &#128270; | days\_supply| int  |
| &#128270; | order\_min| decimal(19,8)  |
| &#128270; | order\_mult| decimal(19,8)  |
| &#128270; | plan\_code| varchar(8000)  |
| &#128270; | mps\_flag| int  |
| &#128270; | accept\_req| int  |
| &#128270; | change\_date| datetime2(26)  |
| &#128270; | revision| varchar(8000)  |
| &#128270; | phantom\_flag| int  |
| &#128270; | plan\_flag| int  |
| &#128270; | paper\_time| int  |
| &#128270; | dock\_time| int  |
| &#128270; | asm\_setup| decimal(20,8)  |
| &#128270; | asm\_run| decimal(20,8)  |
| &#128270; | asm\_matl| decimal(20,8)  |
| &#128270; | asm\_tool| decimal(20,8)  |
| &#128270; | asm\_fixture| decimal(20,8)  |
| &#128270; | asm\_other| decimal(20,8)  |
| &#128270; | asm\_fixed| decimal(20,8)  |
| &#128270; | asm\_var| decimal(20,8)  |
| &#128270; | asm\_outside| decimal(20,8)  |
| &#128270; | comp\_setup| decimal(20,8)  |
| &#128270; | comp\_run| decimal(20,8)  |
| &#128270; | comp\_matl| decimal(20,8)  |
| &#128270; | comp\_tool| decimal(20,8)  |
| &#128270; | comp\_fixture| decimal(20,8)  |
| &#128270; | comp\_other| decimal(20,8)  |
| &#128270; | comp\_fixed| decimal(20,8)  |
| &#128270; | comp\_var| decimal(20,8)  |
| &#128270; | comp\_outside| decimal(20,8)  |
| &#128270; | sub\_matl| decimal(20,8)  |
| &#128270; | shrink\_fact| decimal(5,4)  |
| &#128270; | alt\_item| varchar(8000)  |
| &#128270; | unit\_weight| decimal(11,5)  |
| &#128270; | weight\_units| varchar(8000)  |
| &#128270; | charfld4| varchar(8000)  |
| &#128270; | cur\_u\_cost| decimal(20,8)  |
| &#128270; | feat\_type| varchar(8000)  |
| &#128270; | var\_lead| decimal(10,5)  |
| &#128270; | feat\_str| varchar(8000)  |
| &#128270; | next\_config| int  |
| &#128270; | feat\_templ| varchar(8000)  |
| &#128270; | backflush| int  |
| &#128270; | charfld1| varchar(8000)  |
| &#128270; | charfld2| varchar(8000)  |
| &#128270; | charfld3| varchar(8000)  |
| &#128270; | decifld1| decimal(10,2)  |
| &#128270; | decifld2| decimal(10,2)  |
| &#128270; | decifld3| decimal(10,2)  |
| &#128270; | logifld| int  |
| &#128270; | datefld| datetime2(26)  |
| &#128270; | track\_ecn| int  |
| &#128270; | u\_ws\_price| decimal(20,8)  |
| &#128270; | comm\_code| varchar(8000)  |
| &#128270; | origin| varchar(8000)  |
| &#128270; | unit\_mat\_cost| decimal(20,8)  |
| &#128270; | unit\_duty\_cost| decimal(20,8)  |
| &#128270; | unit\_freight\_cost| decimal(20,8)  |
| &#128270; | unit\_brokerage\_cost| decimal(20,8)  |
| &#128270; | cur\_mat\_cost| decimal(20,8)  |
| &#128270; | cur\_duty\_cost| decimal(20,8)  |
| &#128270; | cur\_freight\_cost| decimal(20,8)  |
| &#128270; | cur\_brokerage\_cost| decimal(20,8)  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | bflush\_loc| varchar(8000)  |
| &#128270; | reservable| int  |
| &#128270; | shelf\_life| int  |
| &#128270; | lot\_prefix| varchar(8000)  |
| &#128270; | serial\_prefix| varchar(8000)  |
| &#128270; | serial\_length| int  |
| &#128270; | issue\_by| varchar(8000)  |
| &#128270; | serial\_tracked| int  |
| &#128270; | lot\_tracked| int  |
| &#128270; | cost\_type| varchar(8000)  |
| &#128270; | matl\_cost| decimal(20,8)  |
| &#128270; | lbr\_cost| decimal(20,8)  |
| &#128270; | fovhd\_cost| decimal(20,8)  |
| &#128270; | vovhd\_cost| decimal(20,8)  |
| &#128270; | out\_cost| decimal(20,8)  |
| &#128270; | cur\_matl\_cost| decimal(20,8)  |
| &#128270; | cur\_lbr\_cost| decimal(20,8)  |
| &#128270; | cur\_fovhd\_cost| decimal(20,8)  |
| &#128270; | cur\_vovhd\_cost| decimal(20,8)  |
| &#128270; | cur\_out\_cost| decimal(20,8)  |
| &#128270; | avg\_matl\_cost| decimal(20,8)  |
| &#128270; | avg\_lbr\_cost| decimal(20,8)  |
| &#128270; | avg\_fovhd\_cost| decimal(20,8)  |
| &#128270; | avg\_vovhd\_cost| decimal(20,8)  |
| &#128270; | avg\_out\_cost| decimal(20,8)  |
| &#128270; | prod\_type| varchar(8000)  |
| &#128270; | rate\_per\_day| decimal(10,3)  |
| &#128270; | mps\_plan\_fence| int  |
| &#128270; | pass\_req| int  |
| &#128270; | lot\_gen\_exp| int  |
| &#128270; | supply\_site| varchar(8000)  |
| &#128270; | prod\_mix| varchar(8000)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | status\_chg\_user\_code| varchar(8000)  |
| &#128270; | chg\_date| datetime2(26)  |
| &#128270; | reason\_code| varchar(8000)  |
| &#128270; | supply\_whse| varchar(8000)  |
| &#128270; | due\_period| int  |
| &#128270; | order\_max| decimal(19,8)  |
| &#128270; | mrp\_part| int  |
| &#128270; | infinite\_part| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | supply\_tolerance\_hrs| decimal(4,1)  |
| &#128270; | exp\_lead\_time| int  |
| &#128270; | var\_exp\_lead| decimal(10,5)  |
| &#128270; | buyer| varchar(8000)  |
| &#128270; | order\_configurable| int  |
| &#128270; | job\_configurable| int  |
| &#128270; | cfg\_model| varchar(8000)  |
| &#128270; | auto\_job| varchar(8000)  |
| &#128270; | setupgroup| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | mfg\_supply\_switching\_active| int  |
| &#128270; | time\_fence\_rule| int  |
| &#128270; | time\_fence\_value| float(53)  |
| &#128270; | earliest\_planned\_po\_receipt| datetime2(26)  |
| &#128270; | use\_reorder\_point| int  |
| &#128270; | reorder\_point| decimal(19,8)  |
| &#128270; | fixed\_order\_qty| decimal(19,8)  |
| &#128270; | unit\_insurance\_cost| decimal(20,8)  |
| &#128270; | unit\_loc\_frt\_cost| decimal(20,8)  |
| &#128270; | cur\_insurance\_cost| decimal(20,8)  |
| &#128270; | cur\_loc\_frt\_cost| decimal(20,8)  |
| &#128270; | tax\_free\_matl| int  |
| &#128270; | tax\_free\_days| int  |
| &#128270; | safety\_stock\_percent| decimal(3,1)  |
| &#128270; | tariff\_classification| varchar(8000)  |
| &#128270; | lowdate| datetime2(26)  |
| &#128270; | rcpt\_rqmt| varchar(8000)  |
| &#128270; | active\_for\_data\_integration| int  |
| &#128270; | rcvd\_over\_po\_qty\_tolerance| decimal(7,4)  |
| &#128270; | rcvd\_under\_po\_qty\_tolerance| decimal(7,4)  |
| &#128270; | include\_in\_net\_change\_planning| int  |
| &#128270; | kit| int  |
| &#128270; | print\_kit\_components| int  |
| &#128270; | safety\_stock\_rule| int  |
| &#128270; | show\_in\_drop\_down\_list| int  |
| &#128270; | controlled\_by\_external\_ics| int  |
| &#128270; | inventory\_ucl\_tolerance| decimal(7,4)  |
| &#128270; | inventory\_lcl\_tolerance| decimal(7,4)  |
| &#128270; | separation\_attribute| varchar(8000)  |
| &#128270; | batch\_release\_attribute1| float(53)  |
| &#128270; | batch\_release\_attribute2| float(53)  |
| &#128270; | batch\_release\_attribute3| float(53)  |
| &#128270; | active\_for\_customer\_portal| int  |
| &#128270; | featured| int  |
| &#128270; | top\_seller| int  |
| &#128270; | overview| varchar(8000)  |
| &#128270; | preassign\_lots| int  |
| &#128270; | preassign\_serials| int  |
| &#128270; | dimension\_group| varchar(8000)  |
| &#128270; | lot\_attr\_group| varchar(8000)  |
| &#128270; | track\_pieces| int  |
| &#128270; | bom\_last\_import\_date| datetime2(26)  |
| &#128270; | save\_current\_rev\_upon\_bom\_import| int  |
| &#128270; | nafta\_pref\_crit| varchar(8000)  |
| &#128270; | subject\_to\_nafta\_rvc| int  |
| &#128270; | producer| int  |
| &#128270; | nafta\_country\_of\_origin| varchar(8000)  |
| &#128270; | must\_use\_future\_rcpts\_before\_pln| int  |
| &#128270; | portal\_pricing\_site| varchar(8000)  |
| &#128270; | portal\_pricing\_enabled| int  |
| &#128270; | subject\_to\_excise\_tax| int  |
| &#128270; | excise\_tax\_percent| decimal(4,2)  |
| &#128270; | freight\_amt| decimal(20,8)  |
| &#128270; | item\_content| int  |
| &#128270; | estimated\_matl\_use\_up\_date| datetime2(26)  |
| &#128270; | last\_matl\_use\_up\_report\_date| datetime2(26)  |
| &#128270; | pp\_length\_linear\_dimension| decimal(20,8)  |
| &#128270; | pp\_width\_linear\_dimension| decimal(20,8)  |
| &#128270; | pp\_height\_linear\_dimension| decimal(20,8)  |
| &#128270; | pp\_linear\_dimension\_u\_m| varchar(8000)  |
| &#128270; | pp\_density| decimal(23,8)  |
| &#128270; | pp\_density\_u\_m| varchar(8000)  |
| &#128270; | pp\_area| decimal(23,8)  |
| &#128270; | pp\_area\_u\_m| varchar(8000)  |
| &#128270; | pp\_bulk\_mass| decimal(11,5)  |
| &#128270; | pp\_bulk\_mass\_u\_m| varchar(8000)  |
| &#128270; | pp\_ream\_mass| decimal(11,5)  |
| &#128270; | pp\_ream\_mass\_u\_m| varchar(8000)  |
| &#128270; | pp\_grade| int  |
| &#128270; | pp\_abnormal\_size| int  |
| &#128270; | pp\_paper\_mass\_basis| varchar(8000)  |
| &#128270; | charge\_item| int  |
| &#128270; | pull\_up\_safety\_stock\_rule| int  |
| &#128270; | pull\_up\_safety\_stock\_value| float(53)  |
| &#128270; | commodity\_jurisdiction| varchar(8000)  |
| &#128270; | eccn\_usml\_value| varchar(8000)  |
| &#128270; | export\_compliance\_program| varchar(8000)  |
| &#128270; | sched\_b\_num| varchar(8000)  |
| &#128270; | hts\_code| varchar(8000)  |
| &#128270; | country| varchar(8000)  |
| &#128270; | fcst\_bom\_supply\_flag| int  |
| &#128270; | allow\_on\_pick\_list| int  |
| &#128270; | auto\_job\_for\_external\_order| int  |
| &#128270; | auto\_create\_for\_config| varchar(8000)  |
| &#128270; | auto\_create\_for\_config\_external\_order| int  |
| &#128270; | cn\_item\_tax\_category| varchar(8000)  |
| &#128270; | taxed\_matl| int  |
| &#128270; | length| decimal(19,8)  |
| &#128270; | width| decimal(19,8)  |
| &#128270; | height| decimal(19,8)  |
| &#128270; | dimension\_u\_m| varchar(8000)  |
| &#128270; | package\_type| varchar(8000)  |
| &#128270; | package\_type\_max\_qty| decimal(19,8)  |
| &#128270; | hazard| int  |
| &#128270; | shipping\_name| varchar(8000)  |
| &#128270; | un\_num| varchar(8000)  |
| &#128270; | hazardous\_matl\_package\_group| varchar(8000)  |
| &#128270; | hazardous\_matl\_class| varchar(8000)  |
| &#128270; | hazmat\_contact| varchar(8000)  |
| &#128270; | hazmat\_contact\_phone| varchar(8000)  |
| &#128270; | hazmat\_placard\_required| int  |
| &#128270; | national\_motor\_freight\_class| varchar(8000)  |
| &#128270; | freight\_class| varchar(8000)  |
| &#128270; | active\_for\_anonymization| int  |
| &#128270; | ready\_mode| varchar(8000)  |
| &#128270; | uf\_bom\_comp| varchar(8000)  |
| &#128270; | uf\_bom\_ini| varchar(8000)  |
| &#128270; | uf\_bom\_status| varchar(8000)  |
| &#128270; | uf\_budget\_pence| decimal(15,4)  |
| &#128270; | uf\_cur\_u\_cost| decimal(20,8)  |
| &#128270; | uf\_drawn\_comp| varchar(8000)  |
| &#128270; | uf\_drawn\_ini| varchar(8000)  |
| &#128270; | uf\_inv\_type| varchar(8000)  |
| &#128270; | uf\_item\_volume| decimal(8,4)  |
| &#128270; | uf\_m2| decimal(15,4)  |
| &#128270; | uf\_one\_piece\_route| int  |
| &#128270; | uf\_prog\_ini| varchar(8000)  |
| &#128270; | uf\_program\_comp| varchar(8000)  |
| &#128270; | uf\_prv\_mfg| decimal(20,8)  |
| &#128270; | uf\_prv\_pur| decimal(20,8)  |
| &#128270; | uf\_prv\_sold| decimal(20,8)  |
| &#128270; | uf\_prv\_used| decimal(20,8)  |
| &#128270; | uf\_query| varchar(8000)  |
| &#128270; | uf\_radbend| varchar(8000)  |
| &#128270; | uf\_rad\_bend\_ini| varchar(8000)  |
| &#128270; | uf\_rating| varchar(8000)  |
| &#128270; | uf\_reserved| varchar(8000)  |
| &#128270; | uf\_sage\_no| varchar(8000)  |
| &#128270; | uf\_standard| varchar(8000)  |
| &#128270; | uf\_superseded| varchar(8000)  |
| &#128270; | uf\_tile\_label| varchar(8000)  |
| &#128270; | uf\_tooling| int  |
| &#128270; | uf\_ruleset| varchar(8000)  |
| &#128270; | uf\_generic\_item| int  |
| &#128270; | uf\_acoustic| varchar(8000)  |
| &#128270; | uf\_additional\_description| varchar(8000)  |
| &#128270; | uf\_angle| varchar(8000)  |
| &#128270; | uf\_aperture\_border| varchar(8000)  |
| &#128270; | uf\_aperture\_flange\_configuration\_a| varchar(8000)  |
| &#128270; | uf\_aperture\_length| varchar(8000)  |
| &#128270; | uf\_aperture\_offset| varchar(8000)  |
| &#128270; | uf\_aperture\_position| varchar(8000)  |
| &#128270; | uf\_aperture\_size| varchar(8000)  |
| &#128270; | uf\_aperture\_type| varchar(8000)  |
| &#128270; | uf\_aperture\_width| varchar(8000)  |
| &#128270; | uf\_architrave| varchar(8000)  |
| &#128270; | uf\_assembled| varchar(8000)  |
| &#128270; | uf\_average\_selling\_price| decimal(8,2)  |
| &#128270; | uf\_birdsmouth\_detail| varchar(8000)  |
| &#128270; | uf\_bom\_ecn| varchar(8000)  |
| &#128270; | uf\_borders\_a| varchar(8000)  |
| &#128270; | uf\_borders\_b| varchar(8000)  |
| &#128270; | uf\_borders\_c| varchar(8000)  |
| &#128270; | uf\_borders\_d| varchar(8000)  |
| &#128270; | uf\_borders\_e| varchar(8000)  |
| &#128270; | uf\_borders\_f| varchar(8000)  |
| &#128270; | uf\_borders\_g| varchar(8000)  |
| &#128270; | uf\_borders\_h| varchar(8000)  |
| &#128270; | uf\_box\_qty| varchar(8000)  |
| &#128270; | uf\_cat\_ref| varchar(8000)  |
| &#128270; | uf\_core\_type| varchar(8000)  |
| &#128270; | uf\_depth| int  |
| &#128270; | uf\_diameter\_offset| varchar(8000)  |
| &#128270; | uf\_diameter\_size| varchar(8000)  |
| &#128270; | uf\_door\_cat| varchar(8000)  |
| &#128270; | uf\_door\_leaf\_type| varchar(8000)  |
| &#128270; | uf\_door\_type| varchar(8000)  |
| &#128270; | uf\_dr\_frm\_config| varchar(8000)  |
| &#128270; | uf\_driver\_type| varchar(8000)  |
| &#128270; | uf\_edge\_config| varchar(8000)  |
| &#128270; | uf\_edgeor\_grid\_size| varchar(8000)  |
| &#128270; | uf\_end\_cap\_type| varchar(8000)  |
| &#128270; | uf\_frame\_finish| varchar(8000)  |
| &#128270; | uf\_frame\_type| varchar(8000)  |
| &#128270; | uf\_gasket| varchar(8000)  |
| &#128270; | uf\_gauge| varchar(8000)  |
| &#128270; | uf\_glaz\_pckt| varchar(8000)  |
| &#128270; | uf\_handing| varchar(8000)  |
| &#128270; | uf\_hinges| varchar(8000)  |
| &#128270; | uf\_insulation\_type| varchar(8000)  |
| &#128270; | uf\_intu\_type| varchar(8000)  |
| &#128270; | uf\_ironmongery| varchar(8000)  |
| &#128270; | uf\_issue\_no| varchar(8000)  |
| &#128270; | uf\_issue\_no\_d| varchar(8000)  |
| &#128270; | uf\_led\_type| varchar(8000)  |
| &#128270; | uf\_length| varchar(8000)  |
| &#128270; | uf\_lens\_type| varchar(8000)  |
| &#128270; | uf\_light\_mod\_type| varchar(8000)  |
| &#128270; | uf\_lipping| int  |
| &#128270; | uf\_long\_description| varchar(8000)  |
| &#128270; | uf\_manufacturer| varchar(8000)  |
| &#128270; | uf\_material\_type| varchar(8000)  |
| &#128270; | uf\_module| varchar(8000)  |
| &#128270; | uf\_module\_length| varchar(8000)  |
| &#128270; | uf\_module\_width| varchar(8000)  |
| &#128270; | uf\_nominal\_border| varchar(8000)  |
| &#128270; | uf\_non\_fire\_rated| varchar(8000)  |
| &#128270; | uf\_no\_of\_bends| varchar(8000)  |
| &#128270; | uf\_old\_system\_part\_number| varchar(8000)  |
| &#128270; | uf\_over\_panel\_h| varchar(8000)  |
| &#128270; | uf\_pad\_density| varchar(8000)  |
| &#128270; | uf\_pad\_depth| varchar(8000)  |
| &#128270; | uf\_paint| varchar(8000)  |
| &#128270; | uf\_paint\_application| varchar(8000)  |
| &#128270; | uf\_partion\_system\_type| varchar(8000)  |
| &#128270; | uf\_partit\_glaze| varchar(8000)  |
| &#128270; | uf\_partition| varchar(8000)  |
| &#128270; | uf\_partition\_type| varchar(8000)  |
| &#128270; | uf\_perf| varchar(8000)  |
| &#128270; | uf\_periphery| varchar(8000)  |
| &#128270; | uf\_product\_type1| varchar(8000)  |
| &#128270; | uf\_profile\_type| varchar(8000)  |
| &#128270; | uf\_rdg\_drawing| int  |
| &#128270; | uf\_route| varchar(8000)  |
| &#128270; | uf\_row\_tooling| varchar(8000)  |
| &#128270; | uf\_shipping| varchar(8000)  |
| &#128270; | uf\_site| varchar(8000)  |
| &#128270; | uf\_slave\_leaf\_w| varchar(8000)  |
| &#128270; | uf\_snap\_infill| varchar(8000)  |
| &#128270; | uf\_strike\_plate| varchar(8000)  |
| &#128270; | uf\_sustainability| varchar(8000)  |
| &#128270; | uf\_swing\_type| varchar(8000)  |
| &#128270; | uf\_sys\_thickness| varchar(8000)  |
| &#128270; | uf\_sys\_type| varchar(8000)  |
| &#128270; | uf\_template\_no| varchar(8000)  |
| &#128270; | uf\_thickness| decimal(8,1)  |
| &#128270; | uf\_tile\_flange\_configuration\_a| varchar(8000)  |
| &#128270; | uf\_veneer| varchar(8000)  |
| &#128270; | uf\_vp\_bead\_type| varchar(8000)  |
| &#128270; | uf\_vph\_lower| varchar(8000)  |
| &#128270; | uf\_vp\_length| varchar(8000)  |
| &#128270; | uf\_vp\_position| varchar(8000)  |
| &#128270; | uf\_vp\_qty\_per\_leaf| varchar(8000)  |
| &#128270; | uf\_vp\_shape| varchar(8000)  |
| &#128270; | uf\_vp\_spacing| varchar(8000)  |
| &#128270; | uf\_vp\_type| varchar(8000)  |
| &#128270; | uf\_vp\_width| varchar(8000)  |
| &#128270; | uf\_width| varchar(8000)  |
| &#128270; | uf\_salesforce\_id| varchar(8000)  |
| &#128270; | sas\_drawing\_vr\_location| varchar(8000)  |
| &#128270; | attr\_group| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON qty\_allocjob|
| &#128270;  | ClusteredIndex | ON u\_m|
| &#128270;  | ClusteredIndex | ON lead\_time|
| &#128270;  | ClusteredIndex | ON lot\_size|
| &#128270;  | ClusteredIndex | ON qty\_used\_ytd|
| &#128270;  | ClusteredIndex | ON qty\_mfg\_ytd|
| &#128270;  | ClusteredIndex | ON abc\_code|
| &#128270;  | ClusteredIndex | ON drawing\_nbr|
| &#128270;  | ClusteredIndex | ON product\_code|
| &#128270;  | ClusteredIndex | ON p\_m\_t\_code|
| &#128270;  | ClusteredIndex | ON cost\_method|
| &#128270;  | ClusteredIndex | ON lst\_lot\_size|
| &#128270;  | ClusteredIndex | ON unit\_cost|
| &#128270;  | ClusteredIndex | ON lst\_u\_cost|
| &#128270;  | ClusteredIndex | ON avg\_u\_cost|
| &#128270;  | ClusteredIndex | ON job|
| &#128270;  | ClusteredIndex | ON suffix|
| &#128270;  | ClusteredIndex | ON stocked|
| &#128270;  | ClusteredIndex | ON matl\_type|
| &#128270;  | ClusteredIndex | ON family\_code|
| &#128270;  | ClusteredIndex | ON low\_level|
| &#128270;  | ClusteredIndex | ON last\_inv|
| &#128270;  | ClusteredIndex | ON days\_supply|
| &#128270;  | ClusteredIndex | ON order\_min|
| &#128270;  | ClusteredIndex | ON order\_mult|
| &#128270;  | ClusteredIndex | ON plan\_code|
| &#128270;  | ClusteredIndex | ON mps\_flag|
| &#128270;  | ClusteredIndex | ON accept\_req|
| &#128270;  | ClusteredIndex | ON change\_date|
| &#128270;  | ClusteredIndex | ON revision|
| &#128270;  | ClusteredIndex | ON phantom\_flag|
| &#128270;  | ClusteredIndex | ON plan\_flag|
| &#128270;  | ClusteredIndex | ON paper\_time|
| &#128270;  | ClusteredIndex | ON dock\_time|
| &#128270;  | ClusteredIndex | ON asm\_setup|
| &#128270;  | ClusteredIndex | ON asm\_run|
| &#128270;  | ClusteredIndex | ON asm\_matl|
| &#128270;  | ClusteredIndex | ON asm\_tool|
| &#128270;  | ClusteredIndex | ON asm\_fixture|
| &#128270;  | ClusteredIndex | ON asm\_other|
| &#128270;  | ClusteredIndex | ON asm\_fixed|
| &#128270;  | ClusteredIndex | ON asm\_var|
| &#128270;  | ClusteredIndex | ON asm\_outside|
| &#128270;  | ClusteredIndex | ON comp\_setup|
| &#128270;  | ClusteredIndex | ON comp\_run|
| &#128270;  | ClusteredIndex | ON comp\_matl|
| &#128270;  | ClusteredIndex | ON comp\_tool|
| &#128270;  | ClusteredIndex | ON comp\_fixture|
| &#128270;  | ClusteredIndex | ON comp\_other|
| &#128270;  | ClusteredIndex | ON comp\_fixed|
| &#128270;  | ClusteredIndex | ON comp\_var|
| &#128270;  | ClusteredIndex | ON comp\_outside|
| &#128270;  | ClusteredIndex | ON sub\_matl|
| &#128270;  | ClusteredIndex | ON shrink\_fact|
| &#128270;  | ClusteredIndex | ON alt\_item|
| &#128270;  | ClusteredIndex | ON unit\_weight|
| &#128270;  | ClusteredIndex | ON weight\_units|
| &#128270;  | ClusteredIndex | ON charfld4|
| &#128270;  | ClusteredIndex | ON cur\_u\_cost|
| &#128270;  | ClusteredIndex | ON feat\_type|
| &#128270;  | ClusteredIndex | ON var\_lead|
| &#128270;  | ClusteredIndex | ON feat\_str|
| &#128270;  | ClusteredIndex | ON next\_config|
| &#128270;  | ClusteredIndex | ON feat\_templ|
| &#128270;  | ClusteredIndex | ON backflush|
| &#128270;  | ClusteredIndex | ON charfld1|
| &#128270;  | ClusteredIndex | ON charfld2|
| &#128270;  | ClusteredIndex | ON charfld3|
| &#128270;  | ClusteredIndex | ON decifld1|
| &#128270;  | ClusteredIndex | ON decifld2|
| &#128270;  | ClusteredIndex | ON decifld3|
| &#128270;  | ClusteredIndex | ON logifld|
| &#128270;  | ClusteredIndex | ON datefld|
| &#128270;  | ClusteredIndex | ON track\_ecn|
| &#128270;  | ClusteredIndex | ON u\_ws\_price|
| &#128270;  | ClusteredIndex | ON comm\_code|
| &#128270;  | ClusteredIndex | ON origin|
| &#128270;  | ClusteredIndex | ON unit\_mat\_cost|
| &#128270;  | ClusteredIndex | ON unit\_duty\_cost|
| &#128270;  | ClusteredIndex | ON unit\_freight\_cost|
| &#128270;  | ClusteredIndex | ON unit\_brokerage\_cost|
| &#128270;  | ClusteredIndex | ON cur\_mat\_cost|
| &#128270;  | ClusteredIndex | ON cur\_duty\_cost|
| &#128270;  | ClusteredIndex | ON cur\_freight\_cost|
| &#128270;  | ClusteredIndex | ON cur\_brokerage\_cost|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON bflush\_loc|
| &#128270;  | ClusteredIndex | ON reservable|
| &#128270;  | ClusteredIndex | ON shelf\_life|
| &#128270;  | ClusteredIndex | ON lot\_prefix|
| &#128270;  | ClusteredIndex | ON serial\_prefix|
| &#128270;  | ClusteredIndex | ON serial\_length|
| &#128270;  | ClusteredIndex | ON issue\_by|
| &#128270;  | ClusteredIndex | ON serial\_tracked|
| &#128270;  | ClusteredIndex | ON lot\_tracked|
| &#128270;  | ClusteredIndex | ON cost\_type|
| &#128270;  | ClusteredIndex | ON matl\_cost|
| &#128270;  | ClusteredIndex | ON lbr\_cost|
| &#128270;  | ClusteredIndex | ON fovhd\_cost|
| &#128270;  | ClusteredIndex | ON vovhd\_cost|
| &#128270;  | ClusteredIndex | ON out\_cost|
| &#128270;  | ClusteredIndex | ON cur\_matl\_cost|
| &#128270;  | ClusteredIndex | ON cur\_lbr\_cost|
| &#128270;  | ClusteredIndex | ON cur\_fovhd\_cost|
| &#128270;  | ClusteredIndex | ON cur\_vovhd\_cost|
| &#128270;  | ClusteredIndex | ON cur\_out\_cost|
| &#128270;  | ClusteredIndex | ON avg\_matl\_cost|
| &#128270;  | ClusteredIndex | ON avg\_lbr\_cost|
| &#128270;  | ClusteredIndex | ON avg\_fovhd\_cost|
| &#128270;  | ClusteredIndex | ON avg\_vovhd\_cost|
| &#128270;  | ClusteredIndex | ON avg\_out\_cost|
| &#128270;  | ClusteredIndex | ON prod\_type|
| &#128270;  | ClusteredIndex | ON rate\_per\_day|
| &#128270;  | ClusteredIndex | ON mps\_plan\_fence|
| &#128270;  | ClusteredIndex | ON pass\_req|
| &#128270;  | ClusteredIndex | ON lot\_gen\_exp|
| &#128270;  | ClusteredIndex | ON supply\_site|
| &#128270;  | ClusteredIndex | ON prod\_mix|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON status\_chg\_user\_code|
| &#128270;  | ClusteredIndex | ON chg\_date|
| &#128270;  | ClusteredIndex | ON reason\_code|
| &#128270;  | ClusteredIndex | ON supply\_whse|
| &#128270;  | ClusteredIndex | ON due\_period|
| &#128270;  | ClusteredIndex | ON order\_max|
| &#128270;  | ClusteredIndex | ON mrp\_part|
| &#128270;  | ClusteredIndex | ON infinite\_part|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON supply\_tolerance\_hrs|
| &#128270;  | ClusteredIndex | ON exp\_lead\_time|
| &#128270;  | ClusteredIndex | ON var\_exp\_lead|
| &#128270;  | ClusteredIndex | ON buyer|
| &#128270;  | ClusteredIndex | ON order\_configurable|
| &#128270;  | ClusteredIndex | ON job\_configurable|
| &#128270;  | ClusteredIndex | ON cfg\_model|
| &#128270;  | ClusteredIndex | ON auto\_job|
| &#128270;  | ClusteredIndex | ON setupgroup|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON mfg\_supply\_switching\_active|
| &#128270;  | ClusteredIndex | ON time\_fence\_rule|
| &#128270;  | ClusteredIndex | ON time\_fence\_value|
| &#128270;  | ClusteredIndex | ON earliest\_planned\_po\_receipt|
| &#128270;  | ClusteredIndex | ON use\_reorder\_point|
| &#128270;  | ClusteredIndex | ON reorder\_point|
| &#128270;  | ClusteredIndex | ON fixed\_order\_qty|
| &#128270;  | ClusteredIndex | ON unit\_insurance\_cost|
| &#128270;  | ClusteredIndex | ON unit\_loc\_frt\_cost|
| &#128270;  | ClusteredIndex | ON cur\_insurance\_cost|
| &#128270;  | ClusteredIndex | ON cur\_loc\_frt\_cost|
| &#128270;  | ClusteredIndex | ON tax\_free\_matl|
| &#128270;  | ClusteredIndex | ON tax\_free\_days|
| &#128270;  | ClusteredIndex | ON safety\_stock\_percent|
| &#128270;  | ClusteredIndex | ON tariff\_classification|
| &#128270;  | ClusteredIndex | ON lowdate|
| &#128270;  | ClusteredIndex | ON rcpt\_rqmt|
| &#128270;  | ClusteredIndex | ON active\_for\_data\_integration|
| &#128270;  | ClusteredIndex | ON rcvd\_over\_po\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON rcvd\_under\_po\_qty\_tolerance|
| &#128270;  | ClusteredIndex | ON include\_in\_net\_change\_planning|
| &#128270;  | ClusteredIndex | ON kit|
| &#128270;  | ClusteredIndex | ON print\_kit\_components|
| &#128270;  | ClusteredIndex | ON safety\_stock\_rule|
| &#128270;  | ClusteredIndex | ON show\_in\_drop\_down\_list|
| &#128270;  | ClusteredIndex | ON controlled\_by\_external\_ics|
| &#128270;  | ClusteredIndex | ON inventory\_ucl\_tolerance|
| &#128270;  | ClusteredIndex | ON inventory\_lcl\_tolerance|
| &#128270;  | ClusteredIndex | ON separation\_attribute|
| &#128270;  | ClusteredIndex | ON batch\_release\_attribute1|
| &#128270;  | ClusteredIndex | ON batch\_release\_attribute2|
| &#128270;  | ClusteredIndex | ON batch\_release\_attribute3|
| &#128270;  | ClusteredIndex | ON active\_for\_customer\_portal|
| &#128270;  | ClusteredIndex | ON featured|
| &#128270;  | ClusteredIndex | ON top\_seller|
| &#128270;  | ClusteredIndex | ON overview|
| &#128270;  | ClusteredIndex | ON preassign\_lots|
| &#128270;  | ClusteredIndex | ON preassign\_serials|
| &#128270;  | ClusteredIndex | ON dimension\_group|
| &#128270;  | ClusteredIndex | ON lot\_attr\_group|
| &#128270;  | ClusteredIndex | ON track\_pieces|
| &#128270;  | ClusteredIndex | ON bom\_last\_import\_date|
| &#128270;  | ClusteredIndex | ON save\_current\_rev\_upon\_bom\_import|
| &#128270;  | ClusteredIndex | ON nafta\_pref\_crit|
| &#128270;  | ClusteredIndex | ON subject\_to\_nafta\_rvc|
| &#128270;  | ClusteredIndex | ON producer|
| &#128270;  | ClusteredIndex | ON nafta\_country\_of\_origin|
| &#128270;  | ClusteredIndex | ON must\_use\_future\_rcpts\_before\_pln|
| &#128270;  | ClusteredIndex | ON portal\_pricing\_site|
| &#128270;  | ClusteredIndex | ON portal\_pricing\_enabled|
| &#128270;  | ClusteredIndex | ON subject\_to\_excise\_tax|
| &#128270;  | ClusteredIndex | ON excise\_tax\_percent|
| &#128270;  | ClusteredIndex | ON freight\_amt|
| &#128270;  | ClusteredIndex | ON item\_content|
| &#128270;  | ClusteredIndex | ON estimated\_matl\_use\_up\_date|
| &#128270;  | ClusteredIndex | ON last\_matl\_use\_up\_report\_date|
| &#128270;  | ClusteredIndex | ON pp\_length\_linear\_dimension|
| &#128270;  | ClusteredIndex | ON pp\_width\_linear\_dimension|
| &#128270;  | ClusteredIndex | ON pp\_height\_linear\_dimension|
| &#128270;  | ClusteredIndex | ON pp\_linear\_dimension\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_density|
| &#128270;  | ClusteredIndex | ON pp\_density\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_area|
| &#128270;  | ClusteredIndex | ON pp\_area\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_bulk\_mass|
| &#128270;  | ClusteredIndex | ON pp\_bulk\_mass\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_ream\_mass|
| &#128270;  | ClusteredIndex | ON pp\_ream\_mass\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_grade|
| &#128270;  | ClusteredIndex | ON pp\_abnormal\_size|
| &#128270;  | ClusteredIndex | ON pp\_paper\_mass\_basis|
| &#128270;  | ClusteredIndex | ON charge\_item|
| &#128270;  | ClusteredIndex | ON pull\_up\_safety\_stock\_rule|
| &#128270;  | ClusteredIndex | ON pull\_up\_safety\_stock\_value|
| &#128270;  | ClusteredIndex | ON commodity\_jurisdiction|
| &#128270;  | ClusteredIndex | ON eccn\_usml\_value|
| &#128270;  | ClusteredIndex | ON export\_compliance\_program|
| &#128270;  | ClusteredIndex | ON sched\_b\_num|
| &#128270;  | ClusteredIndex | ON hts\_code|
| &#128270;  | ClusteredIndex | ON country|
| &#128270;  | ClusteredIndex | ON fcst\_bom\_supply\_flag|
| &#128270;  | ClusteredIndex | ON allow\_on\_pick\_list|
| &#128270;  | ClusteredIndex | ON auto\_job\_for\_external\_order|
| &#128270;  | ClusteredIndex | ON auto\_create\_for\_config|
| &#128270;  | ClusteredIndex | ON auto\_create\_for\_config\_external\_order|
| &#128270;  | ClusteredIndex | ON cn\_item\_tax\_category|
| &#128270;  | ClusteredIndex | ON taxed\_matl|
| &#128270;  | ClusteredIndex | ON length|
| &#128270;  | ClusteredIndex | ON width|
| &#128270;  | ClusteredIndex | ON height|
| &#128270;  | ClusteredIndex | ON dimension\_u\_m|
| &#128270;  | ClusteredIndex | ON package\_type|
| &#128270;  | ClusteredIndex | ON package\_type\_max\_qty|
| &#128270;  | ClusteredIndex | ON hazard|
| &#128270;  | ClusteredIndex | ON shipping\_name|
| &#128270;  | ClusteredIndex | ON un\_num|
| &#128270;  | ClusteredIndex | ON hazardous\_matl\_package\_group|
| &#128270;  | ClusteredIndex | ON hazardous\_matl\_class|
| &#128270;  | ClusteredIndex | ON hazmat\_contact|
| &#128270;  | ClusteredIndex | ON hazmat\_contact\_phone|
| &#128270;  | ClusteredIndex | ON hazmat\_placard\_required|
| &#128270;  | ClusteredIndex | ON national\_motor\_freight\_class|
| &#128270;  | ClusteredIndex | ON freight\_class|
| &#128270;  | ClusteredIndex | ON active\_for\_anonymization|
| &#128270;  | ClusteredIndex | ON ready\_mode|
| &#128270;  | ClusteredIndex | ON uf\_bom\_comp|
| &#128270;  | ClusteredIndex | ON uf\_bom\_ini|
| &#128270;  | ClusteredIndex | ON uf\_bom\_status|
| &#128270;  | ClusteredIndex | ON uf\_budget\_pence|
| &#128270;  | ClusteredIndex | ON uf\_cur\_u\_cost|
| &#128270;  | ClusteredIndex | ON uf\_drawn\_comp|
| &#128270;  | ClusteredIndex | ON uf\_drawn\_ini|
| &#128270;  | ClusteredIndex | ON uf\_inv\_type|
| &#128270;  | ClusteredIndex | ON uf\_item\_volume|
| &#128270;  | ClusteredIndex | ON uf\_m2|
| &#128270;  | ClusteredIndex | ON uf\_one\_piece\_route|
| &#128270;  | ClusteredIndex | ON uf\_prog\_ini|
| &#128270;  | ClusteredIndex | ON uf\_program\_comp|
| &#128270;  | ClusteredIndex | ON uf\_prv\_mfg|
| &#128270;  | ClusteredIndex | ON uf\_prv\_pur|
| &#128270;  | ClusteredIndex | ON uf\_prv\_sold|
| &#128270;  | ClusteredIndex | ON uf\_prv\_used|
| &#128270;  | ClusteredIndex | ON uf\_query|
| &#128270;  | ClusteredIndex | ON uf\_radbend|
| &#128270;  | ClusteredIndex | ON uf\_rad\_bend\_ini|
| &#128270;  | ClusteredIndex | ON uf\_rating|
| &#128270;  | ClusteredIndex | ON uf\_reserved|
| &#128270;  | ClusteredIndex | ON uf\_sage\_no|
| &#128270;  | ClusteredIndex | ON uf\_standard|
| &#128270;  | ClusteredIndex | ON uf\_superseded|
| &#128270;  | ClusteredIndex | ON uf\_tile\_label|
| &#128270;  | ClusteredIndex | ON uf\_tooling|
| &#128270;  | ClusteredIndex | ON uf\_ruleset|
| &#128270;  | ClusteredIndex | ON uf\_generic\_item|
| &#128270;  | ClusteredIndex | ON uf\_acoustic|
| &#128270;  | ClusteredIndex | ON uf\_additional\_description|
| &#128270;  | ClusteredIndex | ON uf\_angle|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_border|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_flange\_configuration\_a|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_length|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_offset|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_position|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_size|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_type|
| &#128270;  | ClusteredIndex | ON uf\_aperture\_width|
| &#128270;  | ClusteredIndex | ON uf\_architrave|
| &#128270;  | ClusteredIndex | ON uf\_assembled|
| &#128270;  | ClusteredIndex | ON uf\_average\_selling\_price|
| &#128270;  | ClusteredIndex | ON uf\_birdsmouth\_detail|
| &#128270;  | ClusteredIndex | ON uf\_bom\_ecn|
| &#128270;  | ClusteredIndex | ON uf\_borders\_a|
| &#128270;  | ClusteredIndex | ON uf\_borders\_b|
| &#128270;  | ClusteredIndex | ON uf\_borders\_c|
| &#128270;  | ClusteredIndex | ON uf\_borders\_d|
| &#128270;  | ClusteredIndex | ON uf\_borders\_e|
| &#128270;  | ClusteredIndex | ON uf\_borders\_f|
| &#128270;  | ClusteredIndex | ON uf\_borders\_g|
| &#128270;  | ClusteredIndex | ON uf\_borders\_h|
| &#128270;  | ClusteredIndex | ON uf\_box\_qty|
| &#128270;  | ClusteredIndex | ON uf\_cat\_ref|
| &#128270;  | ClusteredIndex | ON uf\_core\_type|
| &#128270;  | ClusteredIndex | ON uf\_depth|
| &#128270;  | ClusteredIndex | ON uf\_diameter\_offset|
| &#128270;  | ClusteredIndex | ON uf\_diameter\_size|
| &#128270;  | ClusteredIndex | ON uf\_door\_cat|
| &#128270;  | ClusteredIndex | ON uf\_door\_leaf\_type|
| &#128270;  | ClusteredIndex | ON uf\_door\_type|
| &#128270;  | ClusteredIndex | ON uf\_dr\_frm\_config|
| &#128270;  | ClusteredIndex | ON uf\_driver\_type|
| &#128270;  | ClusteredIndex | ON uf\_edge\_config|
| &#128270;  | ClusteredIndex | ON uf\_edgeor\_grid\_size|
| &#128270;  | ClusteredIndex | ON uf\_end\_cap\_type|
| &#128270;  | ClusteredIndex | ON uf\_frame\_finish|
| &#128270;  | ClusteredIndex | ON uf\_frame\_type|
| &#128270;  | ClusteredIndex | ON uf\_gasket|
| &#128270;  | ClusteredIndex | ON uf\_gauge|
| &#128270;  | ClusteredIndex | ON uf\_glaz\_pckt|
| &#128270;  | ClusteredIndex | ON uf\_handing|
| &#128270;  | ClusteredIndex | ON uf\_hinges|
| &#128270;  | ClusteredIndex | ON uf\_insulation\_type|
| &#128270;  | ClusteredIndex | ON uf\_intu\_type|
| &#128270;  | ClusteredIndex | ON uf\_ironmongery|
| &#128270;  | ClusteredIndex | ON uf\_issue\_no|
| &#128270;  | ClusteredIndex | ON uf\_issue\_no\_d|
| &#128270;  | ClusteredIndex | ON uf\_led\_type|
| &#128270;  | ClusteredIndex | ON uf\_length|
| &#128270;  | ClusteredIndex | ON uf\_lens\_type|
| &#128270;  | ClusteredIndex | ON uf\_light\_mod\_type|
| &#128270;  | ClusteredIndex | ON uf\_lipping|
| &#128270;  | ClusteredIndex | ON uf\_long\_description|
| &#128270;  | ClusteredIndex | ON uf\_manufacturer|
| &#128270;  | ClusteredIndex | ON uf\_material\_type|
| &#128270;  | ClusteredIndex | ON uf\_module|
| &#128270;  | ClusteredIndex | ON uf\_module\_length|
| &#128270;  | ClusteredIndex | ON uf\_module\_width|
| &#128270;  | ClusteredIndex | ON uf\_nominal\_border|
| &#128270;  | ClusteredIndex | ON uf\_non\_fire\_rated|
| &#128270;  | ClusteredIndex | ON uf\_no\_of\_bends|
| &#128270;  | ClusteredIndex | ON uf\_old\_system\_part\_number|
| &#128270;  | ClusteredIndex | ON uf\_over\_panel\_h|
| &#128270;  | ClusteredIndex | ON uf\_pad\_density|
| &#128270;  | ClusteredIndex | ON uf\_pad\_depth|
| &#128270;  | ClusteredIndex | ON uf\_paint|
| &#128270;  | ClusteredIndex | ON uf\_paint\_application|
| &#128270;  | ClusteredIndex | ON uf\_partion\_system\_type|
| &#128270;  | ClusteredIndex | ON uf\_partit\_glaze|
| &#128270;  | ClusteredIndex | ON uf\_partition|
| &#128270;  | ClusteredIndex | ON uf\_partition\_type|
| &#128270;  | ClusteredIndex | ON uf\_perf|
| &#128270;  | ClusteredIndex | ON uf\_periphery|
| &#128270;  | ClusteredIndex | ON uf\_product\_type1|
| &#128270;  | ClusteredIndex | ON uf\_profile\_type|
| &#128270;  | ClusteredIndex | ON uf\_rdg\_drawing|
| &#128270;  | ClusteredIndex | ON uf\_route|
| &#128270;  | ClusteredIndex | ON uf\_row\_tooling|
| &#128270;  | ClusteredIndex | ON uf\_shipping|
| &#128270;  | ClusteredIndex | ON uf\_site|
| &#128270;  | ClusteredIndex | ON uf\_slave\_leaf\_w|
| &#128270;  | ClusteredIndex | ON uf\_snap\_infill|
| &#128270;  | ClusteredIndex | ON uf\_strike\_plate|
| &#128270;  | ClusteredIndex | ON uf\_sustainability|
| &#128270;  | ClusteredIndex | ON uf\_swing\_type|
| &#128270;  | ClusteredIndex | ON uf\_sys\_thickness|
| &#128270;  | ClusteredIndex | ON uf\_sys\_type|
| &#128270;  | ClusteredIndex | ON uf\_template\_no|
| &#128270;  | ClusteredIndex | ON uf\_thickness|
| &#128270;  | ClusteredIndex | ON uf\_tile\_flange\_configuration\_a|
| &#128270;  | ClusteredIndex | ON uf\_veneer|
| &#128270;  | ClusteredIndex | ON uf\_vp\_bead\_type|
| &#128270;  | ClusteredIndex | ON uf\_vph\_lower|
| &#128270;  | ClusteredIndex | ON uf\_vp\_length|
| &#128270;  | ClusteredIndex | ON uf\_vp\_position|
| &#128270;  | ClusteredIndex | ON uf\_vp\_qty\_per\_leaf|
| &#128270;  | ClusteredIndex | ON uf\_vp\_shape|
| &#128270;  | ClusteredIndex | ON uf\_vp\_spacing|
| &#128270;  | ClusteredIndex | ON uf\_vp\_type|
| &#128270;  | ClusteredIndex | ON uf\_vp\_width|
| &#128270;  | ClusteredIndex | ON uf\_width|
| &#128270;  | ClusteredIndex | ON uf\_salesforce\_id|
| &#128270;  | ClusteredIndex | ON sas\_drawing\_vr\_location|
| &#128270;  | ClusteredIndex | ON attr\_group|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.itemprice_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | item| varchar(8000)  |
| &#128270; | effect\_date| datetime2(26)  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | unit\_price1| decimal(20,8)  |
| &#128270; | unit\_price2| decimal(20,8)  |
| &#128270; | unit\_price3| decimal(20,8)  |
| &#128270; | unit\_price4| decimal(20,8)  |
| &#128270; | unit\_price5| decimal(20,8)  |
| &#128270; | unit\_price6| decimal(20,8)  |
| &#128270; | reprice| int  |
| &#128270; | brk\_qty\_1| decimal(19,8)  |
| &#128270; | brk\_qty\_2| decimal(19,8)  |
| &#128270; | brk\_qty\_3| decimal(19,8)  |
| &#128270; | brk\_qty\_4| decimal(19,8)  |
| &#128270; | brk\_qty\_5| decimal(19,8)  |
| &#128270; | brk\_price\_1| decimal(20,8)  |
| &#128270; | brk\_price\_2| decimal(20,8)  |
| &#128270; | brk\_price\_3| decimal(20,8)  |
| &#128270; | brk\_price\_4| decimal(20,8)  |
| &#128270; | brk\_price\_5| decimal(20,8)  |
| &#128270; | base\_code\_1| varchar(8000)  |
| &#128270; | base\_code\_2| varchar(8000)  |
| &#128270; | base\_code\_3| varchar(8000)  |
| &#128270; | base\_code\_4| varchar(8000)  |
| &#128270; | base\_code\_5| varchar(8000)  |
| &#128270; | dol\_percent\_1| varchar(8000)  |
| &#128270; | dol\_percent\_2| varchar(8000)  |
| &#128270; | dol\_percent\_3| varchar(8000)  |
| &#128270; | dol\_percent\_4| varchar(8000)  |
| &#128270; | dol\_percent\_5| varchar(8000)  |
| &#128270; | pricecode| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON effect\_date|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON unit\_price1|
| &#128270;  | ClusteredIndex | ON unit\_price2|
| &#128270;  | ClusteredIndex | ON unit\_price3|
| &#128270;  | ClusteredIndex | ON unit\_price4|
| &#128270;  | ClusteredIndex | ON unit\_price5|
| &#128270;  | ClusteredIndex | ON unit\_price6|
| &#128270;  | ClusteredIndex | ON reprice|
| &#128270;  | ClusteredIndex | ON brk\_qty\_1|
| &#128270;  | ClusteredIndex | ON brk\_qty\_2|
| &#128270;  | ClusteredIndex | ON brk\_qty\_3|
| &#128270;  | ClusteredIndex | ON brk\_qty\_4|
| &#128270;  | ClusteredIndex | ON brk\_qty\_5|
| &#128270;  | ClusteredIndex | ON brk\_price\_1|
| &#128270;  | ClusteredIndex | ON brk\_price\_2|
| &#128270;  | ClusteredIndex | ON brk\_price\_3|
| &#128270;  | ClusteredIndex | ON brk\_price\_4|
| &#128270;  | ClusteredIndex | ON brk\_price\_5|
| &#128270;  | ClusteredIndex | ON base\_code\_1|
| &#128270;  | ClusteredIndex | ON base\_code\_2|
| &#128270;  | ClusteredIndex | ON base\_code\_3|
| &#128270;  | ClusteredIndex | ON base\_code\_4|
| &#128270;  | ClusteredIndex | ON base\_code\_5|
| &#128270;  | ClusteredIndex | ON dol\_percent\_1|
| &#128270;  | ClusteredIndex | ON dol\_percent\_2|
| &#128270;  | ClusteredIndex | ON dol\_percent\_3|
| &#128270;  | ClusteredIndex | ON dol\_percent\_4|
| &#128270;  | ClusteredIndex | ON dol\_percent\_5|
| &#128270;  | ClusteredIndex | ON pricecode|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.job_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | type| varchar(8000)  |
| &#128270; | job| varchar(8000)  |
| &#128270; | suffix| int  |
| &#128270; | job\_date| datetime2(26)  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | ord\_type| varchar(8000)  |
| &#128270; | ord\_num| varchar(8000)  |
| &#128270; | ord\_line| int  |
| &#128270; | ord\_release| int  |
| &#128270; | est\_job| varchar(8000)  |
| &#128270; | est\_suf| int  |
| &#128270; | item| varchar(8000)  |
| &#128270; | qty\_released| decimal(19,8)  |
| &#128270; | qty\_complete| decimal(19,8)  |
| &#128270; | qty\_scrapped| decimal(19,8)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | lst\_trx\_date| datetime2(26)  |
| &#128270; | root\_job| varchar(8000)  |
| &#128270; | root\_suf| int  |
| &#128270; | ref\_job| varchar(8000)  |
| &#128270; | ref\_suf| int  |
| &#128270; | ref\_oper| int  |
| &#128270; | ref\_seq| int  |
| &#128270; | low\_level| int  |
| &#128270; | effect\_date| datetime2(26)  |
| &#128270; | wip\_acct| varchar(8000)  |
| &#128270; | wip\_total| decimal(23,8)  |
| &#128270; | wip\_complete| decimal(23,8)  |
| &#128270; | wip\_special| decimal(23,8)  |
| &#128270; | revision| varchar(8000)  |
| &#128270; | picked| int  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | jcb\_acct| varchar(8000)  |
| &#128270; | ps\_num| varchar(8000)  |
| &#128270; | wip\_lbr\_acct| varchar(8000)  |
| &#128270; | wip\_fovhd\_acct| varchar(8000)  |
| &#128270; | wip\_vovhd\_acct| varchar(8000)  |
| &#128270; | wip\_out\_acct| varchar(8000)  |
| &#128270; | wip\_matl\_total| decimal(23,8)  |
| &#128270; | wip\_lbr\_total| decimal(23,8)  |
| &#128270; | wip\_fovhd\_total| decimal(23,8)  |
| &#128270; | wip\_vovhd\_total| decimal(23,8)  |
| &#128270; | wip\_out\_total| decimal(23,8)  |
| &#128270; | wip\_matl\_comp| decimal(23,8)  |
| &#128270; | wip\_lbr\_comp| decimal(23,8)  |
| &#128270; | wip\_fovhd\_comp| decimal(23,8)  |
| &#128270; | wip\_vovhd\_comp| decimal(23,8)  |
| &#128270; | wip\_out\_comp| decimal(23,8)  |
| &#128270; | rollup\_date| datetime2(26)  |
| &#128270; | wip\_acct\_unit1| varchar(8000)  |
| &#128270; | wip\_acct\_unit2| varchar(8000)  |
| &#128270; | wip\_acct\_unit3| varchar(8000)  |
| &#128270; | wip\_acct\_unit4| varchar(8000)  |
| &#128270; | jcb\_acct\_unit1| varchar(8000)  |
| &#128270; | jcb\_acct\_unit2| varchar(8000)  |
| &#128270; | jcb\_acct\_unit3| varchar(8000)  |
| &#128270; | jcb\_acct\_unit4| varchar(8000)  |
| &#128270; | wip\_lbr\_acct\_unit1| varchar(8000)  |
| &#128270; | wip\_lbr\_acct\_unit2| varchar(8000)  |
| &#128270; | wip\_lbr\_acct\_unit3| varchar(8000)  |
| &#128270; | wip\_lbr\_acct\_unit4| varchar(8000)  |
| &#128270; | wip\_fovhd\_acct\_unit1| varchar(8000)  |
| &#128270; | wip\_fovhd\_acct\_unit2| varchar(8000)  |
| &#128270; | wip\_fovhd\_acct\_unit3| varchar(8000)  |
| &#128270; | wip\_fovhd\_acct\_unit4| varchar(8000)  |
| &#128270; | wip\_vovhd\_acct\_unit1| varchar(8000)  |
| &#128270; | wip\_vovhd\_acct\_unit2| varchar(8000)  |
| &#128270; | wip\_vovhd\_acct\_unit3| varchar(8000)  |
| &#128270; | wip\_vovhd\_acct\_unit4| varchar(8000)  |
| &#128270; | wip\_out\_acct\_unit1| varchar(8000)  |
| &#128270; | wip\_out\_acct\_unit2| varchar(8000)  |
| &#128270; | wip\_out\_acct\_unit3| varchar(8000)  |
| &#128270; | wip\_out\_acct\_unit4| varchar(8000)  |
| &#128270; | prod\_mix| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | config\_id| varchar(8000)  |
| &#128270; | co\_product\_mix| int  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | scheduled| int  |
| &#128270; | rcpt\_rqmt| varchar(8000)  |
| &#128270; | export\_type| varchar(8000)  |
| &#128270; | contains\_tax\_free\_matl| int  |
| &#128270; | midnight\_of\_job\_sch\_end\_date| datetime2(26)  |
| &#128270; | midnight\_of\_job\_sch\_compdate| datetime2(26)  |
| &#128270; | rework| int  |
| &#128270; | unlinked\_xref| int  |
| &#128270; | prospect\_id| varchar(8000)  |
| &#128270; | is\_external| int  |
| &#128270; | preassign\_lots| int  |
| &#128270; | preassign\_serials| int  |
| &#128270; | config\_doc\_id| varchar(8000)  |
| &#128270; | mo\_bom\_alternate\_id| varchar(8000)  |
| &#128270; | mo\_bom\_alternate\_description| varchar(8000)  |
| &#128270; | mo\_co\_job| int  |
| &#128270; | mo\_product\_cycle| int  |
| &#128270; | mo\_qty\_per\_cycle| decimal(19,8)  |
| &#128270; | mo\_job\_description| varchar(8000)  |
| &#128270; | pmf\_mfg\_spec\_order\_row\_pointer| varchar(8000)  |
| &#128270; | produces\_fill| int  |
| &#128270; | consumes\_fill| int  |
| &#128270; | pmf\_pn\_batch\_row\_pointer| varchar(8000)  |
| &#128270; | pmf\_formula\_row\_pointer| varchar(8000)  |
| &#128270; | copied\_from\_pmf\_formula\_row\_pointer| varchar(8000)  |
| &#128270; | pn\_batch\_job\_type| int  |
| &#128270; | plant| varchar(8000)  |
| &#128270; | uf\_batchqty| decimal(20,8)  |
| &#128270; | uf\_co\_line\_config\_description| varchar(8000)  |
| &#128270; | uf\_drawing\_no\_job| varchar(8000)  |
| &#128270; | uf\_item\_variation\_job| varchar(8000)  |
| &#128270; | uf\_job\_weight| decimal(11,2)  |
| &#128270; | uf\_old\_ref\_lin\_suf| int  |
| &#128270; | uf\_old\_ref\_num| varchar(8000)  |
| &#128270; | uf\_old\_ref\_release| int  |
| &#128270; | uf\_old\_ref\_type| varchar(8000)  |
| &#128270; | uf\_paint\_date| datetime2(26)  |
| &#128270; | uf\_paint\_pick| int  |
| &#128270; | uf\_paper\_work\_raised| int  |
| &#128270; | uf\_release\_date| datetime2(26)  |
| &#128270; | uf\_special\_packaging| varchar(8000)  |
| &#128270; | sas\_drawing\_vr\_location| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON job|
| &#128270;  | ClusteredIndex | ON suffix|
| &#128270;  | ClusteredIndex | ON job\_date|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON ord\_type|
| &#128270;  | ClusteredIndex | ON ord\_num|
| &#128270;  | ClusteredIndex | ON ord\_line|
| &#128270;  | ClusteredIndex | ON ord\_release|
| &#128270;  | ClusteredIndex | ON est\_job|
| &#128270;  | ClusteredIndex | ON est\_suf|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON qty\_released|
| &#128270;  | ClusteredIndex | ON qty\_complete|
| &#128270;  | ClusteredIndex | ON qty\_scrapped|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON lst\_trx\_date|
| &#128270;  | ClusteredIndex | ON root\_job|
| &#128270;  | ClusteredIndex | ON root\_suf|
| &#128270;  | ClusteredIndex | ON ref\_job|
| &#128270;  | ClusteredIndex | ON ref\_suf|
| &#128270;  | ClusteredIndex | ON ref\_oper|
| &#128270;  | ClusteredIndex | ON ref\_seq|
| &#128270;  | ClusteredIndex | ON low\_level|
| &#128270;  | ClusteredIndex | ON effect\_date|
| &#128270;  | ClusteredIndex | ON wip\_acct|
| &#128270;  | ClusteredIndex | ON wip\_total|
| &#128270;  | ClusteredIndex | ON wip\_complete|
| &#128270;  | ClusteredIndex | ON wip\_special|
| &#128270;  | ClusteredIndex | ON revision|
| &#128270;  | ClusteredIndex | ON picked|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON jcb\_acct|
| &#128270;  | ClusteredIndex | ON ps\_num|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_acct|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_acct|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_acct|
| &#128270;  | ClusteredIndex | ON wip\_out\_acct|
| &#128270;  | ClusteredIndex | ON wip\_matl\_total|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_total|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_total|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_total|
| &#128270;  | ClusteredIndex | ON wip\_out\_total|
| &#128270;  | ClusteredIndex | ON wip\_matl\_comp|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_comp|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_comp|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_comp|
| &#128270;  | ClusteredIndex | ON wip\_out\_comp|
| &#128270;  | ClusteredIndex | ON rollup\_date|
| &#128270;  | ClusteredIndex | ON wip\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON wip\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON wip\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON wip\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON jcb\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON jcb\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON jcb\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON jcb\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON wip\_out\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON wip\_out\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON wip\_out\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON wip\_out\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON prod\_mix|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON config\_id|
| &#128270;  | ClusteredIndex | ON co\_product\_mix|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON scheduled|
| &#128270;  | ClusteredIndex | ON rcpt\_rqmt|
| &#128270;  | ClusteredIndex | ON export\_type|
| &#128270;  | ClusteredIndex | ON contains\_tax\_free\_matl|
| &#128270;  | ClusteredIndex | ON midnight\_of\_job\_sch\_end\_date|
| &#128270;  | ClusteredIndex | ON midnight\_of\_job\_sch\_compdate|
| &#128270;  | ClusteredIndex | ON rework|
| &#128270;  | ClusteredIndex | ON unlinked\_xref|
| &#128270;  | ClusteredIndex | ON prospect\_id|
| &#128270;  | ClusteredIndex | ON is\_external|
| &#128270;  | ClusteredIndex | ON preassign\_lots|
| &#128270;  | ClusteredIndex | ON preassign\_serials|
| &#128270;  | ClusteredIndex | ON config\_doc\_id|
| &#128270;  | ClusteredIndex | ON mo\_bom\_alternate\_id|
| &#128270;  | ClusteredIndex | ON mo\_bom\_alternate\_description|
| &#128270;  | ClusteredIndex | ON mo\_co\_job|
| &#128270;  | ClusteredIndex | ON mo\_product\_cycle|
| &#128270;  | ClusteredIndex | ON mo\_qty\_per\_cycle|
| &#128270;  | ClusteredIndex | ON mo\_job\_description|
| &#128270;  | ClusteredIndex | ON pmf\_mfg\_spec\_order\_row\_pointer|
| &#128270;  | ClusteredIndex | ON produces\_fill|
| &#128270;  | ClusteredIndex | ON consumes\_fill|
| &#128270;  | ClusteredIndex | ON pmf\_pn\_batch\_row\_pointer|
| &#128270;  | ClusteredIndex | ON pmf\_formula\_row\_pointer|
| &#128270;  | ClusteredIndex | ON copied\_from\_pmf\_formula\_row\_pointer|
| &#128270;  | ClusteredIndex | ON pn\_batch\_job\_type|
| &#128270;  | ClusteredIndex | ON plant|
| &#128270;  | ClusteredIndex | ON uf\_batchqty|
| &#128270;  | ClusteredIndex | ON uf\_co\_line\_config\_description|
| &#128270;  | ClusteredIndex | ON uf\_drawing\_no\_job|
| &#128270;  | ClusteredIndex | ON uf\_item\_variation\_job|
| &#128270;  | ClusteredIndex | ON uf\_job\_weight|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_lin\_suf|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_num|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_release|
| &#128270;  | ClusteredIndex | ON uf\_old\_ref\_type|
| &#128270;  | ClusteredIndex | ON uf\_paint\_date|
| &#128270;  | ClusteredIndex | ON uf\_paint\_pick|
| &#128270;  | ClusteredIndex | ON uf\_paper\_work\_raised|
| &#128270;  | ClusteredIndex | ON uf\_release\_date|
| &#128270;  | ClusteredIndex | ON uf\_special\_packaging|
| &#128270;  | ClusteredIndex | ON sas\_drawing\_vr\_location|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.jobmatl_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | job| varchar(8000)  |
| &#128270; | suffix| int  |
| &#128270; | oper\_num| int  |
| &#128270; | sequence| int  |
| &#128270; | matl\_type| varchar(8000)  |
| &#128270; | item| varchar(8000)  |
| &#128270; | matl\_qty| decimal(18,8)  |
| &#128270; | units| varchar(8000)  |
| &#128270; | cost| decimal(20,8)  |
| &#128270; | qty\_issued| decimal(18,8)  |
| &#128270; | a\_cost| decimal(20,8)  |
| &#128270; | ref\_type| varchar(8000)  |
| &#128270; | ref\_num| varchar(8000)  |
| &#128270; | ref\_line\_suf| int  |
| &#128270; | ref\_release| int  |
| &#128270; | po\_unit\_cost| decimal(20,8)  |
| &#128270; | effect\_date| datetime2(26)  |
| &#128270; | obs\_date| datetime2(26)  |
| &#128270; | scrap\_fact| decimal(5,4)  |
| &#128270; | qty\_var| decimal(18,8)  |
| &#128270; | fixovhd\_t| decimal(20,8)  |
| &#128270; | varovhd\_t| decimal(20,8)  |
| &#128270; | feature| varchar(8000)  |
| &#128270; | probable| decimal(4,3)  |
| &#128270; | opt\_code| varchar(8000)  |
| &#128270; | inc\_price| decimal(20,8)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | pick\_date| datetime2(26)  |
| &#128270; | bom\_seq| int  |
| &#128270; | matl\_qty\_conv| decimal(18,8)  |
| &#128270; | u\_m| varchar(8000)  |
| &#128270; | inc\_price\_conv| decimal(20,8)  |
| &#128270; | cost\_conv| decimal(20,8)  |
| &#128270; | backflush| int  |
| &#128270; | bflush\_loc| varchar(8000)  |
| &#128270; | fmatlovhd| decimal(9,3)  |
| &#128270; | vmatlovhd| decimal(9,3)  |
| &#128270; | matl\_cost| decimal(20,8)  |
| &#128270; | lbr\_cost| decimal(20,8)  |
| &#128270; | fovhd\_cost| decimal(20,8)  |
| &#128270; | vovhd\_cost| decimal(20,8)  |
| &#128270; | out\_cost| decimal(20,8)  |
| &#128270; | a\_matl\_cost| decimal(20,8)  |
| &#128270; | a\_lbr\_cost| decimal(20,8)  |
| &#128270; | a\_fovhd\_cost| decimal(20,8)  |
| &#128270; | a\_vovhd\_cost| decimal(20,8)  |
| &#128270; | a\_out\_cost| decimal(20,8)  |
| &#128270; | matl\_cost\_conv| decimal(20,8)  |
| &#128270; | lbr\_cost\_conv| decimal(20,8)  |
| &#128270; | fovhd\_cost\_conv| decimal(20,8)  |
| &#128270; | vovhd\_cost\_conv| decimal(20,8)  |
| &#128270; | out\_cost\_conv| decimal(20,8)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | alt\_group| int  |
| &#128270; | alt\_group\_rank| int  |
| &#128270; | planned\_alternate| int  |
| &#128270; | new\_sequence| int  |
| &#128270; | manufacturer\_id| varchar(8000)  |
| &#128270; | manufacturer\_item| varchar(8000)  |
| &#128270; | pp\_matl\_is\_paper| int  |
| &#128270; | mo\_formula\_matl\_weight\_pct| decimal(6,3)  |
| &#128270; | revision| varchar(8000)  |
| &#128270; | qty\_picked| decimal(19,8)  |
| &#128270; | uf\_date\_updated| datetime2(26)  |
| &#128270; | uf\_job\_wip\_move| int  |
| &#128270; | uf\_long\_description| varchar(8000)  |
| &#128270; | uf\_updated| int  |
| &#128270; | uf\_unit\_price| decimal(18,8)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON job|
| &#128270;  | ClusteredIndex | ON suffix|
| &#128270;  | ClusteredIndex | ON oper\_num|
| &#128270;  | ClusteredIndex | ON sequence|
| &#128270;  | ClusteredIndex | ON matl\_type|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON matl\_qty|
| &#128270;  | ClusteredIndex | ON units|
| &#128270;  | ClusteredIndex | ON cost|
| &#128270;  | ClusteredIndex | ON qty\_issued|
| &#128270;  | ClusteredIndex | ON a\_cost|
| &#128270;  | ClusteredIndex | ON ref\_type|
| &#128270;  | ClusteredIndex | ON ref\_num|
| &#128270;  | ClusteredIndex | ON ref\_line\_suf|
| &#128270;  | ClusteredIndex | ON ref\_release|
| &#128270;  | ClusteredIndex | ON po\_unit\_cost|
| &#128270;  | ClusteredIndex | ON effect\_date|
| &#128270;  | ClusteredIndex | ON obs\_date|
| &#128270;  | ClusteredIndex | ON scrap\_fact|
| &#128270;  | ClusteredIndex | ON qty\_var|
| &#128270;  | ClusteredIndex | ON fixovhd\_t|
| &#128270;  | ClusteredIndex | ON varovhd\_t|
| &#128270;  | ClusteredIndex | ON feature|
| &#128270;  | ClusteredIndex | ON probable|
| &#128270;  | ClusteredIndex | ON opt\_code|
| &#128270;  | ClusteredIndex | ON inc\_price|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON pick\_date|
| &#128270;  | ClusteredIndex | ON bom\_seq|
| &#128270;  | ClusteredIndex | ON matl\_qty\_conv|
| &#128270;  | ClusteredIndex | ON u\_m|
| &#128270;  | ClusteredIndex | ON inc\_price\_conv|
| &#128270;  | ClusteredIndex | ON cost\_conv|
| &#128270;  | ClusteredIndex | ON backflush|
| &#128270;  | ClusteredIndex | ON bflush\_loc|
| &#128270;  | ClusteredIndex | ON fmatlovhd|
| &#128270;  | ClusteredIndex | ON vmatlovhd|
| &#128270;  | ClusteredIndex | ON matl\_cost|
| &#128270;  | ClusteredIndex | ON lbr\_cost|
| &#128270;  | ClusteredIndex | ON fovhd\_cost|
| &#128270;  | ClusteredIndex | ON vovhd\_cost|
| &#128270;  | ClusteredIndex | ON out\_cost|
| &#128270;  | ClusteredIndex | ON a\_matl\_cost|
| &#128270;  | ClusteredIndex | ON a\_lbr\_cost|
| &#128270;  | ClusteredIndex | ON a\_fovhd\_cost|
| &#128270;  | ClusteredIndex | ON a\_vovhd\_cost|
| &#128270;  | ClusteredIndex | ON a\_out\_cost|
| &#128270;  | ClusteredIndex | ON matl\_cost\_conv|
| &#128270;  | ClusteredIndex | ON lbr\_cost\_conv|
| &#128270;  | ClusteredIndex | ON fovhd\_cost\_conv|
| &#128270;  | ClusteredIndex | ON vovhd\_cost\_conv|
| &#128270;  | ClusteredIndex | ON out\_cost\_conv|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON alt\_group|
| &#128270;  | ClusteredIndex | ON alt\_group\_rank|
| &#128270;  | ClusteredIndex | ON planned\_alternate|
| &#128270;  | ClusteredIndex | ON new\_sequence|
| &#128270;  | ClusteredIndex | ON manufacturer\_id|
| &#128270;  | ClusteredIndex | ON manufacturer\_item|
| &#128270;  | ClusteredIndex | ON pp\_matl\_is\_paper|
| &#128270;  | ClusteredIndex | ON mo\_formula\_matl\_weight\_pct|
| &#128270;  | ClusteredIndex | ON revision|
| &#128270;  | ClusteredIndex | ON qty\_picked|
| &#128270;  | ClusteredIndex | ON uf\_date\_updated|
| &#128270;  | ClusteredIndex | ON uf\_job\_wip\_move|
| &#128270;  | ClusteredIndex | ON uf\_long\_description|
| &#128270;  | ClusteredIndex | ON uf\_updated|
| &#128270;  | ClusteredIndex | ON uf\_unit\_price|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.jobroute_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | job| varchar(8000)  |
| &#128270; | suffix| int  |
| &#128270; | oper\_num| int  |
| &#128270; | wc| varchar(8000)  |
| &#128270; | setup\_hrs\_t| decimal(19,8)  |
| &#128270; | setup\_cost\_t| decimal(20,8)  |
| &#128270; | complete| int  |
| &#128270; | setup\_hrs\_v| decimal(19,8)  |
| &#128270; | wip\_amt| decimal(20,8)  |
| &#128270; | qty\_scrapped| decimal(19,8)  |
| &#128270; | qty\_received| decimal(19,8)  |
| &#128270; | qty\_moved| decimal(19,8)  |
| &#128270; | qty\_complete| decimal(19,8)  |
| &#128270; | effect\_date| datetime2(26)  |
| &#128270; | obs\_date| datetime2(26)  |
| &#128270; | bflush\_type| varchar(8000)  |
| &#128270; | run\_basis\_lbr| varchar(8000)  |
| &#128270; | run\_basis\_mch| varchar(8000)  |
| &#128270; | fixovhd\_t\_lbr| decimal(20,8)  |
| &#128270; | fixovhd\_t\_mch| decimal(20,8)  |
| &#128270; | varovhd\_t\_lbr| decimal(20,8)  |
| &#128270; | varovhd\_t\_mch| decimal(20,8)  |
| &#128270; | run\_hrs\_t\_lbr| decimal(19,8)  |
| &#128270; | run\_hrs\_t\_mch| decimal(19,8)  |
| &#128270; | run\_hrs\_v\_lbr| decimal(10,5)  |
| &#128270; | run\_hrs\_v\_mch| decimal(10,5)  |
| &#128270; | run\_cost\_t\_lbr| decimal(20,8)  |
| &#128270; | cntrl\_point| int  |
| &#128270; | setup\_rate| decimal(10,3)  |
| &#128270; | efficiency| decimal(4,1)  |
| &#128270; | fovhd\_rate\_mch| decimal(9,3)  |
| &#128270; | vovhd\_rate\_mch| decimal(9,3)  |
| &#128270; | run\_rate\_lbr| decimal(10,3)  |
| &#128270; | varovhd\_rate| decimal(9,3)  |
| &#128270; | fixovhd\_rate| decimal(9,3)  |
| &#128270; | wip\_matl\_amt| decimal(20,8)  |
| &#128270; | wip\_lbr\_amt| decimal(20,8)  |
| &#128270; | wip\_fovhd\_amt| decimal(20,8)  |
| &#128270; | wip\_vovhd\_amt| decimal(20,8)  |
| &#128270; | wip\_out\_amt| decimal(20,8)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | yield| decimal(5,2)  |
| &#128270; | opm\_consec\_oper| int  |
| &#128270; | mo\_shared| int  |
| &#128270; | mo\_seconds\_per\_cycle| decimal(8,4)  |
| &#128270; | mo\_formula\_matl\_weight| decimal(9,2)  |
| &#128270; | mo\_formula\_matl\_weight\_units| varchar(8000)  |
| &#128270; | uf\_date\_updated| datetime2(26)  |
| &#128270; | uf\_long\_description| varchar(8000)  |
| &#128270; | uf\_qty\_complete| decimal(15,0)  |
| &#128270; | uf\_qty\_released| decimal(15,0)  |
| &#128270; | uf\_updated| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON job|
| &#128270;  | ClusteredIndex | ON suffix|
| &#128270;  | ClusteredIndex | ON oper\_num|
| &#128270;  | ClusteredIndex | ON wc|
| &#128270;  | ClusteredIndex | ON setup\_hrs\_t|
| &#128270;  | ClusteredIndex | ON setup\_cost\_t|
| &#128270;  | ClusteredIndex | ON complete|
| &#128270;  | ClusteredIndex | ON setup\_hrs\_v|
| &#128270;  | ClusteredIndex | ON wip\_amt|
| &#128270;  | ClusteredIndex | ON qty\_scrapped|
| &#128270;  | ClusteredIndex | ON qty\_received|
| &#128270;  | ClusteredIndex | ON qty\_moved|
| &#128270;  | ClusteredIndex | ON qty\_complete|
| &#128270;  | ClusteredIndex | ON effect\_date|
| &#128270;  | ClusteredIndex | ON obs\_date|
| &#128270;  | ClusteredIndex | ON bflush\_type|
| &#128270;  | ClusteredIndex | ON run\_basis\_lbr|
| &#128270;  | ClusteredIndex | ON run\_basis\_mch|
| &#128270;  | ClusteredIndex | ON fixovhd\_t\_lbr|
| &#128270;  | ClusteredIndex | ON fixovhd\_t\_mch|
| &#128270;  | ClusteredIndex | ON varovhd\_t\_lbr|
| &#128270;  | ClusteredIndex | ON varovhd\_t\_mch|
| &#128270;  | ClusteredIndex | ON run\_hrs\_t\_lbr|
| &#128270;  | ClusteredIndex | ON run\_hrs\_t\_mch|
| &#128270;  | ClusteredIndex | ON run\_hrs\_v\_lbr|
| &#128270;  | ClusteredIndex | ON run\_hrs\_v\_mch|
| &#128270;  | ClusteredIndex | ON run\_cost\_t\_lbr|
| &#128270;  | ClusteredIndex | ON cntrl\_point|
| &#128270;  | ClusteredIndex | ON setup\_rate|
| &#128270;  | ClusteredIndex | ON efficiency|
| &#128270;  | ClusteredIndex | ON fovhd\_rate\_mch|
| &#128270;  | ClusteredIndex | ON vovhd\_rate\_mch|
| &#128270;  | ClusteredIndex | ON run\_rate\_lbr|
| &#128270;  | ClusteredIndex | ON varovhd\_rate|
| &#128270;  | ClusteredIndex | ON fixovhd\_rate|
| &#128270;  | ClusteredIndex | ON wip\_matl\_amt|
| &#128270;  | ClusteredIndex | ON wip\_lbr\_amt|
| &#128270;  | ClusteredIndex | ON wip\_fovhd\_amt|
| &#128270;  | ClusteredIndex | ON wip\_vovhd\_amt|
| &#128270;  | ClusteredIndex | ON wip\_out\_amt|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON yield|
| &#128270;  | ClusteredIndex | ON opm\_consec\_oper|
| &#128270;  | ClusteredIndex | ON mo\_shared|
| &#128270;  | ClusteredIndex | ON mo\_seconds\_per\_cycle|
| &#128270;  | ClusteredIndex | ON mo\_formula\_matl\_weight|
| &#128270;  | ClusteredIndex | ON mo\_formula\_matl\_weight\_units|
| &#128270;  | ClusteredIndex | ON uf\_date\_updated|
| &#128270;  | ClusteredIndex | ON uf\_long\_description|
| &#128270;  | ClusteredIndex | ON uf\_qty\_complete|
| &#128270;  | ClusteredIndex | ON uf\_qty\_released|
| &#128270;  | ClusteredIndex | ON uf\_updated|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.jobtran_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | trans\_num| decimal(11,0)  |
| &#128270; | job| varchar(8000)  |
| &#128270; | suffix| int  |
| &#128270; | trans\_type| varchar(8000)  |
| &#128270; | trans\_date| datetime2(26)  |
| &#128270; | qty\_complete| decimal(19,8)  |
| &#128270; | qty\_scrapped| decimal(19,8)  |
| &#128270; | oper\_num| int  |
| &#128270; | a\_hrs| decimal(19,8)  |
| &#128270; | next\_oper| int  |
| &#128270; | emp\_num| varchar(8000)  |
| &#128270; | a\_dollar| decimal(20,8)  |
| &#128270; | start\_time| int  |
| &#128270; | end\_time| int  |
| &#128270; | ind\_code| varchar(8000)  |
| &#128270; | pay\_rate| varchar(8000)  |
| &#128270; | qty\_moved| decimal(19,8)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | loc| varchar(8000)  |
| &#128270; | user\_code| varchar(8000)  |
| &#128270; | close\_job| int  |
| &#128270; | issue\_parent| int  |
| &#128270; | lot| varchar(8000)  |
| &#128270; | complete\_op| int  |
| &#128270; | pr\_rate| decimal(9,3)  |
| &#128270; | job\_rate| decimal(9,3)  |
| &#128270; | shift| varchar(8000)  |
| &#128270; | posted| int  |
| &#128270; | low\_level| int  |
| &#128270; | backflush| int  |
| &#128270; | reason\_code| varchar(8000)  |
| &#128270; | trans\_class| varchar(8000)  |
| &#128270; | ps\_num| varchar(8000)  |
| &#128270; | wc| varchar(8000)  |
| &#128270; | awaiting\_eop| int  |
| &#128270; | fixovhd| decimal(20,8)  |
| &#128270; | varovhd| decimal(20,8)  |
| &#128270; | cost\_code| varchar(8000)  |
| &#128270; | co\_product\_mix| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | import\_doc\_id| varchar(8000)  |
| &#128270; | container\_num| varchar(8000)  |
| &#128270; | parent\_lot| varchar(8000)  |
| &#128270; | parent\_serial| varchar(8000)  |
| &#128270; | resid| varchar(8000)  |
| &#128270; | lot\_manufactured\_date| datetime2(26)  |
| &#128270; | downtime\_code| varchar(8000)  |
| &#128270; | uf\_lc\_lt\_resource| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON trans\_num|
| &#128270;  | ClusteredIndex | ON job|
| &#128270;  | ClusteredIndex | ON suffix|
| &#128270;  | ClusteredIndex | ON trans\_type|
| &#128270;  | ClusteredIndex | ON trans\_date|
| &#128270;  | ClusteredIndex | ON qty\_complete|
| &#128270;  | ClusteredIndex | ON qty\_scrapped|
| &#128270;  | ClusteredIndex | ON oper\_num|
| &#128270;  | ClusteredIndex | ON a\_hrs|
| &#128270;  | ClusteredIndex | ON next\_oper|
| &#128270;  | ClusteredIndex | ON emp\_num|
| &#128270;  | ClusteredIndex | ON a\_dollar|
| &#128270;  | ClusteredIndex | ON start\_time|
| &#128270;  | ClusteredIndex | ON end\_time|
| &#128270;  | ClusteredIndex | ON ind\_code|
| &#128270;  | ClusteredIndex | ON pay\_rate|
| &#128270;  | ClusteredIndex | ON qty\_moved|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON loc|
| &#128270;  | ClusteredIndex | ON user\_code|
| &#128270;  | ClusteredIndex | ON close\_job|
| &#128270;  | ClusteredIndex | ON issue\_parent|
| &#128270;  | ClusteredIndex | ON lot|
| &#128270;  | ClusteredIndex | ON complete\_op|
| &#128270;  | ClusteredIndex | ON pr\_rate|
| &#128270;  | ClusteredIndex | ON job\_rate|
| &#128270;  | ClusteredIndex | ON shift|
| &#128270;  | ClusteredIndex | ON posted|
| &#128270;  | ClusteredIndex | ON low\_level|
| &#128270;  | ClusteredIndex | ON backflush|
| &#128270;  | ClusteredIndex | ON reason\_code|
| &#128270;  | ClusteredIndex | ON trans\_class|
| &#128270;  | ClusteredIndex | ON ps\_num|
| &#128270;  | ClusteredIndex | ON wc|
| &#128270;  | ClusteredIndex | ON awaiting\_eop|
| &#128270;  | ClusteredIndex | ON fixovhd|
| &#128270;  | ClusteredIndex | ON varovhd|
| &#128270;  | ClusteredIndex | ON cost\_code|
| &#128270;  | ClusteredIndex | ON co\_product\_mix|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON import\_doc\_id|
| &#128270;  | ClusteredIndex | ON container\_num|
| &#128270;  | ClusteredIndex | ON parent\_lot|
| &#128270;  | ClusteredIndex | ON parent\_serial|
| &#128270;  | ClusteredIndex | ON resid|
| &#128270;  | ClusteredIndex | ON lot\_manufactured\_date|
| &#128270;  | ClusteredIndex | ON downtime\_code|
| &#128270;  | ClusteredIndex | ON uf\_lc\_lt\_resource|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table staging.kpi_kpi_result_v3 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(8000)  |
| &#128270; | kpi\_value| float(53)  |
| &#128270; | organisational\_unit| varchar(8000)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(8000)  |
| &#128270; | target\_value| float(53)  |
| &#128270; | breach\_direction| varchar(8000)  |
| &#128270; | week\_key| varchar(8000)  |
| &#128270; | kpi\_code| varchar(8000)  |
| &#128270; | department| varchar(8000)  |
| &#128270; | measure| varchar(8000)  |
| &#128270; | measure\_name| varchar(8000)  |
| &#128270; | uom| varchar(8000)  |
| &#128270; | sign| varchar(8000)  |
| &#128270; | sign\_label| varchar(8000)  |
| &#128270; | commentary| varchar(8000)  |
| &#128270; | variance\_value| float(53)  |
| &#128270; | performance\_variance\_value| float(53)  |
| &#128270; | rag\_status| varchar(8000)  |
| &#128270; | data\_status| varchar(8000)  |
| &#128270; | source\_system| varchar(8000)  |
| &#128270; | source\_object| varchar(8000)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table salesforce.kpi_result_design_rnd 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| * &#128270; | kpi\_name| varchar(100)  |
| &#128270; | kpi\_value| decimal(18,6)  |
| * &#128270; | organisational\_unit| varchar(100)  |
| &#128270; | kpi\_id| bigint  |
| * &#128270; | kpi\_category| varchar(100)  |
| &#128270; | target\_value| decimal(18,6)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | week\_key| int  |
| * &#128270; | kpi\_code| varchar(50)  |
| * &#128270; | department| varchar(100)  |
| * &#128270; | measure| varchar(100)  |
| * &#128270; | measure\_name| varchar(100)  |
| * &#128270; | uom| varchar(50)  |
| &#128270; | sign| varchar(20)  |
| &#128270; | sign\_label| varchar(20)  |
| * &#128270; | commentary| varchar(500)  |
| &#128270; | variance\_value| decimal(18,6)  |
| &#128270; | performance\_variance\_value| decimal(18,6)  |
| * &#128270; | rag\_status| varchar(20)  |
| * &#128270; | data\_status| varchar(50)  |
| * &#128270; | source\_system| varchar(50)  |
| * &#128270; | source\_object| varchar(500)  |
| * &#128270; | source\_row\_count| bigint  |
| * &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table safety_culture.kpi_result_ehs_safetyculture 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(255)  |
| &#128270; | kpi\_value| decimal(18,6)  |
| &#128270; | organisational\_unit| varchar(255)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(100)  |
| &#128270; | target\_value| decimal(18,6)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_code| varchar(100)  |
| &#128270; | department| varchar(255)  |
| &#128270; | measure| varchar(500)  |
| &#128270; | measure\_name| varchar(500)  |
| &#128270; | unit\_of\_measure| varchar(50)  |
| &#128270; | sign| varchar(100)  |
| &#128270; | sign\_label| varchar(100)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | variance\_value| decimal(18,6)  |
| &#128270; | performance\_variance\_value| decimal(18,6)  |
| &#128270; | red\_amber\_green\_status| varchar(20)  |
| &#128270; | data\_status| varchar(50)  |
| &#128270; | source\_system| varchar(100)  |
| &#128270; | source\_object| varchar(500)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON unit\_of\_measure|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON red\_amber\_green\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table freshservice.kpi_result_it_freshservice 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(255)  |
| &#128270; | kpi\_value| decimal(18,6)  |
| &#128270; | organisational\_unit| varchar(255)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(100)  |
| &#128270; | target\_value| decimal(18,6)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_code| varchar(100)  |
| &#128270; | department| varchar(255)  |
| &#128270; | measure| varchar(500)  |
| &#128270; | measure\_name| varchar(500)  |
| &#128270; | uom| varchar(50)  |
| &#128270; | sign| varchar(100)  |
| &#128270; | sign\_label| varchar(100)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | variance\_value| decimal(18,6)  |
| &#128270; | performance\_variance\_value| decimal(18,6)  |
| &#128270; | rag\_status| varchar(20)  |
| &#128270; | data\_status| varchar(50)  |
| &#128270; | source\_system| varchar(100)  |
| &#128270; | source\_object| varchar(500)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table syteline.kpi_result_product_engineering_cost 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(255)  |
| &#128270; | kpi\_value| decimal(18,6)  |
| &#128270; | organisational\_unit| varchar(255)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(100)  |
| &#128270; | target\_value| decimal(18,6)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_code| varchar(100)  |
| &#128270; | department| varchar(255)  |
| &#128270; | measure| varchar(500)  |
| &#128270; | measure\_name| varchar(500)  |
| &#128270; | uom| varchar(50)  |
| &#128270; | sign| varchar(100)  |
| &#128270; | sign\_label| varchar(100)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | variance\_value| decimal(18,6)  |
| &#128270; | performance\_variance\_value| decimal(18,6)  |
| &#128270; | rag\_status| varchar(20)  |
| &#128270; | data\_status| varchar(50)  |
| &#128270; | source\_system| varchar(100)  |
| &#128270; | source\_object| varchar(500)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table syteline.kpi_result_product_engineering_productivity 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(255)  |
| &#128270; | kpi\_value| decimal(18,6)  |
| &#128270; | organisational\_unit| varchar(255)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(100)  |
| &#128270; | target\_value| decimal(18,6)  |
| &#128270; | breach\_direction| varchar(20)  |
| &#128270; | week\_key| int  |
| &#128270; | kpi\_code| varchar(100)  |
| &#128270; | department| varchar(255)  |
| &#128270; | measure| varchar(500)  |
| &#128270; | measure\_name| varchar(500)  |
| &#128270; | uom| varchar(50)  |
| &#128270; | sign| varchar(100)  |
| &#128270; | sign\_label| varchar(100)  |
| &#128270; | commentary| varchar(1000)  |
| &#128270; | variance\_value| decimal(18,6)  |
| &#128270; | performance\_variance\_value| decimal(18,6)  |
| &#128270; | rag\_status| varchar(20)  |
| &#128270; | data\_status| varchar(50)  |
| &#128270; | source\_system| varchar(100)  |
| &#128270; | source\_object| varchar(500)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table staging.kpi_result_silver 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(8000)  |
| &#128270; | kpi\_value| float(53)  |
| &#128270; | organisational\_unit| varchar(8000)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|



### Table dbo.kpi_result_silver_enriched_v2 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | closed\_year| int  |
| &#128270; | closed\_week| int  |
| &#128270; | kpi\_name| varchar(8000)  |
| &#128270; | kpi\_value| float(53)  |
| &#128270; | organisational\_unit| varchar(8000)  |
| &#128270; | kpi\_id| bigint  |
| &#128270; | kpi\_category| varchar(8000)  |
| &#128270; | target\_value| float(53)  |
| &#128270; | breach\_direction| varchar(8000)  |
| &#128270; | week\_key| varchar(8000)  |
| &#128270; | kpi\_code| varchar(8000)  |
| &#128270; | department| varchar(8000)  |
| &#128270; | measure| varchar(8000)  |
| &#128270; | measure\_name| varchar(8000)  |
| &#128270; | uom| varchar(8000)  |
| &#128270; | sign| varchar(8000)  |
| &#128270; | sign\_label| varchar(8000)  |
| &#128270; | commentary| varchar(8000)  |
| &#128270; | variance\_value| float(53)  |
| &#128270; | performance\_variance\_value| float(53)  |
| &#128270; | rag\_status| varchar(8000)  |
| &#128270; | data\_status| varchar(8000)  |
| &#128270; | source\_system| varchar(8000)  |
| &#128270; | source\_object| varchar(8000)  |
| &#128270; | source\_row\_count| bigint  |
| &#128270; | calculation\_timestamp| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON closed\_year|
| &#128270;  | ClusteredIndex | ON closed\_week|
| &#128270;  | ClusteredIndex | ON kpi\_name|
| &#128270;  | ClusteredIndex | ON kpi\_value|
| &#128270;  | ClusteredIndex | ON organisational\_unit|
| &#128270;  | ClusteredIndex | ON kpi\_id|
| &#128270;  | ClusteredIndex | ON kpi\_category|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON breach\_direction|
| &#128270;  | ClusteredIndex | ON week\_key|
| &#128270;  | ClusteredIndex | ON kpi\_code|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON measure|
| &#128270;  | ClusteredIndex | ON measure\_name|
| &#128270;  | ClusteredIndex | ON uom|
| &#128270;  | ClusteredIndex | ON sign|
| &#128270;  | ClusteredIndex | ON sign\_label|
| &#128270;  | ClusteredIndex | ON commentary|
| &#128270;  | ClusteredIndex | ON variance\_value|
| &#128270;  | ClusteredIndex | ON performance\_variance\_value|
| &#128270;  | ClusteredIndex | ON rag\_status|
| &#128270;  | ClusteredIndex | ON data\_status|
| &#128270;  | ClusteredIndex | ON source\_system|
| &#128270;  | ClusteredIndex | ON source\_object|
| &#128270;  | ClusteredIndex | ON source\_row\_count|
| &#128270;  | ClusteredIndex | ON calculation\_timestamp|



### Table syteline_staging.ledger_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | trans\_num| decimal(10,0)  |
| &#128270; | acct| varchar(8000)  |
| &#128270; | trans\_date| datetime2(26)  |
| &#128270; | dom\_amount| decimal(23,8)  |
| &#128270; | ref| varchar(8000)  |
| &#128270; | vend\_num| varchar(8000)  |
| &#128270; | voucher| varchar(8000)  |
| &#128270; | check\_num| int  |
| &#128270; | check\_date| datetime2(26)  |
| &#128270; | from\_site| varchar(8000)  |
| &#128270; | from\_id| varchar(8000)  |
| &#128270; | vouch\_seq| int  |
| &#128270; | ref\_type| varchar(8000)  |
| &#128270; | matl\_trans\_num| decimal(10,0)  |
| &#128270; | d\_trans\_num| decimal(10,0)  |
| &#128270; | bank\_code| varchar(8000)  |
| &#128270; | acct\_unit1| varchar(8000)  |
| &#128270; | acct\_unit2| varchar(8000)  |
| &#128270; | acct\_unit3| varchar(8000)  |
| &#128270; | acct\_unit4| varchar(8000)  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | exch\_rate| decimal(12,7)  |
| &#128270; | for\_amount| decimal(23,8)  |
| &#128270; | site| varchar(8000)  |
| &#128270; | hierarchy| varchar(8000)  |
| &#128270; | consolidated| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | journal\_batch\_id| decimal(24,0)  |
| &#128270; | control\_prefix| varchar(8000)  |
| &#128270; | control\_site| varchar(8000)  |
| &#128270; | control\_year| int  |
| &#128270; | control\_period| int  |
| &#128270; | control\_number| decimal(10,0)  |
| &#128270; | ref\_control\_prefix| varchar(8000)  |
| &#128270; | ref\_control\_site| varchar(8000)  |
| &#128270; | ref\_control\_year| int  |
| &#128270; | ref\_control\_period| int  |
| &#128270; | ref\_control\_number| decimal(10,0)  |
| &#128270; | processed| int  |
| &#128270; | proj\_trans\_num| decimal(11,0)  |
| &#128270; | cancellation| int  |
| &#128270; | gl\_voucher| varchar(8000)  |
| &#128270; | fr\_letter| varchar(8000)  |
| &#128270; | fr\_lettering\_date| datetime2(26)  |
| &#128270; | th\_payment\_number| varchar(8000)  |
| &#128270; | pl\_journal\_create\_date| datetime2(26)  |
| &#128270; | pl\_journal\_created\_by| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON trans\_num|
| &#128270;  | ClusteredIndex | ON acct|
| &#128270;  | ClusteredIndex | ON trans\_date|
| &#128270;  | ClusteredIndex | ON dom\_amount|
| &#128270;  | ClusteredIndex | ON ref|
| &#128270;  | ClusteredIndex | ON vend\_num|
| &#128270;  | ClusteredIndex | ON voucher|
| &#128270;  | ClusteredIndex | ON check\_num|
| &#128270;  | ClusteredIndex | ON check\_date|
| &#128270;  | ClusteredIndex | ON from\_site|
| &#128270;  | ClusteredIndex | ON from\_id|
| &#128270;  | ClusteredIndex | ON vouch\_seq|
| &#128270;  | ClusteredIndex | ON ref\_type|
| &#128270;  | ClusteredIndex | ON matl\_trans\_num|
| &#128270;  | ClusteredIndex | ON d\_trans\_num|
| &#128270;  | ClusteredIndex | ON bank\_code|
| &#128270;  | ClusteredIndex | ON acct\_unit1|
| &#128270;  | ClusteredIndex | ON acct\_unit2|
| &#128270;  | ClusteredIndex | ON acct\_unit3|
| &#128270;  | ClusteredIndex | ON acct\_unit4|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON exch\_rate|
| &#128270;  | ClusteredIndex | ON for\_amount|
| &#128270;  | ClusteredIndex | ON site|
| &#128270;  | ClusteredIndex | ON hierarchy|
| &#128270;  | ClusteredIndex | ON consolidated|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON journal\_batch\_id|
| &#128270;  | ClusteredIndex | ON control\_prefix|
| &#128270;  | ClusteredIndex | ON control\_site|
| &#128270;  | ClusteredIndex | ON control\_year|
| &#128270;  | ClusteredIndex | ON control\_period|
| &#128270;  | ClusteredIndex | ON control\_number|
| &#128270;  | ClusteredIndex | ON ref\_control\_prefix|
| &#128270;  | ClusteredIndex | ON ref\_control\_site|
| &#128270;  | ClusteredIndex | ON ref\_control\_year|
| &#128270;  | ClusteredIndex | ON ref\_control\_period|
| &#128270;  | ClusteredIndex | ON ref\_control\_number|
| &#128270;  | ClusteredIndex | ON processed|
| &#128270;  | ClusteredIndex | ON proj\_trans\_num|
| &#128270;  | ClusteredIndex | ON cancellation|
| &#128270;  | ClusteredIndex | ON gl\_voucher|
| &#128270;  | ClusteredIndex | ON fr\_letter|
| &#128270;  | ClusteredIndex | ON fr\_lettering\_date|
| &#128270;  | ClusteredIndex | ON th\_payment\_number|
| &#128270;  | ClusteredIndex | ON pl\_journal\_create\_date|
| &#128270;  | ClusteredIndex | ON pl\_journal\_created\_by|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table sharepoint.mean_time_between_failure 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | mtbf| float(53)  |
| &#128270; | target| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON mtbf|
| &#128270;  | ClusteredIndex | ON target|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint_staging.mean_time_between_failure 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | mtbf| float(53)  |
| &#128270; | target| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON mtbf|
| &#128270;  | ClusteredIndex | ON target|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.non_inventory_item_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | item| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | u\_m| varchar(8000)  |
| &#128270; | drawing\_nbr| varchar(8000)  |
| &#128270; | revision| varchar(8000)  |
| &#128270; | product\_code| varchar(8000)  |
| &#128270; | family\_code| varchar(8000)  |
| &#128270; | matl\_type| varchar(8000)  |
| &#128270; | comm\_code| varchar(8000)  |
| &#128270; | origin| varchar(8000)  |
| &#128270; | prod\_type| varchar(8000)  |
| &#128270; | tariff\_classification| varchar(8000)  |
| &#128270; | nafta\_pref\_crit| varchar(8000)  |
| &#128270; | subject\_to\_nafta\_rvc| int  |
| &#128270; | producer| int  |
| &#128270; | nafta\_country\_of\_origin| varchar(8000)  |
| &#128270; | unit\_cost| decimal(20,8)  |
| &#128270; | unit\_price| decimal(20,8)  |
| &#128270; | unit\_weight| decimal(11,5)  |
| &#128270; | weight\_units| varchar(8000)  |
| &#128270; | buyer| varchar(8000)  |
| &#128270; | show\_in\_drop\_down\_list| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | pp\_length\_linear\_dimension| decimal(20,8)  |
| &#128270; | pp\_width\_linear\_dimension| decimal(20,8)  |
| &#128270; | pp\_height\_linear\_dimension| decimal(20,8)  |
| &#128270; | pp\_linear\_dimension\_u\_m| varchar(8000)  |
| &#128270; | pp\_density| decimal(23,8)  |
| &#128270; | pp\_density\_u\_m| varchar(8000)  |
| &#128270; | pp\_area| decimal(23,8)  |
| &#128270; | pp\_area\_u\_m| varchar(8000)  |
| &#128270; | pp\_bulk\_mass| decimal(11,5)  |
| &#128270; | pp\_bulk\_mass\_u\_m| varchar(8000)  |
| &#128270; | pp\_ream\_mass| decimal(11,5)  |
| &#128270; | pp\_ream\_mass\_u\_m| varchar(8000)  |
| &#128270; | pp\_grade| int  |
| &#128270; | pp\_abnormal\_size| int  |
| &#128270; | pp\_paper\_mass\_basis| varchar(8000)  |
| &#128270; | pp\_unit\_price2| decimal(20,8)  |
| &#128270; | pp\_unit\_price3| decimal(20,8)  |
| &#128270; | pp\_unit\_price4| decimal(20,8)  |
| &#128270; | pp\_unit\_price5| decimal(20,8)  |
| &#128270; | pp\_unit\_price6| decimal(20,8)  |
| &#128270; | pp\_brk\_qty\_1| decimal(19,8)  |
| &#128270; | pp\_brk\_qty\_2| decimal(19,8)  |
| &#128270; | pp\_brk\_qty\_3| decimal(19,8)  |
| &#128270; | pp\_brk\_qty\_4| decimal(19,8)  |
| &#128270; | pp\_brk\_qty\_5| decimal(19,8)  |
| &#128270; | pp\_base\_code\_1| varchar(8000)  |
| &#128270; | pp\_base\_code\_2| varchar(8000)  |
| &#128270; | pp\_base\_code\_3| varchar(8000)  |
| &#128270; | pp\_base\_code\_4| varchar(8000)  |
| &#128270; | pp\_base\_code\_5| varchar(8000)  |
| &#128270; | pp\_dol\_percent\_1| varchar(8000)  |
| &#128270; | pp\_dol\_percent\_2| varchar(8000)  |
| &#128270; | pp\_dol\_percent\_3| varchar(8000)  |
| &#128270; | pp\_dol\_percent\_4| varchar(8000)  |
| &#128270; | pp\_dol\_percent\_5| varchar(8000)  |
| &#128270; | pp\_brk\_price\_1| decimal(20,8)  |
| &#128270; | pp\_brk\_price\_2| decimal(20,8)  |
| &#128270; | pp\_brk\_price\_3| decimal(20,8)  |
| &#128270; | pp\_brk\_price\_4| decimal(20,8)  |
| &#128270; | pp\_brk\_price\_5| decimal(20,8)  |
| &#128270; | allow\_on\_pick\_list| int  |
| &#128270; | uf\_non\_inv\_acct| varchar(8000)  |
| &#128270; | uf\_non\_inv\_no\_tp| int  |
| &#128270; | uf\_non\_inv\_unit1| varchar(8000)  |
| &#128270; | uf\_non\_inv\_unit2| varchar(8000)  |
| &#128270; | uf\_non\_inv\_unit3| varchar(8000)  |
| &#128270; | uf\_non\_inv\_unit4| varchar(8000)  |
| &#128270; | uf\_update\_uc4| int  |
| &#128270; | uf\_salesforce\_id| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON u\_m|
| &#128270;  | ClusteredIndex | ON drawing\_nbr|
| &#128270;  | ClusteredIndex | ON revision|
| &#128270;  | ClusteredIndex | ON product\_code|
| &#128270;  | ClusteredIndex | ON family\_code|
| &#128270;  | ClusteredIndex | ON matl\_type|
| &#128270;  | ClusteredIndex | ON comm\_code|
| &#128270;  | ClusteredIndex | ON origin|
| &#128270;  | ClusteredIndex | ON prod\_type|
| &#128270;  | ClusteredIndex | ON tariff\_classification|
| &#128270;  | ClusteredIndex | ON nafta\_pref\_crit|
| &#128270;  | ClusteredIndex | ON subject\_to\_nafta\_rvc|
| &#128270;  | ClusteredIndex | ON producer|
| &#128270;  | ClusteredIndex | ON nafta\_country\_of\_origin|
| &#128270;  | ClusteredIndex | ON unit\_cost|
| &#128270;  | ClusteredIndex | ON unit\_price|
| &#128270;  | ClusteredIndex | ON unit\_weight|
| &#128270;  | ClusteredIndex | ON weight\_units|
| &#128270;  | ClusteredIndex | ON buyer|
| &#128270;  | ClusteredIndex | ON show\_in\_drop\_down\_list|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON pp\_length\_linear\_dimension|
| &#128270;  | ClusteredIndex | ON pp\_width\_linear\_dimension|
| &#128270;  | ClusteredIndex | ON pp\_height\_linear\_dimension|
| &#128270;  | ClusteredIndex | ON pp\_linear\_dimension\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_density|
| &#128270;  | ClusteredIndex | ON pp\_density\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_area|
| &#128270;  | ClusteredIndex | ON pp\_area\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_bulk\_mass|
| &#128270;  | ClusteredIndex | ON pp\_bulk\_mass\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_ream\_mass|
| &#128270;  | ClusteredIndex | ON pp\_ream\_mass\_u\_m|
| &#128270;  | ClusteredIndex | ON pp\_grade|
| &#128270;  | ClusteredIndex | ON pp\_abnormal\_size|
| &#128270;  | ClusteredIndex | ON pp\_paper\_mass\_basis|
| &#128270;  | ClusteredIndex | ON pp\_unit\_price2|
| &#128270;  | ClusteredIndex | ON pp\_unit\_price3|
| &#128270;  | ClusteredIndex | ON pp\_unit\_price4|
| &#128270;  | ClusteredIndex | ON pp\_unit\_price5|
| &#128270;  | ClusteredIndex | ON pp\_unit\_price6|
| &#128270;  | ClusteredIndex | ON pp\_brk\_qty\_1|
| &#128270;  | ClusteredIndex | ON pp\_brk\_qty\_2|
| &#128270;  | ClusteredIndex | ON pp\_brk\_qty\_3|
| &#128270;  | ClusteredIndex | ON pp\_brk\_qty\_4|
| &#128270;  | ClusteredIndex | ON pp\_brk\_qty\_5|
| &#128270;  | ClusteredIndex | ON pp\_base\_code\_1|
| &#128270;  | ClusteredIndex | ON pp\_base\_code\_2|
| &#128270;  | ClusteredIndex | ON pp\_base\_code\_3|
| &#128270;  | ClusteredIndex | ON pp\_base\_code\_4|
| &#128270;  | ClusteredIndex | ON pp\_base\_code\_5|
| &#128270;  | ClusteredIndex | ON pp\_dol\_percent\_1|
| &#128270;  | ClusteredIndex | ON pp\_dol\_percent\_2|
| &#128270;  | ClusteredIndex | ON pp\_dol\_percent\_3|
| &#128270;  | ClusteredIndex | ON pp\_dol\_percent\_4|
| &#128270;  | ClusteredIndex | ON pp\_dol\_percent\_5|
| &#128270;  | ClusteredIndex | ON pp\_brk\_price\_1|
| &#128270;  | ClusteredIndex | ON pp\_brk\_price\_2|
| &#128270;  | ClusteredIndex | ON pp\_brk\_price\_3|
| &#128270;  | ClusteredIndex | ON pp\_brk\_price\_4|
| &#128270;  | ClusteredIndex | ON pp\_brk\_price\_5|
| &#128270;  | ClusteredIndex | ON allow\_on\_pick\_list|
| &#128270;  | ClusteredIndex | ON uf\_non\_inv\_acct|
| &#128270;  | ClusteredIndex | ON uf\_non\_inv\_no\_tp|
| &#128270;  | ClusteredIndex | ON uf\_non\_inv\_unit1|
| &#128270;  | ClusteredIndex | ON uf\_non\_inv\_unit2|
| &#128270;  | ClusteredIndex | ON uf\_non\_inv\_unit3|
| &#128270;  | ClusteredIndex | ON uf\_non\_inv\_unit4|
| &#128270;  | ClusteredIndex | ON uf\_update\_uc4|
| &#128270;  | ClusteredIndex | ON uf\_salesforce\_id|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.opportunity 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | account\_id| varchar(8000)  |
| &#128270; | record\_type\_id| varchar(8000)  |
| &#128270; | is\_private| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | stage\_name| varchar(8000)  |
| &#128270; | amount| decimal(38,18)  |
| &#128270; | probability| decimal(38,18)  |
| &#128270; | expected\_revenue| decimal(38,18)  |
| &#128270; | total\_opportunity\_quantity| decimal(38,18)  |
| &#128270; | close\_date| datetime2(26)  |
| &#128270; | type| varchar(8000)  |
| &#128270; | next\_step| varchar(8000)  |
| &#128270; | lead\_source| varchar(8000)  |
| &#128270; | is\_closed| bit  |
| &#128270; | is\_won| bit  |
| &#128270; | forecast\_category| varchar(8000)  |
| &#128270; | forecast\_category\_name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | campaign\_id| varchar(8000)  |
| &#128270; | has\_opportunity\_line\_item| bit  |
| &#128270; | pricebook2\_id| varchar(8000)  |
| &#128270; | owner\_id| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | fiscal\_quarter| int  |
| &#128270; | fiscal\_year| int  |
| &#128270; | fiscal| varchar(8000)  |
| &#128270; | contact\_id| varchar(8000)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | contract\_id| varchar(8000)  |
| &#128270; | has\_open\_activity| bit  |
| &#128270; | has\_overdue\_task| bit  |
| &#128270; | merge\_field| varchar(8000)  |
| &#128270; | submarket| varchar(8000)  |
| &#128270; | net\_internal\_area| decimal(38,18)  |
| &#128270; | additional\_address\_line| varchar(8000)  |
| &#128270; | loss\_reason| varchar(8000)  |
| &#128270; | address| varchar(8000)  |
| &#128270; | balance| decimal(38,18)  |
| &#128270; | build\_type| varchar(8000)  |
| &#128270; | building\_name\_number| varchar(8000)  |
| &#128270; | contact| varchar(8000)  |
| &#128270; | country| varchar(8000)  |
| &#128270; | custom\_rollup\_summary| decimal(38,18)  |
| &#128270; | deleted\_reason| varchar(8000)  |
| &#128270; | forecasted\_sqm| decimal(38,18)  |
| &#128270; | forecasted\_value| decimal(38,18)  |
| &#128270; | infor\_reference\_number| varchar(8000)  |
| &#128270; | last\_interaction\_date| datetime2(26)  |
| &#128270; | lead\_reference| varchar(8000)  |
| &#128270; | lease\_expiry\_follow\_up| datetime2(26)  |
| &#128270; | link\_to\_external\_lead| varchar(8000)  |
| &#128270; | lost\_deleted\_additional\_info| varchar(8000)  |
| &#128270; | securing\_manufacturer| varchar(8000)  |
| &#128270; | marketing\_additional\_info| varchar(8000)  |
| &#128270; | new\_proposal| bit  |
| &#128270; | notes| varchar(8000)  |
| &#128270; | opportunity\_sqm| decimal(38,18)  |
| &#128270; | opportunity\_value| decimal(38,18)  |
| &#128270; | order\_date| datetime2(26)  |
| &#128270; | order\_sqm| decimal(38,18)  |
| &#128270; | order\_value| decimal(38,18)  |
| &#128270; | pass\_to\_marketing| varchar(8000)  |
| &#128270; | photo\_available\_date| datetime2(26)  |
| &#128270; | postcode| varchar(8000)  |
| &#128270; | project\_alternative\_name| varchar(8000)  |
| &#128270; | project\_complete| bit  |
| &#128270; | budget\_value| decimal(38,18)  |
| &#128270; | project\_concern\_info| varchar(8000)  |
| &#128270; | project\_concerns| varchar(8000)  |
| &#128270; | project\_delivery\_date\_from| datetime2(26)  |
| &#128270; | project\_delivery\_date\_to| datetime2(26)  |
| &#128270; | project\_estimated\_start\_date| datetime2(26)  |
| &#128270; | project\_probability| varchar(8000)  |
| &#128270; | proposal\_issued| varchar(8000)  |
| &#128270; | proposal\_issued\_date| datetime2(26)  |
| &#128270; | push\_count| decimal(38,18)  |
| &#128270; | reason\_for\_raising\_a\_project| varchar(8000)  |
| &#128270; | red\_flag\_removal\_reason| varchar(8000)  |
| &#128270; | red\_flag\_status\_old\_values| varchar(8000)  |
| &#128270; | region| varchar(8000)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | sales\_region| varchar(8000)  |
| &#128270; | scheme| varchar(8000)  |
| &#128270; | secondary\_owner| varchar(8000)  |
| &#128270; | secondary\_source| varchar(8000)  |
| &#128270; | sharepoint| varchar(8000)  |
| &#128270; | source\_if\_other| varchar(8000)  |
| &#128270; | specification\_detail| varchar(8000)  |
| &#128270; | street\_address| varchar(8000)  |
| &#128270; | total\_opportunity\_size\_sqm| decimal(38,18)  |
| &#128270; | town| varchar(8000)  |
| &#128270; | estimates\_rollup| decimal(38,18)  |
| &#128270; | main\_contractor\_records| decimal(38,18)  |
| &#128270; | sub\_contractor\_records| decimal(38,18)  |
| &#128270; | opportunity\_sqm\_two| decimal(38,18)  |
| &#128270; | product\_count| decimal(38,18)  |
| &#128270; | project\_owner| varchar(8000)  |
| &#128270; | opportunity\_review\_required| bit  |
| &#128270; | business\_commercial\_review\_required| bit  |
| &#128270; | typical\_floor\_size| decimal(38,18)  |
| &#128270; | verified| bit  |
| &#128270; | number\_of\_floors| decimal(38,18)  |
| &#128270; | architect\_contacts\_checkbox| bit  |
| &#128270; | engaged\_with\_architect| bit  |
| &#128270; | architect\_listed| bit  |
| &#128270; | concept\_source| varchar(8000)  |
| &#128270; | client\_listed| bit  |
| &#128270; | opportunity\_sign\_off| varchar(8000)  |
| &#128270; | opportunity\_review\_date| datetime2(26)  |
| &#128270; | opportunity\_sign\_off\_by| varchar(8000)  |
| &#128270; | opportunity\_review\_notes| varchar(8000)  |
| &#128270; | client\_contact\_listed| bit  |
| &#128270; | design\_review\_by| varchar(8000)  |
| &#128270; | design\_review| bit  |
| &#128270; | budget\_provided| bit  |
| &#128270; | construction\_dates\_provided| bit  |
| &#128270; | products\_specified\_checkbox| bit  |
| &#128270; | proposal\_issued\_checkbox| bit  |
| &#128270; | competitor\_project\_value| decimal(38,18)  |
| &#128270; | specification\_issued| bit  |
| &#128270; | estimates\_sent| bit  |
| &#128270; | project\_images| varchar(8000)  |
| &#128270; | final\_target\_market\_value| decimal(38,18)  |
| &#128270; | final\_target\_sales\_price| decimal(38,18)  |
| &#128270; | main\_contractor\_bidders\_provided| bit  |
| &#128270; | main\_contractor\_engagement| bit  |
| &#128270; | fit\_out\_contractor\_records| decimal(38,18)  |
| &#128270; | nda\_signed| bit  |
| &#128270; | special\_projects\_reference| varchar(8000)  |
| &#128270; | prior\_stage| varchar(8000)  |
| &#128270; | sub\_contractor\_bidders| bit  |
| &#128270; | ceiling\_design\_committed| bit  |
| &#128270; | main\_contractor\_contacts| bit  |
| &#128270; | dfm\_review\_date| datetime2(26)  |
| &#128270; | user| varchar(8000)  |
| &#128270; | dfm\_review\_required| bit  |
| &#128270; | sub\_contractor\_awarded| bit  |
| &#128270; | sub\_contractor\_engagement| bit  |
| &#128270; | architect\_contacts\_reason| varchar(8000)  |
| &#128270; | architect\_listed\_reason| varchar(8000)  |
| &#128270; | engaged\_with\_architect\_reason| varchar(8000)  |
| &#128270; | main\_contractor\_bidders\_reason| varchar(8000)  |
| &#128270; | main\_contractor\_contact\_reason| varchar(8000)  |
| &#128270; | specification\_issued\_reason| varchar(8000)  |
| &#128270; | sub\_contractor\_awarded\_reason| varchar(8000)  |
| &#128270; | sub\_contractor\_bidders\_reason| varchar(8000)  |
| &#128270; | fit\_out\_type| varchar(8000)  |
| &#128270; | sub\_contract\_award\_percentage| decimal(38,18)  |
| &#128270; | project\_manager\_ref| varchar(8000)  |
| &#128270; | introduction\_percentage| decimal(38,18)  |
| &#128270; | db\_m\_contractor\_records| decimal(38,18)  |
| &#128270; | main\_contract\_award\_percentage| decimal(38,18)  |
| &#128270; | project\_design\_percentage| decimal(38,18)  |
| &#128270; | infor\_error| varchar(8000)  |
| &#128270; | infor\_last\_updated| datetime2(26)  |
| &#128270; | infor\_status| varchar(8000)  |
| &#128270; | distributor\_records| decimal(38,18)  |
| &#128270; | sc\_subcontractor\_records| decimal(38,18)  |
| &#128270; | project\_estimated\_end\_date| datetime2(26)  |
| &#128270; | lost\_to\_product| varchar(8000)  |
| &#128270; | construction\_manager\_records| decimal(38,18)  |
| &#128270; | proposal\_number| varchar(8000)  |
| &#128270; | secured\_reason| varchar(8000)  |
| &#128270; | business\_commercial\_sign\_off| bit  |
| &#128270; | bcr\_estimate\_request\_no| varchar(8000)  |
| &#128270; | bcr\_sign\_off\_date| datetime2(26)  |
| &#128270; | dfm\_estimate\_request\_no| varchar(8000)  |
| &#128270; | dfm\_sign\_off\_date| datetime2(26)  |
| &#128270; | dfm\_signed\_off| bit  |
| &#128270; | tender\_percentage| decimal(38,18)  |
| &#128270; | architect\_contact\_records| decimal(38,18)  |
| &#128270; | client\_contact\_records| decimal(38,18)  |
| &#128270; | main\_contractor\_contact\_records| decimal(38,18)  |
| &#128270; | sub\_contractor\_bidder\_records| decimal(38,18)  |
| &#128270; | case\_study\_required| bit  |
| &#128270; | case\_study\_request\_date| datetime2(26)  |
| &#128270; | original\_project| varchar(8000)  |
| &#128270; | take\_back\_type| varchar(8000)  |
| &#128270; | approximate\_sqm| decimal(38,18)  |
| &#128270; | sqm\_value| decimal(38,18)  |
| &#128270; | approximate\_value| decimal(38,18)  |
| &#128270; | carbon\_saving| decimal(38,18)  |
| &#128270; | estimated\_yield| decimal(38,18)  |
| &#128270; | net\_yield| decimal(38,18)  |
| &#128270; | resale\_rate\_sqm| decimal(38,18)  |
| &#128270; | on\_hold| bit  |
| &#128270; | project\_updated| bit  |
| &#128270; | sbaa\_approval\_status| varchar(8000)  |
| &#128270; | marketing\_review\_by| varchar(8000)  |
| &#128270; | marketing\_review| bit  |
| &#128270; | sbaa\_approval\_step| decimal(38,18)  |
| &#128270; | sbaa\_approver| varchar(8000)  |
| &#128270; | sbaa\_step\_approved| bit  |
| &#128270; | sbaa\_submitted\_date| datetime2(26)  |
| &#128270; | sbaa\_submitted\_user| varchar(8000)  |
| &#128270; | sbqq\_amended\_contract| varchar(8000)  |
| &#128270; | sbqq\_contracted| bit  |
| &#128270; | sbqq\_create\_contracted\_prices| bit  |
| &#128270; | sbqq\_order\_group\_id| varchar(8000)  |
| &#128270; | sbqq\_ordered| bit  |
| &#128270; | target\_market\_value| varchar(8000)  |
| &#128270; | target\_sales\_price| varchar(8000)  |
| &#128270; | sbqq\_primary\_quote| varchar(8000)  |
| &#128270; | sbqq\_quote\_pricebook\_id| varchar(8000)  |
| &#128270; | sbqq\_renewal| bit  |
| &#128270; | sbqq\_renewed\_contract| varchar(8000)  |
| &#128270; | build\_schedules\_status| varchar(8000)  |
| &#128270; | override\_schedule\_quantity| decimal(38,18)  |
| &#128270; | state| varchar(8000)  |
| &#128270; | link\_to\_planning| varchar(8000)  |
| &#128270; | planning\_reference| varchar(8000)  |
| &#128270; | design\_sign\_off\_by| varchar(8000)  |
| &#128270; | review\_required\_date| datetime2(26)  |
| &#128270; | project\_figures\_reported\_date| datetime2(26)  |
| &#128270; | primary\_sector| varchar(8000)  |
| &#128270; | weeks\_between\_order\_delivery| decimal(38,18)  |
| &#128270; | sector\_count| decimal(38,18)  |
| &#128270; | last\_activity| varchar(8000)  |
| &#128270; | product\_overview| varchar(8000)  |
| &#128270; | quote\_status| varchar(8000)  |
| &#128270; | project\_transfer\_value| decimal(38,18)  |
| &#128270; | researcher| varchar(8000)  |
| &#128270; | me\_contractor\_records| decimal(38,18)  |
| &#128270; | estimated\_project\_margin| decimal(38,18)  |
| &#128270; | push\_counter| decimal(38,18)  |
| &#128270; | project\_primary\_quoted\_date| datetime2(26)  |
| &#128270; | quote\_records| decimal(38,18)  |
| &#128270; | proposal\_records| decimal(38,18)  |
| &#128270; | proactive| bit  |
| &#128270; | original\_quoted\_value| decimal(38,18)  |
| &#128270; | building\_value| decimal(38,18)  |
| &#128270; | quote\_to\_ordered\_status| varchar(8000)  |
| &#128270; | primary\_quotes| decimal(38,18)  |
| &#128270; | x2025\_budgeted\_project\_value| decimal(38,18)  |
| &#128270; | x2025\_budgeted\_forecast\_amount| decimal(38,18)  |
| &#128270; | x2025\_budgeted\_probability| decimal(38,18)  |
| &#128270; | construction\_timeline| varchar(8000)  |
| &#128270; | quotes\_rollup| decimal(38,18)  |
| &#128270; | nda\_start\_date| datetime2(26)  |
| &#128270; | nda\_expiry\_date| datetime2(26)  |
| &#128270; | main\_contractor\_awarded| bit  |
| &#128270; | sas\_specified| bit  |
| &#128270; | x2025\_budgeted\_order\_date| datetime2(26)  |
| &#128270; | main\_contractor\_tender\_date| datetime2(26)  |
| &#128270; | x2025\_budgeted\_first\_delivery\_date| datetime2(26)  |
| &#128270; | order\_tracking\_records| decimal(38,18)  |
| &#128270; | met\_with\_architect| bit  |
| &#128270; | open\_task\_records| decimal(38,18)  |
| &#128270; | primary\_estimate\_value| decimal(38,18)  |
| &#128270; | opportunity\_sqm\_roll\_up| decimal(38,18)  |
| &#128270; | figures\_quote\_records| decimal(38,18)  |
| &#128270; | figures\_estimate\_records| decimal(38,18)  |
| &#128270; | strategic\_support| bit  |
| &#128270; | project\_manager| varchar(8000)  |
| &#128270; | billing\_contact| varchar(8000)  |
| &#128270; | shipping\_contact| varchar(8000)  |
| &#128270; | shipping\_address| varchar(8000)  |
| &#128270; | order\_tracking\_status| varchar(8000)  |
| &#128270; | customer\_credit| varchar(8000)  |
| &#128270; | tax\_exempt| varchar(8000)  |
| &#128270; | roe| decimal(38,18)  |
| &#128270; | po\_number| varchar(8000)  |
| &#128270; | po\_value| decimal(38,18)  |
| &#128270; | po\_received\_date| datetime2(26)  |
| &#128270; | change\_orders| varchar(8000)  |
| &#128270; | securing\_manufacturer\_check| bit  |
| &#128270; | change\_order\_value| decimal(38,18)  |
| &#128270; | proforma\_value| decimal(38,18)  |
| &#128270; | specification\_provided| bit  |
| &#128270; | tariff\_value| varchar(8000)  |
| &#128270; | estimated\_gm| decimal(38,18)  |
| &#128270; | shops\_approved\_date| datetime2(26)  |
| &#128270; | deposit\_payment\_date| datetime2(26)  |
| &#128270; | final\_delivery\_date| datetime2(26)  |
| &#128270; | who\_is\_specified| bit  |
| &#128270; | final\_dispatch\_date| datetime2(26)  |
| &#128270; | estimate\_reference| varchar(8000)  |
| &#128270; | order\_tracking\_company| varchar(8000)  |
| &#128270; | architect\_records| decimal(38,18)  |
| &#128270; | client\_records| decimal(38,18)  |
| &#128270; | developer\_records| decimal(38,18)  |
| &#128270; | main\_contractor\_bidders| decimal(38,18)  |
| &#128270; | stage\_text| varchar(8000)  |
| &#128270; | no\_of\_products| decimal(38,18)  |
| &#128270; | number\_of\_schedules| decimal(38,18)  |
| &#128270; | subcontractor\_tender\_records| decimal(38,18)  |
| &#128270; | primary\_quote\_date| datetime2(26)  |
| &#128270; | gate\_2\_approval| bit  |
| &#128270; | gate\_2\_approval\_date| datetime2(26)  |
| &#128270; | gate\_3\_approval| bit  |
| &#128270; | gate\_3\_approval\_date| datetime2(26)  |
| &#128270; | main\_contractor\_awarded\_reason| varchar(8000)  |
| &#128270; | gate\_4\_approval| bit  |
| &#128270; | gate\_4\_approval\_date| datetime2(26)  |
| &#128270; | met\_with\_architect\_reason| varchar(8000)  |
| &#128270; | sales\_quote\_review| bit  |
| &#128270; | deleted\_ts| datetime2(26)  |
| &#128270; | lost\_project\_ts| datetime2(26)  |
| &#128270; | timeline\_reason| varchar(8000)  |
| &#128270; | project\_next\_task\_date| datetime2(26)  |
| &#128270; | opportunity\_sqm\_copy| decimal(38,18)  |
| &#128270; | opportunity\_value\_copy| decimal(38,18)  |
| &#128270; | primary\_estimates| decimal(38,18)  |
| &#128270; | usa\_configuration\_specified| bit  |
| &#128270; | project\_engagement\_count| decimal(38,18)  |
| &#128270; | configuration\_specified\_date| datetime2(26)  |
| &#128270; | horizon\_specification\_issued| bit  |
| &#128270; | product\_type| varchar(8000)  |
| &#128270; | x2024\_budget\_order\_date| varchar(8000)  |
| &#128270; | x2024\_budget\_delivery\_to\_site| varchar(8000)  |
| &#128270; | x2024\_budget\_opportunity\_value| varchar(8000)  |
| &#128270; | x2024\_budget\_forecasted\_value| varchar(8000)  |
| &#128270; | x2024\_budget\_project\_probability| varchar(8000)  |
| &#128270; | x2024\_budget\_stage| varchar(8000)  |
| &#128270; | x2024\_budget\_construction\_stage| varchar(8000)  |
| &#128270; | x2024\_budget\_qualification\_percentage| varchar(8000)  |
| &#128270; | x2024\_budget\_introduction\_percentage| varchar(8000)  |
| &#128270; | x2024\_budget\_specification\_percentage| varchar(8000)  |
| &#128270; | x2024\_budget\_commercial\_strategy| varchar(8000)  |
| &#128270; | x2024\_budget\_negotiation\_percentage| varchar(8000)  |
| &#128270; | total\_project\_percentage| decimal(38,18)  |
| &#128270; | date\_change\_reason| varchar(8000)  |
| &#128270; | project\_engagement| bit  |
| &#128270; | total\_opportunity\_sqm| decimal(38,18)  |
| &#128270; | estimated\_sqm| decimal(38,18)  |
| &#128270; | first\_delivery\_on\_site| datetime2(26)  |
| &#128270; | estimate\_records| decimal(38,18)  |
| &#128270; | estimates\_issued\_percentage| decimal(38,18)  |
| &#128270; | master\_project| varchar(8000)  |
| &#128270; | total\_projects\_value| decimal(38,18)  |
| &#128270; | product\_type\_if\_other| varchar(8000)  |
| &#128270; | x2024\_budget\_value\_currency| decimal(38,18)  |
| &#128270; | x2024\_delivery\_to\_site\_date| datetime2(26)  |
| &#128270; | x2024\_order\_date\_date| datetime2(26)  |
| &#128270; | major\_priority\_project| bit  |
| &#128270; | project\_complexity| varchar(8000)  |
| &#128270; | planning\_approved| bit  |
| &#128270; | manf\_location| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON account\_id|
| &#128270;  | ClusteredIndex | ON record\_type\_id|
| &#128270;  | ClusteredIndex | ON is\_private|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON stage\_name|
| &#128270;  | ClusteredIndex | ON amount|
| &#128270;  | ClusteredIndex | ON probability|
| &#128270;  | ClusteredIndex | ON expected\_revenue|
| &#128270;  | ClusteredIndex | ON total\_opportunity\_quantity|
| &#128270;  | ClusteredIndex | ON close\_date|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON next\_step|
| &#128270;  | ClusteredIndex | ON lead\_source|
| &#128270;  | ClusteredIndex | ON is\_closed|
| &#128270;  | ClusteredIndex | ON is\_won|
| &#128270;  | ClusteredIndex | ON forecast\_category|
| &#128270;  | ClusteredIndex | ON forecast\_category\_name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON campaign\_id|
| &#128270;  | ClusteredIndex | ON has\_opportunity\_line\_item|
| &#128270;  | ClusteredIndex | ON pricebook2\_id|
| &#128270;  | ClusteredIndex | ON owner\_id|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON fiscal\_quarter|
| &#128270;  | ClusteredIndex | ON fiscal\_year|
| &#128270;  | ClusteredIndex | ON fiscal|
| &#128270;  | ClusteredIndex | ON contact\_id|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON contract\_id|
| &#128270;  | ClusteredIndex | ON has\_open\_activity|
| &#128270;  | ClusteredIndex | ON has\_overdue\_task|
| &#128270;  | ClusteredIndex | ON merge\_field|
| &#128270;  | ClusteredIndex | ON submarket|
| &#128270;  | ClusteredIndex | ON net\_internal\_area|
| &#128270;  | ClusteredIndex | ON additional\_address\_line|
| &#128270;  | ClusteredIndex | ON loss\_reason|
| &#128270;  | ClusteredIndex | ON address|
| &#128270;  | ClusteredIndex | ON balance|
| &#128270;  | ClusteredIndex | ON build\_type|
| &#128270;  | ClusteredIndex | ON building\_name\_number|
| &#128270;  | ClusteredIndex | ON contact|
| &#128270;  | ClusteredIndex | ON country|
| &#128270;  | ClusteredIndex | ON custom\_rollup\_summary|
| &#128270;  | ClusteredIndex | ON deleted\_reason|
| &#128270;  | ClusteredIndex | ON forecasted\_sqm|
| &#128270;  | ClusteredIndex | ON forecasted\_value|
| &#128270;  | ClusteredIndex | ON infor\_reference\_number|
| &#128270;  | ClusteredIndex | ON last\_interaction\_date|
| &#128270;  | ClusteredIndex | ON lead\_reference|
| &#128270;  | ClusteredIndex | ON lease\_expiry\_follow\_up|
| &#128270;  | ClusteredIndex | ON link\_to\_external\_lead|
| &#128270;  | ClusteredIndex | ON lost\_deleted\_additional\_info|
| &#128270;  | ClusteredIndex | ON securing\_manufacturer|
| &#128270;  | ClusteredIndex | ON marketing\_additional\_info|
| &#128270;  | ClusteredIndex | ON new\_proposal|
| &#128270;  | ClusteredIndex | ON notes|
| &#128270;  | ClusteredIndex | ON opportunity\_sqm|
| &#128270;  | ClusteredIndex | ON opportunity\_value|
| &#128270;  | ClusteredIndex | ON order\_date|
| &#128270;  | ClusteredIndex | ON order\_sqm|
| &#128270;  | ClusteredIndex | ON order\_value|
| &#128270;  | ClusteredIndex | ON pass\_to\_marketing|
| &#128270;  | ClusteredIndex | ON photo\_available\_date|
| &#128270;  | ClusteredIndex | ON postcode|
| &#128270;  | ClusteredIndex | ON project\_alternative\_name|
| &#128270;  | ClusteredIndex | ON project\_complete|
| &#128270;  | ClusteredIndex | ON budget\_value|
| &#128270;  | ClusteredIndex | ON project\_concern\_info|
| &#128270;  | ClusteredIndex | ON project\_concerns|
| &#128270;  | ClusteredIndex | ON project\_delivery\_date\_from|
| &#128270;  | ClusteredIndex | ON project\_delivery\_date\_to|
| &#128270;  | ClusteredIndex | ON project\_estimated\_start\_date|
| &#128270;  | ClusteredIndex | ON project\_probability|
| &#128270;  | ClusteredIndex | ON proposal\_issued|
| &#128270;  | ClusteredIndex | ON proposal\_issued\_date|
| &#128270;  | ClusteredIndex | ON push\_count|
| &#128270;  | ClusteredIndex | ON reason\_for\_raising\_a\_project|
| &#128270;  | ClusteredIndex | ON red\_flag\_removal\_reason|
| &#128270;  | ClusteredIndex | ON red\_flag\_status\_old\_values|
| &#128270;  | ClusteredIndex | ON region|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON sales\_region|
| &#128270;  | ClusteredIndex | ON scheme|
| &#128270;  | ClusteredIndex | ON secondary\_owner|
| &#128270;  | ClusteredIndex | ON secondary\_source|
| &#128270;  | ClusteredIndex | ON sharepoint|
| &#128270;  | ClusteredIndex | ON source\_if\_other|
| &#128270;  | ClusteredIndex | ON specification\_detail|
| &#128270;  | ClusteredIndex | ON street\_address|
| &#128270;  | ClusteredIndex | ON total\_opportunity\_size\_sqm|
| &#128270;  | ClusteredIndex | ON town|
| &#128270;  | ClusteredIndex | ON estimates\_rollup|
| &#128270;  | ClusteredIndex | ON main\_contractor\_records|
| &#128270;  | ClusteredIndex | ON sub\_contractor\_records|
| &#128270;  | ClusteredIndex | ON opportunity\_sqm\_two|
| &#128270;  | ClusteredIndex | ON product\_count|
| &#128270;  | ClusteredIndex | ON project\_owner|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_required|
| &#128270;  | ClusteredIndex | ON business\_commercial\_review\_required|
| &#128270;  | ClusteredIndex | ON typical\_floor\_size|
| &#128270;  | ClusteredIndex | ON verified|
| &#128270;  | ClusteredIndex | ON number\_of\_floors|
| &#128270;  | ClusteredIndex | ON architect\_contacts\_checkbox|
| &#128270;  | ClusteredIndex | ON engaged\_with\_architect|
| &#128270;  | ClusteredIndex | ON architect\_listed|
| &#128270;  | ClusteredIndex | ON concept\_source|
| &#128270;  | ClusteredIndex | ON client\_listed|
| &#128270;  | ClusteredIndex | ON opportunity\_sign\_off|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_date|
| &#128270;  | ClusteredIndex | ON opportunity\_sign\_off\_by|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_notes|
| &#128270;  | ClusteredIndex | ON client\_contact\_listed|
| &#128270;  | ClusteredIndex | ON design\_review\_by|
| &#128270;  | ClusteredIndex | ON design\_review|
| &#128270;  | ClusteredIndex | ON budget\_provided|
| &#128270;  | ClusteredIndex | ON construction\_dates\_provided|
| &#128270;  | ClusteredIndex | ON products\_specified\_checkbox|
| &#128270;  | ClusteredIndex | ON proposal\_issued\_checkbox|
| &#128270;  | ClusteredIndex | ON competitor\_project\_value|
| &#128270;  | ClusteredIndex | ON specification\_issued|
| &#128270;  | ClusteredIndex | ON estimates\_sent|
| &#128270;  | ClusteredIndex | ON project\_images|
| &#128270;  | ClusteredIndex | ON final\_target\_market\_value|
| &#128270;  | ClusteredIndex | ON final\_target\_sales\_price|
| &#128270;  | ClusteredIndex | ON main\_contractor\_bidders\_provided|
| &#128270;  | ClusteredIndex | ON main\_contractor\_engagement|
| &#128270;  | ClusteredIndex | ON fit\_out\_contractor\_records|
| &#128270;  | ClusteredIndex | ON nda\_signed|
| &#128270;  | ClusteredIndex | ON special\_projects\_reference|
| &#128270;  | ClusteredIndex | ON prior\_stage|
| &#128270;  | ClusteredIndex | ON sub\_contractor\_bidders|
| &#128270;  | ClusteredIndex | ON ceiling\_design\_committed|
| &#128270;  | ClusteredIndex | ON main\_contractor\_contacts|
| &#128270;  | ClusteredIndex | ON dfm\_review\_date|
| &#128270;  | ClusteredIndex | ON user|
| &#128270;  | ClusteredIndex | ON dfm\_review\_required|
| &#128270;  | ClusteredIndex | ON sub\_contractor\_awarded|
| &#128270;  | ClusteredIndex | ON sub\_contractor\_engagement|
| &#128270;  | ClusteredIndex | ON architect\_contacts\_reason|
| &#128270;  | ClusteredIndex | ON architect\_listed\_reason|
| &#128270;  | ClusteredIndex | ON engaged\_with\_architect\_reason|
| &#128270;  | ClusteredIndex | ON main\_contractor\_bidders\_reason|
| &#128270;  | ClusteredIndex | ON main\_contractor\_contact\_reason|
| &#128270;  | ClusteredIndex | ON specification\_issued\_reason|
| &#128270;  | ClusteredIndex | ON sub\_contractor\_awarded\_reason|
| &#128270;  | ClusteredIndex | ON sub\_contractor\_bidders\_reason|
| &#128270;  | ClusteredIndex | ON fit\_out\_type|
| &#128270;  | ClusteredIndex | ON sub\_contract\_award\_percentage|
| &#128270;  | ClusteredIndex | ON project\_manager\_ref|
| &#128270;  | ClusteredIndex | ON introduction\_percentage|
| &#128270;  | ClusteredIndex | ON db\_m\_contractor\_records|
| &#128270;  | ClusteredIndex | ON main\_contract\_award\_percentage|
| &#128270;  | ClusteredIndex | ON project\_design\_percentage|
| &#128270;  | ClusteredIndex | ON infor\_error|
| &#128270;  | ClusteredIndex | ON infor\_last\_updated|
| &#128270;  | ClusteredIndex | ON infor\_status|
| &#128270;  | ClusteredIndex | ON distributor\_records|
| &#128270;  | ClusteredIndex | ON sc\_subcontractor\_records|
| &#128270;  | ClusteredIndex | ON project\_estimated\_end\_date|
| &#128270;  | ClusteredIndex | ON lost\_to\_product|
| &#128270;  | ClusteredIndex | ON construction\_manager\_records|
| &#128270;  | ClusteredIndex | ON proposal\_number|
| &#128270;  | ClusteredIndex | ON secured\_reason|
| &#128270;  | ClusteredIndex | ON business\_commercial\_sign\_off|
| &#128270;  | ClusteredIndex | ON bcr\_estimate\_request\_no|
| &#128270;  | ClusteredIndex | ON bcr\_sign\_off\_date|
| &#128270;  | ClusteredIndex | ON dfm\_estimate\_request\_no|
| &#128270;  | ClusteredIndex | ON dfm\_sign\_off\_date|
| &#128270;  | ClusteredIndex | ON dfm\_signed\_off|
| &#128270;  | ClusteredIndex | ON tender\_percentage|
| &#128270;  | ClusteredIndex | ON architect\_contact\_records|
| &#128270;  | ClusteredIndex | ON client\_contact\_records|
| &#128270;  | ClusteredIndex | ON main\_contractor\_contact\_records|
| &#128270;  | ClusteredIndex | ON sub\_contractor\_bidder\_records|
| &#128270;  | ClusteredIndex | ON case\_study\_required|
| &#128270;  | ClusteredIndex | ON case\_study\_request\_date|
| &#128270;  | ClusteredIndex | ON original\_project|
| &#128270;  | ClusteredIndex | ON take\_back\_type|
| &#128270;  | ClusteredIndex | ON approximate\_sqm|
| &#128270;  | ClusteredIndex | ON sqm\_value|
| &#128270;  | ClusteredIndex | ON approximate\_value|
| &#128270;  | ClusteredIndex | ON carbon\_saving|
| &#128270;  | ClusteredIndex | ON estimated\_yield|
| &#128270;  | ClusteredIndex | ON net\_yield|
| &#128270;  | ClusteredIndex | ON resale\_rate\_sqm|
| &#128270;  | ClusteredIndex | ON on\_hold|
| &#128270;  | ClusteredIndex | ON project\_updated|
| &#128270;  | ClusteredIndex | ON sbaa\_approval\_status|
| &#128270;  | ClusteredIndex | ON marketing\_review\_by|
| &#128270;  | ClusteredIndex | ON marketing\_review|
| &#128270;  | ClusteredIndex | ON sbaa\_approval\_step|
| &#128270;  | ClusteredIndex | ON sbaa\_approver|
| &#128270;  | ClusteredIndex | ON sbaa\_step\_approved|
| &#128270;  | ClusteredIndex | ON sbaa\_submitted\_date|
| &#128270;  | ClusteredIndex | ON sbaa\_submitted\_user|
| &#128270;  | ClusteredIndex | ON sbqq\_amended\_contract|
| &#128270;  | ClusteredIndex | ON sbqq\_contracted|
| &#128270;  | ClusteredIndex | ON sbqq\_create\_contracted\_prices|
| &#128270;  | ClusteredIndex | ON sbqq\_order\_group\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_ordered|
| &#128270;  | ClusteredIndex | ON target\_market\_value|
| &#128270;  | ClusteredIndex | ON target\_sales\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_primary\_quote|
| &#128270;  | ClusteredIndex | ON sbqq\_quote\_pricebook\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_renewal|
| &#128270;  | ClusteredIndex | ON sbqq\_renewed\_contract|
| &#128270;  | ClusteredIndex | ON build\_schedules\_status|
| &#128270;  | ClusteredIndex | ON override\_schedule\_quantity|
| &#128270;  | ClusteredIndex | ON state|
| &#128270;  | ClusteredIndex | ON link\_to\_planning|
| &#128270;  | ClusteredIndex | ON planning\_reference|
| &#128270;  | ClusteredIndex | ON design\_sign\_off\_by|
| &#128270;  | ClusteredIndex | ON review\_required\_date|
| &#128270;  | ClusteredIndex | ON project\_figures\_reported\_date|
| &#128270;  | ClusteredIndex | ON primary\_sector|
| &#128270;  | ClusteredIndex | ON weeks\_between\_order\_delivery|
| &#128270;  | ClusteredIndex | ON sector\_count|
| &#128270;  | ClusteredIndex | ON last\_activity|
| &#128270;  | ClusteredIndex | ON product\_overview|
| &#128270;  | ClusteredIndex | ON quote\_status|
| &#128270;  | ClusteredIndex | ON project\_transfer\_value|
| &#128270;  | ClusteredIndex | ON researcher|
| &#128270;  | ClusteredIndex | ON me\_contractor\_records|
| &#128270;  | ClusteredIndex | ON estimated\_project\_margin|
| &#128270;  | ClusteredIndex | ON push\_counter|
| &#128270;  | ClusteredIndex | ON project\_primary\_quoted\_date|
| &#128270;  | ClusteredIndex | ON quote\_records|
| &#128270;  | ClusteredIndex | ON proposal\_records|
| &#128270;  | ClusteredIndex | ON proactive|
| &#128270;  | ClusteredIndex | ON original\_quoted\_value|
| &#128270;  | ClusteredIndex | ON building\_value|
| &#128270;  | ClusteredIndex | ON quote\_to\_ordered\_status|
| &#128270;  | ClusteredIndex | ON primary\_quotes|
| &#128270;  | ClusteredIndex | ON x2025\_budgeted\_project\_value|
| &#128270;  | ClusteredIndex | ON x2025\_budgeted\_forecast\_amount|
| &#128270;  | ClusteredIndex | ON x2025\_budgeted\_probability|
| &#128270;  | ClusteredIndex | ON construction\_timeline|
| &#128270;  | ClusteredIndex | ON quotes\_rollup|
| &#128270;  | ClusteredIndex | ON nda\_start\_date|
| &#128270;  | ClusteredIndex | ON nda\_expiry\_date|
| &#128270;  | ClusteredIndex | ON main\_contractor\_awarded|
| &#128270;  | ClusteredIndex | ON sas\_specified|
| &#128270;  | ClusteredIndex | ON x2025\_budgeted\_order\_date|
| &#128270;  | ClusteredIndex | ON main\_contractor\_tender\_date|
| &#128270;  | ClusteredIndex | ON x2025\_budgeted\_first\_delivery\_date|
| &#128270;  | ClusteredIndex | ON order\_tracking\_records|
| &#128270;  | ClusteredIndex | ON met\_with\_architect|
| &#128270;  | ClusteredIndex | ON open\_task\_records|
| &#128270;  | ClusteredIndex | ON primary\_estimate\_value|
| &#128270;  | ClusteredIndex | ON opportunity\_sqm\_roll\_up|
| &#128270;  | ClusteredIndex | ON figures\_quote\_records|
| &#128270;  | ClusteredIndex | ON figures\_estimate\_records|
| &#128270;  | ClusteredIndex | ON strategic\_support|
| &#128270;  | ClusteredIndex | ON project\_manager|
| &#128270;  | ClusteredIndex | ON billing\_contact|
| &#128270;  | ClusteredIndex | ON shipping\_contact|
| &#128270;  | ClusteredIndex | ON shipping\_address|
| &#128270;  | ClusteredIndex | ON order\_tracking\_status|
| &#128270;  | ClusteredIndex | ON customer\_credit|
| &#128270;  | ClusteredIndex | ON tax\_exempt|
| &#128270;  | ClusteredIndex | ON roe|
| &#128270;  | ClusteredIndex | ON po\_number|
| &#128270;  | ClusteredIndex | ON po\_value|
| &#128270;  | ClusteredIndex | ON po\_received\_date|
| &#128270;  | ClusteredIndex | ON change\_orders|
| &#128270;  | ClusteredIndex | ON securing\_manufacturer\_check|
| &#128270;  | ClusteredIndex | ON change\_order\_value|
| &#128270;  | ClusteredIndex | ON proforma\_value|
| &#128270;  | ClusteredIndex | ON specification\_provided|
| &#128270;  | ClusteredIndex | ON tariff\_value|
| &#128270;  | ClusteredIndex | ON estimated\_gm|
| &#128270;  | ClusteredIndex | ON shops\_approved\_date|
| &#128270;  | ClusteredIndex | ON deposit\_payment\_date|
| &#128270;  | ClusteredIndex | ON final\_delivery\_date|
| &#128270;  | ClusteredIndex | ON who\_is\_specified|
| &#128270;  | ClusteredIndex | ON final\_dispatch\_date|
| &#128270;  | ClusteredIndex | ON estimate\_reference|
| &#128270;  | ClusteredIndex | ON order\_tracking\_company|
| &#128270;  | ClusteredIndex | ON architect\_records|
| &#128270;  | ClusteredIndex | ON client\_records|
| &#128270;  | ClusteredIndex | ON developer\_records|
| &#128270;  | ClusteredIndex | ON main\_contractor\_bidders|
| &#128270;  | ClusteredIndex | ON stage\_text|
| &#128270;  | ClusteredIndex | ON no\_of\_products|
| &#128270;  | ClusteredIndex | ON number\_of\_schedules|
| &#128270;  | ClusteredIndex | ON subcontractor\_tender\_records|
| &#128270;  | ClusteredIndex | ON primary\_quote\_date|
| &#128270;  | ClusteredIndex | ON gate\_2\_approval|
| &#128270;  | ClusteredIndex | ON gate\_2\_approval\_date|
| &#128270;  | ClusteredIndex | ON gate\_3\_approval|
| &#128270;  | ClusteredIndex | ON gate\_3\_approval\_date|
| &#128270;  | ClusteredIndex | ON main\_contractor\_awarded\_reason|
| &#128270;  | ClusteredIndex | ON gate\_4\_approval|
| &#128270;  | ClusteredIndex | ON gate\_4\_approval\_date|
| &#128270;  | ClusteredIndex | ON met\_with\_architect\_reason|
| &#128270;  | ClusteredIndex | ON sales\_quote\_review|
| &#128270;  | ClusteredIndex | ON deleted\_ts|
| &#128270;  | ClusteredIndex | ON lost\_project\_ts|
| &#128270;  | ClusteredIndex | ON timeline\_reason|
| &#128270;  | ClusteredIndex | ON project\_next\_task\_date|
| &#128270;  | ClusteredIndex | ON opportunity\_sqm\_copy|
| &#128270;  | ClusteredIndex | ON opportunity\_value\_copy|
| &#128270;  | ClusteredIndex | ON primary\_estimates|
| &#128270;  | ClusteredIndex | ON usa\_configuration\_specified|
| &#128270;  | ClusteredIndex | ON project\_engagement\_count|
| &#128270;  | ClusteredIndex | ON configuration\_specified\_date|
| &#128270;  | ClusteredIndex | ON horizon\_specification\_issued|
| &#128270;  | ClusteredIndex | ON product\_type|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_order\_date|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_delivery\_to\_site|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_opportunity\_value|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_forecasted\_value|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_project\_probability|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_stage|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_construction\_stage|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_qualification\_percentage|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_introduction\_percentage|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_specification\_percentage|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_commercial\_strategy|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_negotiation\_percentage|
| &#128270;  | ClusteredIndex | ON total\_project\_percentage|
| &#128270;  | ClusteredIndex | ON date\_change\_reason|
| &#128270;  | ClusteredIndex | ON project\_engagement|
| &#128270;  | ClusteredIndex | ON total\_opportunity\_sqm|
| &#128270;  | ClusteredIndex | ON estimated\_sqm|
| &#128270;  | ClusteredIndex | ON first\_delivery\_on\_site|
| &#128270;  | ClusteredIndex | ON estimate\_records|
| &#128270;  | ClusteredIndex | ON estimates\_issued\_percentage|
| &#128270;  | ClusteredIndex | ON master\_project|
| &#128270;  | ClusteredIndex | ON total\_projects\_value|
| &#128270;  | ClusteredIndex | ON product\_type\_if\_other|
| &#128270;  | ClusteredIndex | ON x2024\_budget\_value\_currency|
| &#128270;  | ClusteredIndex | ON x2024\_delivery\_to\_site\_date|
| &#128270;  | ClusteredIndex | ON x2024\_order\_date\_date|
| &#128270;  | ClusteredIndex | ON major\_priority\_project|
| &#128270;  | ClusteredIndex | ON project\_complexity|
| &#128270;  | ClusteredIndex | ON planning\_approved|
| &#128270;  | ClusteredIndex | ON manf\_location|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.order_tracking 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | owner\_id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | record\_type\_id| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | status| varchar(8000)  |
| &#128270; | project\_name| varchar(8000)  |
| &#128270; | company\_name| varchar(8000)  |
| &#128270; | contact\_name| varchar(8000)  |
| &#128270; | pending\_reason\_formula| varchar(8000)  |
| &#128270; | sample\_mock\_up| varchar(8000)  |
| &#128270; | factory\_manager| varchar(8000)  |
| &#128270; | order\_number| varchar(8000)  |
| &#128270; | po\_received| datetime2(26)  |
| &#128270; | po\_value| decimal(38,18)  |
| &#128270; | days\_in\_to\_be\_acknowledged| decimal(38,18)  |
| &#128270; | deposit\_proforma\_issued| datetime2(26)  |
| &#128270; | proforma\_value| decimal(38,18)  |
| &#128270; | payment\_received| datetime2(26)  |
| &#128270; | sign\_off\_notes| varchar(8000)  |
| &#128270; | chase\_date| datetime2(26)  |
| &#128270; | days\_in\_estimating| decimal(38,18)  |
| &#128270; | submittal\_issued| datetime2(26)  |
| &#128270; | submittals\_approved| datetime2(26)  |
| &#128270; | handover\_to\_so| datetime2(26)  |
| &#128270; | department\_to\_chase| varchar(8000)  |
| &#128270; | stage| varchar(8000)  |
| &#128270; | product\_into\_engineering\_planning| datetime2(26)  |
| &#128270; | no\_of\_chases| decimal(38,18)  |
| &#128270; | order\_lines\_dated\_on\_factory\_book| datetime2(26)  |
| &#128270; | last\_chase\_date| datetime2(26)  |
| &#128270; | order\_acknowledgement\_sent\_to\_customer| datetime2(26)  |
| &#128270; | date\_shipped\_out\_of\_factory| datetime2(26)  |
| &#128270; | value\_due| decimal(38,18)  |
| &#128270; | due\_by| datetime2(26)  |
| &#128270; | infor\_references| varchar(8000)  |
| &#128270; | shipping\_method| varchar(8000)  |
| &#128270; | pkgs| decimal(38,18)  |
| &#128270; | ets| varchar(8000)  |
| &#128270; | eta| varchar(8000)  |
| &#128270; | shipment\_notice\_issued\_to\_customer| datetime2(26)  |
| &#128270; | owner\_and\_reason| varchar(8000)  |
| &#128270; | project\_owner| varchar(8000)  |
| &#128270; | project\_secondary\_owner| varchar(8000)  |
| &#128270; | project\_stage| varchar(8000)  |
| &#128270; | project\_probability| varchar(8000)  |
| &#128270; | project\_specification| varchar(8000)  |
| &#128270; | in\_contract\_start\_date| datetime2(26)  |
| &#128270; | in\_contract\_end\_date| datetime2(26)  |
| &#128270; | shops\_submittals\_start\_date| datetime2(26)  |
| &#128270; | shops\_submittals\_end\_date| datetime2(26)  |
| &#128270; | handover\_st2\_start\_date| datetime2(26)  |
| &#128270; | handover\_st2\_end\_date| datetime2(26)  |
| &#128270; | engineering\_planning\_start\_date| datetime2(26)  |
| &#128270; | engineering\_planning\_end\_date| datetime2(26)  |
| &#128270; | production\_start\_date| datetime2(26)  |
| &#128270; | production\_end\_date| datetime2(26)  |
| &#128270; | shipping\_in\_transit\_start\_date| datetime2(26)  |
| &#128270; | shipping\_in\_transit\_end\_date| datetime2(26)  |
| &#128270; | balance\_payable\_start\_date| datetime2(26)  |
| &#128270; | balance\_payable\_end\_date| datetime2(26)  |
| &#128270; | in\_contract\_started| bit  |
| &#128270; | shops\_submittals\_started| bit  |
| &#128270; | handover\_st2\_started| bit  |
| &#128270; | engineering\_planning\_started| bit  |
| &#128270; | production\_started| bit  |
| &#128270; | shipping\_in\_transit\_started| bit  |
| &#128270; | balance\_payable\_started| bit  |
| &#128270; | project\_infor\_reference| varchar(8000)  |
| &#128270; | infor\_order\_reference| varchar(8000)  |
| &#128270; | additional\_infor\_orders| varchar(8000)  |
| &#128270; | days\_in\_awaiting\_factory\_info| decimal(38,18)  |
| &#128270; | order\_description| varchar(8000)  |
| &#128270; | handover\_link| varchar(8000)  |
| &#128270; | shops\_approved\_date| datetime2(26)  |
| &#128270; | shops\_revision\_issued| varchar(8000)  |
| &#128270; | samples\_sent\_to\_customer| datetime2(26)  |
| &#128270; | additional\_sample\_mock\_ups| varchar(8000)  |
| &#128270; | samples\_approved| datetime2(26)  |
| &#128270; | shop\_revision\_approved| varchar(8000)  |
| &#128270; | pending\_reason| varchar(8000)  |
| &#128270; | po\_number| varchar(8000)  |
| &#128270; | co1\_value| decimal(38,18)  |
| &#128270; | acknowledged| varchar(8000)  |
| &#128270; | processed\_by| varchar(8000)  |
| &#128270; | order\_value| decimal(38,18)  |
| &#128270; | order\_sqm| decimal(38,18)  |
| &#128270; | days\_in\_cleansing| decimal(38,18)  |
| &#128270; | pending\_amount| decimal(38,18)  |
| &#128270; | days\_in\_design| decimal(38,18)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | acknowledged\_text| varchar(8000)  |
| &#128270; | days\_in\_customer\_sign\_off| decimal(38,18)  |
| &#128270; | days\_in\_engineering| decimal(38,18)  |
| &#128270; | days\_in\_scheduling| decimal(38,18)  |
| &#128270; | weekday| decimal(38,18)  |
| &#128270; | infor\_order\_reference\_f| varchar(8000)  |
| &#128270; | order\_type| varchar(8000)  |
| &#128270; | final\_dispatch\_date| datetime2(26)  |
| &#128270; | commercial\_rec\_complete| datetime2(26)  |
| &#128270; | final\_delivery\_date| datetime2(26)  |
| &#128270; | company\_infor\_reference| varchar(8000)  |
| &#128270; | ship\_date| datetime2(26)  |
| &#128270; | value| decimal(38,18)  |
| &#128270; | project\_complexity| varchar(8000)  |
| &#128270; | notes| varchar(8000)  |
| &#128270; | first\_delivery\_on\_site| datetime2(26)  |
| &#128270; | date\_in\_customer\_sign\_off| datetime2(26)  |
| &#128270; | date\_out\_customer\_sign\_off| datetime2(26)  |
| &#128270; | date\_in\_engineering| datetime2(26)  |
| &#128270; | date\_out\_engineering| datetime2(26)  |
| &#128270; | date\_in\_scheduling| datetime2(26)  |
| &#128270; | date\_out\_scheduling| datetime2(26)  |
| &#128270; | material\_group| varchar(8000)  |
| &#128270; | project\_description| varchar(8000)  |
| &#128270; | emailed\_projected\_date| datetime2(26)  |
| &#128270; | us\_shipping\_method| varchar(8000)  |
| &#128270; | rbmw\_order| varchar(8000)  |
| &#128270; | pu\_order| varchar(8000)  |
| &#128270; | additional\_information\_on\_the\_order| varchar(8000)  |
| &#128270; | request\_date| datetime2(26)  |
| &#128270; | order\_lines\_dated\_on\_factory\_book\_text| varchar(8000)  |
| &#128270; | cb\_order\_reference| varchar(8000)  |
| &#128270; | pb\_order\_reference| varchar(8000)  |
| &#128270; | c\_order\_reference| varchar(8000)  |
| &#128270; | order\_manager| varchar(8000)  |
| &#128270; | sign\_off\_status| bit  |
| &#128270; | complexity| varchar(8000)  |
| &#128270; | created\_date\_custom| datetime2(26)  |
| &#128270; | closed\_date| datetime2(26)  |
| &#128270; | days\_taken\_to\_close| decimal(38,18)  |
| &#128270; | overdue| bit  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON owner\_id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON record\_type\_id|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON company\_name|
| &#128270;  | ClusteredIndex | ON contact\_name|
| &#128270;  | ClusteredIndex | ON pending\_reason\_formula|
| &#128270;  | ClusteredIndex | ON sample\_mock\_up|
| &#128270;  | ClusteredIndex | ON factory\_manager|
| &#128270;  | ClusteredIndex | ON order\_number|
| &#128270;  | ClusteredIndex | ON po\_received|
| &#128270;  | ClusteredIndex | ON po\_value|
| &#128270;  | ClusteredIndex | ON days\_in\_to\_be\_acknowledged|
| &#128270;  | ClusteredIndex | ON deposit\_proforma\_issued|
| &#128270;  | ClusteredIndex | ON proforma\_value|
| &#128270;  | ClusteredIndex | ON payment\_received|
| &#128270;  | ClusteredIndex | ON sign\_off\_notes|
| &#128270;  | ClusteredIndex | ON chase\_date|
| &#128270;  | ClusteredIndex | ON days\_in\_estimating|
| &#128270;  | ClusteredIndex | ON submittal\_issued|
| &#128270;  | ClusteredIndex | ON submittals\_approved|
| &#128270;  | ClusteredIndex | ON handover\_to\_so|
| &#128270;  | ClusteredIndex | ON department\_to\_chase|
| &#128270;  | ClusteredIndex | ON stage|
| &#128270;  | ClusteredIndex | ON product\_into\_engineering\_planning|
| &#128270;  | ClusteredIndex | ON no\_of\_chases|
| &#128270;  | ClusteredIndex | ON order\_lines\_dated\_on\_factory\_book|
| &#128270;  | ClusteredIndex | ON last\_chase\_date|
| &#128270;  | ClusteredIndex | ON order\_acknowledgement\_sent\_to\_customer|
| &#128270;  | ClusteredIndex | ON date\_shipped\_out\_of\_factory|
| &#128270;  | ClusteredIndex | ON value\_due|
| &#128270;  | ClusteredIndex | ON due\_by|
| &#128270;  | ClusteredIndex | ON infor\_references|
| &#128270;  | ClusteredIndex | ON shipping\_method|
| &#128270;  | ClusteredIndex | ON pkgs|
| &#128270;  | ClusteredIndex | ON ets|
| &#128270;  | ClusteredIndex | ON eta|
| &#128270;  | ClusteredIndex | ON shipment\_notice\_issued\_to\_customer|
| &#128270;  | ClusteredIndex | ON owner\_and\_reason|
| &#128270;  | ClusteredIndex | ON project\_owner|
| &#128270;  | ClusteredIndex | ON project\_secondary\_owner|
| &#128270;  | ClusteredIndex | ON project\_stage|
| &#128270;  | ClusteredIndex | ON project\_probability|
| &#128270;  | ClusteredIndex | ON project\_specification|
| &#128270;  | ClusteredIndex | ON in\_contract\_start\_date|
| &#128270;  | ClusteredIndex | ON in\_contract\_end\_date|
| &#128270;  | ClusteredIndex | ON shops\_submittals\_start\_date|
| &#128270;  | ClusteredIndex | ON shops\_submittals\_end\_date|
| &#128270;  | ClusteredIndex | ON handover\_st2\_start\_date|
| &#128270;  | ClusteredIndex | ON handover\_st2\_end\_date|
| &#128270;  | ClusteredIndex | ON engineering\_planning\_start\_date|
| &#128270;  | ClusteredIndex | ON engineering\_planning\_end\_date|
| &#128270;  | ClusteredIndex | ON production\_start\_date|
| &#128270;  | ClusteredIndex | ON production\_end\_date|
| &#128270;  | ClusteredIndex | ON shipping\_in\_transit\_start\_date|
| &#128270;  | ClusteredIndex | ON shipping\_in\_transit\_end\_date|
| &#128270;  | ClusteredIndex | ON balance\_payable\_start\_date|
| &#128270;  | ClusteredIndex | ON balance\_payable\_end\_date|
| &#128270;  | ClusteredIndex | ON in\_contract\_started|
| &#128270;  | ClusteredIndex | ON shops\_submittals\_started|
| &#128270;  | ClusteredIndex | ON handover\_st2\_started|
| &#128270;  | ClusteredIndex | ON engineering\_planning\_started|
| &#128270;  | ClusteredIndex | ON production\_started|
| &#128270;  | ClusteredIndex | ON shipping\_in\_transit\_started|
| &#128270;  | ClusteredIndex | ON balance\_payable\_started|
| &#128270;  | ClusteredIndex | ON project\_infor\_reference|
| &#128270;  | ClusteredIndex | ON infor\_order\_reference|
| &#128270;  | ClusteredIndex | ON additional\_infor\_orders|
| &#128270;  | ClusteredIndex | ON days\_in\_awaiting\_factory\_info|
| &#128270;  | ClusteredIndex | ON order\_description|
| &#128270;  | ClusteredIndex | ON handover\_link|
| &#128270;  | ClusteredIndex | ON shops\_approved\_date|
| &#128270;  | ClusteredIndex | ON shops\_revision\_issued|
| &#128270;  | ClusteredIndex | ON samples\_sent\_to\_customer|
| &#128270;  | ClusteredIndex | ON additional\_sample\_mock\_ups|
| &#128270;  | ClusteredIndex | ON samples\_approved|
| &#128270;  | ClusteredIndex | ON shop\_revision\_approved|
| &#128270;  | ClusteredIndex | ON pending\_reason|
| &#128270;  | ClusteredIndex | ON po\_number|
| &#128270;  | ClusteredIndex | ON co1\_value|
| &#128270;  | ClusteredIndex | ON acknowledged|
| &#128270;  | ClusteredIndex | ON processed\_by|
| &#128270;  | ClusteredIndex | ON order\_value|
| &#128270;  | ClusteredIndex | ON order\_sqm|
| &#128270;  | ClusteredIndex | ON days\_in\_cleansing|
| &#128270;  | ClusteredIndex | ON pending\_amount|
| &#128270;  | ClusteredIndex | ON days\_in\_design|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON acknowledged\_text|
| &#128270;  | ClusteredIndex | ON days\_in\_customer\_sign\_off|
| &#128270;  | ClusteredIndex | ON days\_in\_engineering|
| &#128270;  | ClusteredIndex | ON days\_in\_scheduling|
| &#128270;  | ClusteredIndex | ON weekday|
| &#128270;  | ClusteredIndex | ON infor\_order\_reference\_f|
| &#128270;  | ClusteredIndex | ON order\_type|
| &#128270;  | ClusteredIndex | ON final\_dispatch\_date|
| &#128270;  | ClusteredIndex | ON commercial\_rec\_complete|
| &#128270;  | ClusteredIndex | ON final\_delivery\_date|
| &#128270;  | ClusteredIndex | ON company\_infor\_reference|
| &#128270;  | ClusteredIndex | ON ship\_date|
| &#128270;  | ClusteredIndex | ON value|
| &#128270;  | ClusteredIndex | ON project\_complexity|
| &#128270;  | ClusteredIndex | ON notes|
| &#128270;  | ClusteredIndex | ON first\_delivery\_on\_site|
| &#128270;  | ClusteredIndex | ON date\_in\_customer\_sign\_off|
| &#128270;  | ClusteredIndex | ON date\_out\_customer\_sign\_off|
| &#128270;  | ClusteredIndex | ON date\_in\_engineering|
| &#128270;  | ClusteredIndex | ON date\_out\_engineering|
| &#128270;  | ClusteredIndex | ON date\_in\_scheduling|
| &#128270;  | ClusteredIndex | ON date\_out\_scheduling|
| &#128270;  | ClusteredIndex | ON material\_group|
| &#128270;  | ClusteredIndex | ON project\_description|
| &#128270;  | ClusteredIndex | ON emailed\_projected\_date|
| &#128270;  | ClusteredIndex | ON us\_shipping\_method|
| &#128270;  | ClusteredIndex | ON rbmw\_order|
| &#128270;  | ClusteredIndex | ON pu\_order|
| &#128270;  | ClusteredIndex | ON additional\_information\_on\_the\_order|
| &#128270;  | ClusteredIndex | ON request\_date|
| &#128270;  | ClusteredIndex | ON order\_lines\_dated\_on\_factory\_book\_text|
| &#128270;  | ClusteredIndex | ON cb\_order\_reference|
| &#128270;  | ClusteredIndex | ON pb\_order\_reference|
| &#128270;  | ClusteredIndex | ON c\_order\_reference|
| &#128270;  | ClusteredIndex | ON order\_manager|
| &#128270;  | ClusteredIndex | ON sign\_off\_status|
| &#128270;  | ClusteredIndex | ON complexity|
| &#128270;  | ClusteredIndex | ON created\_date\_custom|
| &#128270;  | ClusteredIndex | ON closed\_date|
| &#128270;  | ClusteredIndex | ON days\_taken\_to\_close|
| &#128270;  | ClusteredIndex | ON overdue|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.po_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | po\_num| varchar(8000)  |
| &#128270; | vend\_num| varchar(8000)  |
| &#128270; | order\_date| datetime2(26)  |
| &#128270; | po\_cost| decimal(23,8)  |
| &#128270; | ship\_code| varchar(8000)  |
| &#128270; | terms\_code| varchar(8000)  |
| &#128270; | fob| varchar(8000)  |
| &#128270; | print\_price| int  |
| &#128270; | vend\_order| varchar(8000)  |
| &#128270; | misc\_charges| decimal(23,8)  |
| &#128270; | sales\_tax| decimal(23,8)  |
| &#128270; | freight| decimal(23,8)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | inv\_date| datetime2(26)  |
| &#128270; | inv\_num| varchar(8000)  |
| &#128270; | dist\_date| datetime2(26)  |
| &#128270; | type| varchar(8000)  |
| &#128270; | drop\_ship\_no| varchar(8000)  |
| &#128270; | drop\_seq| int  |
| &#128270; | eff\_date| datetime2(26)  |
| &#128270; | exp\_date| datetime2(26)  |
| &#128270; | ship\_addr| varchar(8000)  |
| &#128270; | m\_charges\_t| decimal(23,8)  |
| &#128270; | sales\_tax\_t| decimal(23,8)  |
| &#128270; | freight\_t| decimal(23,8)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | sales\_tax\_2| decimal(23,8)  |
| &#128270; | sales\_tax\_t2| decimal(23,8)  |
| &#128270; | charfld1| varchar(8000)  |
| &#128270; | charfld2| varchar(8000)  |
| &#128270; | charfld3| varchar(8000)  |
| &#128270; | datefld| datetime2(26)  |
| &#128270; | decifld1| decimal(10,2)  |
| &#128270; | decifld2| decimal(10,2)  |
| &#128270; | decifld3| decimal(10,2)  |
| &#128270; | logifld| int  |
| &#128270; | duty\_amt\_t| decimal(23,8)  |
| &#128270; | duty\_amt| decimal(23,8)  |
| &#128270; | brokerage\_amt| decimal(23,8)  |
| &#128270; | brokerage\_amt\_t| decimal(23,8)  |
| &#128270; | trans\_nat| varchar(8000)  |
| &#128270; | process\_ind| varchar(8000)  |
| &#128270; | delterm| varchar(8000)  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | frt\_tax\_code1| varchar(8000)  |
| &#128270; | frt\_tax\_code2| varchar(8000)  |
| &#128270; | msc\_tax\_code1| varchar(8000)  |
| &#128270; | msc\_tax\_code2| varchar(8000)  |
| &#128270; | prepaid\_amt| decimal(23,8)  |
| &#128270; | prepaid\_t| decimal(23,8)  |
| &#128270; | exch\_rate| decimal(12,7)  |
| &#128270; | fixed\_rate| int  |
| &#128270; | freight\_vend\_num| varchar(8000)  |
| &#128270; | duty\_vend\_num| varchar(8000)  |
| &#128270; | brokerage\_vend\_num| varchar(8000)  |
| &#128270; | frt\_alloc\_percent| decimal(8,5)  |
| &#128270; | duty\_alloc\_percent| decimal(8,5)  |
| &#128270; | brk\_alloc\_percent| decimal(8,5)  |
| &#128270; | est\_freight| decimal(23,8)  |
| &#128270; | act\_freight| decimal(23,8)  |
| &#128270; | est\_brokerage| decimal(23,8)  |
| &#128270; | act\_brokerage| decimal(23,8)  |
| &#128270; | est\_duty| decimal(23,8)  |
| &#128270; | act\_duty| decimal(23,8)  |
| &#128270; | duty\_alloc\_meth| varchar(8000)  |
| &#128270; | frt\_alloc\_meth| varchar(8000)  |
| &#128270; | brk\_alloc\_meth| varchar(8000)  |
| &#128270; | duty\_alloc\_type| varchar(8000)  |
| &#128270; | frt\_alloc\_type| varchar(8000)  |
| &#128270; | brk\_alloc\_type| varchar(8000)  |
| &#128270; | vend\_lcr\_num| varchar(8000)  |
| &#128270; | received| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | buyer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | ins\_vend\_num| varchar(8000)  |
| &#128270; | ins\_alloc\_percent| decimal(8,5)  |
| &#128270; | ins\_alloc\_type| varchar(8000)  |
| &#128270; | est\_insurance| decimal(23,8)  |
| &#128270; | ins\_alloc\_meth| varchar(8000)  |
| &#128270; | act\_insurance| decimal(23,8)  |
| &#128270; | insurance\_amt| decimal(23,8)  |
| &#128270; | insurance\_amt\_t| decimal(23,8)  |
| &#128270; | loc\_frt\_vend\_num| varchar(8000)  |
| &#128270; | loc\_frt\_alloc\_percent| decimal(8,5)  |
| &#128270; | loc\_frt\_alloc\_type| varchar(8000)  |
| &#128270; | est\_local\_freight| decimal(23,8)  |
| &#128270; | loc\_frt\_alloc\_meth| varchar(8000)  |
| &#128270; | act\_local\_freight| decimal(23,8)  |
| &#128270; | local\_freight\_amt| decimal(23,8)  |
| &#128270; | local\_freight\_amt\_t| decimal(23,8)  |
| &#128270; | include\_tax\_in\_cost| int  |
| &#128270; | trans\_nat\_2| varchar(8000)  |
| &#128270; | contains\_only\_tax\_free\_matls| int  |
| &#128270; | supply\_web\_po\_stat| varchar(8000)  |
| &#128270; | builder\_po\_orig\_site| varchar(8000)  |
| &#128270; | builder\_po\_num| varchar(8000)  |
| &#128270; | builder\_po\_printed| int  |
| &#128270; | synchronized\_to\_bus| int  |
| &#128270; | auto\_voucher| int  |
| &#128270; | auto\_receive\_demanding\_site\_po| int  |
| &#128270; | auto\_ship\_demanding\_site\_co| int  |
| &#128270; | source\_site\_co\_num| varchar(8000)  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | fr\_fixed\_asset| int  |
| &#128270; | uf\_confirmation| int  |
| &#128270; | uf\_eng\_project| varchar(8000)  |
| &#128270; | uf\_micross\_no| varchar(8000)  |
| &#128270; | uf\_project| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON po\_num|
| &#128270;  | ClusteredIndex | ON vend\_num|
| &#128270;  | ClusteredIndex | ON order\_date|
| &#128270;  | ClusteredIndex | ON po\_cost|
| &#128270;  | ClusteredIndex | ON ship\_code|
| &#128270;  | ClusteredIndex | ON terms\_code|
| &#128270;  | ClusteredIndex | ON fob|
| &#128270;  | ClusteredIndex | ON print\_price|
| &#128270;  | ClusteredIndex | ON vend\_order|
| &#128270;  | ClusteredIndex | ON misc\_charges|
| &#128270;  | ClusteredIndex | ON sales\_tax|
| &#128270;  | ClusteredIndex | ON freight|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON inv\_date|
| &#128270;  | ClusteredIndex | ON inv\_num|
| &#128270;  | ClusteredIndex | ON dist\_date|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON drop\_ship\_no|
| &#128270;  | ClusteredIndex | ON drop\_seq|
| &#128270;  | ClusteredIndex | ON eff\_date|
| &#128270;  | ClusteredIndex | ON exp\_date|
| &#128270;  | ClusteredIndex | ON ship\_addr|
| &#128270;  | ClusteredIndex | ON m\_charges\_t|
| &#128270;  | ClusteredIndex | ON sales\_tax\_t|
| &#128270;  | ClusteredIndex | ON freight\_t|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON sales\_tax\_2|
| &#128270;  | ClusteredIndex | ON sales\_tax\_t2|
| &#128270;  | ClusteredIndex | ON charfld1|
| &#128270;  | ClusteredIndex | ON charfld2|
| &#128270;  | ClusteredIndex | ON charfld3|
| &#128270;  | ClusteredIndex | ON datefld|
| &#128270;  | ClusteredIndex | ON decifld1|
| &#128270;  | ClusteredIndex | ON decifld2|
| &#128270;  | ClusteredIndex | ON decifld3|
| &#128270;  | ClusteredIndex | ON logifld|
| &#128270;  | ClusteredIndex | ON duty\_amt\_t|
| &#128270;  | ClusteredIndex | ON duty\_amt|
| &#128270;  | ClusteredIndex | ON brokerage\_amt|
| &#128270;  | ClusteredIndex | ON brokerage\_amt\_t|
| &#128270;  | ClusteredIndex | ON trans\_nat|
| &#128270;  | ClusteredIndex | ON process\_ind|
| &#128270;  | ClusteredIndex | ON delterm|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON frt\_tax\_code1|
| &#128270;  | ClusteredIndex | ON frt\_tax\_code2|
| &#128270;  | ClusteredIndex | ON msc\_tax\_code1|
| &#128270;  | ClusteredIndex | ON msc\_tax\_code2|
| &#128270;  | ClusteredIndex | ON prepaid\_amt|
| &#128270;  | ClusteredIndex | ON prepaid\_t|
| &#128270;  | ClusteredIndex | ON exch\_rate|
| &#128270;  | ClusteredIndex | ON fixed\_rate|
| &#128270;  | ClusteredIndex | ON freight\_vend\_num|
| &#128270;  | ClusteredIndex | ON duty\_vend\_num|
| &#128270;  | ClusteredIndex | ON brokerage\_vend\_num|
| &#128270;  | ClusteredIndex | ON frt\_alloc\_percent|
| &#128270;  | ClusteredIndex | ON duty\_alloc\_percent|
| &#128270;  | ClusteredIndex | ON brk\_alloc\_percent|
| &#128270;  | ClusteredIndex | ON est\_freight|
| &#128270;  | ClusteredIndex | ON act\_freight|
| &#128270;  | ClusteredIndex | ON est\_brokerage|
| &#128270;  | ClusteredIndex | ON act\_brokerage|
| &#128270;  | ClusteredIndex | ON est\_duty|
| &#128270;  | ClusteredIndex | ON act\_duty|
| &#128270;  | ClusteredIndex | ON duty\_alloc\_meth|
| &#128270;  | ClusteredIndex | ON frt\_alloc\_meth|
| &#128270;  | ClusteredIndex | ON brk\_alloc\_meth|
| &#128270;  | ClusteredIndex | ON duty\_alloc\_type|
| &#128270;  | ClusteredIndex | ON frt\_alloc\_type|
| &#128270;  | ClusteredIndex | ON brk\_alloc\_type|
| &#128270;  | ClusteredIndex | ON vend\_lcr\_num|
| &#128270;  | ClusteredIndex | ON received|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON buyer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON ins\_vend\_num|
| &#128270;  | ClusteredIndex | ON ins\_alloc\_percent|
| &#128270;  | ClusteredIndex | ON ins\_alloc\_type|
| &#128270;  | ClusteredIndex | ON est\_insurance|
| &#128270;  | ClusteredIndex | ON ins\_alloc\_meth|
| &#128270;  | ClusteredIndex | ON act\_insurance|
| &#128270;  | ClusteredIndex | ON insurance\_amt|
| &#128270;  | ClusteredIndex | ON insurance\_amt\_t|
| &#128270;  | ClusteredIndex | ON loc\_frt\_vend\_num|
| &#128270;  | ClusteredIndex | ON loc\_frt\_alloc\_percent|
| &#128270;  | ClusteredIndex | ON loc\_frt\_alloc\_type|
| &#128270;  | ClusteredIndex | ON est\_local\_freight|
| &#128270;  | ClusteredIndex | ON loc\_frt\_alloc\_meth|
| &#128270;  | ClusteredIndex | ON act\_local\_freight|
| &#128270;  | ClusteredIndex | ON local\_freight\_amt|
| &#128270;  | ClusteredIndex | ON local\_freight\_amt\_t|
| &#128270;  | ClusteredIndex | ON include\_tax\_in\_cost|
| &#128270;  | ClusteredIndex | ON trans\_nat\_2|
| &#128270;  | ClusteredIndex | ON contains\_only\_tax\_free\_matls|
| &#128270;  | ClusteredIndex | ON supply\_web\_po\_stat|
| &#128270;  | ClusteredIndex | ON builder\_po\_orig\_site|
| &#128270;  | ClusteredIndex | ON builder\_po\_num|
| &#128270;  | ClusteredIndex | ON builder\_po\_printed|
| &#128270;  | ClusteredIndex | ON synchronized\_to\_bus|
| &#128270;  | ClusteredIndex | ON auto\_voucher|
| &#128270;  | ClusteredIndex | ON auto\_receive\_demanding\_site\_po|
| &#128270;  | ClusteredIndex | ON auto\_ship\_demanding\_site\_co|
| &#128270;  | ClusteredIndex | ON source\_site\_co\_num|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON fr\_fixed\_asset|
| &#128270;  | ClusteredIndex | ON uf\_confirmation|
| &#128270;  | ClusteredIndex | ON uf\_eng\_project|
| &#128270;  | ClusteredIndex | ON uf\_micross\_no|
| &#128270;  | ClusteredIndex | ON uf\_project|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.poitem_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | po\_num| varchar(8000)  |
| &#128270; | po\_line| int  |
| &#128270; | po\_release| int  |
| &#128270; | item| varchar(8000)  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | qty\_ordered| decimal(19,8)  |
| &#128270; | qty\_received| decimal(19,8)  |
| &#128270; | qty\_rejected| decimal(19,8)  |
| &#128270; | qty\_voucher| decimal(19,8)  |
| &#128270; | qty\_returned| decimal(19,8)  |
| &#128270; | item\_cost| decimal(20,8)  |
| &#128270; | ref\_type| varchar(8000)  |
| &#128270; | ref\_num| varchar(8000)  |
| &#128270; | ref\_line\_suf| int  |
| &#128270; | ref\_release| int  |
| &#128270; | due\_date| datetime2(26)  |
| &#128270; | rcvd\_date| datetime2(26)  |
| &#128270; | vend\_item| varchar(8000)  |
| &#128270; | root\_job| varchar(8000)  |
| &#128270; | root\_suf| int  |
| &#128270; | plan\_cost| decimal(20,8)  |
| &#128270; | voucher\_cost| decimal(23,8)  |
| &#128270; | non\_inv\_acct| varchar(8000)  |
| &#128270; | drop\_ship\_no| varchar(8000)  |
| &#128270; | drop\_seq| int  |
| &#128270; | ship\_addr| varchar(8000)  |
| &#128270; | promise\_date| datetime2(26)  |
| &#128270; | release\_date| datetime2(26)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | item\_type| varchar(8000)  |
| &#128270; | cost\_type| varchar(8000)  |
| &#128270; | comm\_code| varchar(8000)  |
| &#128270; | trans\_nat| varchar(8000)  |
| &#128270; | process\_ind| varchar(8000)  |
| &#128270; | unit\_weight| decimal(11,3)  |
| &#128270; | delterm| varchar(8000)  |
| &#128270; | origin| varchar(8000)  |
| &#128270; | cons\_num| int  |
| &#128270; | unit\_mat\_cost| decimal(20,8)  |
| &#128270; | unit\_duty\_cost| decimal(20,8)  |
| &#128270; | unit\_freight\_cost| decimal(20,8)  |
| &#128270; | unit\_brokerage\_cost| decimal(20,8)  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | export\_value| decimal(23,8)  |
| &#128270; | ec\_code| varchar(8000)  |
| &#128270; | transport| varchar(8000)  |
| &#128270; | req\_num| varchar(8000)  |
| &#128270; | req\_line| int  |
| &#128270; | u\_m| varchar(8000)  |
| &#128270; | qty\_ordered\_conv| decimal(19,8)  |
| &#128270; | item\_cost\_conv| decimal(20,8)  |
| &#128270; | plan\_cost\_conv| decimal(20,8)  |
| &#128270; | unit\_mat\_cost\_conv| decimal(20,8)  |
| &#128270; | unit\_duty\_cost\_conv| decimal(20,8)  |
| &#128270; | unit\_freight\_cost\_conv| decimal(20,8)  |
| &#128270; | unit\_brokerage\_cost\_conv| decimal(20,8)  |
| &#128270; | non\_inv\_acct\_unit1| varchar(8000)  |
| &#128270; | non\_inv\_acct\_unit2| varchar(8000)  |
| &#128270; | non\_inv\_acct\_unit3| varchar(8000)  |
| &#128270; | non\_inv\_acct\_unit4| varchar(8000)  |
| &#128270; | lc\_override| int  |
| &#128270; | revision| varchar(8000)  |
| &#128270; | drawing\_nbr| varchar(8000)  |
| &#128270; | po\_vend\_num| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | expedited| int  |
| &#128270; | rcpt\_rqmt| varchar(8000)  |
| &#128270; | unit\_insurance\_cost| decimal(20,8)  |
| &#128270; | unit\_insurance\_cost\_conv| decimal(20,8)  |
| &#128270; | unit\_loc\_frt\_cost| decimal(20,8)  |
| &#128270; | unit\_loc\_frt\_cost\_conv| decimal(20,8)  |
| &#128270; | trans\_nat\_2| varchar(8000)  |
| &#128270; | suppl\_qty\_conv\_factor| float(53)  |
| &#128270; | unlinked\_xref| int  |
| &#128270; | due\_date\_day| datetime2(26)  |
| &#128270; | preassign\_lots| int  |
| &#128270; | preassign\_serials| int  |
| &#128270; | ipr\_id| varchar(8000)  |
| &#128270; | ipr\_seq| decimal(11,0)  |
| &#128270; | manufacturer\_id| varchar(8000)  |
| &#128270; | manufacturer\_item| varchar(8000)  |
| &#128270; | fa\_num| varchar(8000)  |
| &#128270; | fa\_class| varchar(8000)  |
| &#128270; | dept| varchar(8000)  |
| &#128270; | uf\_ack\_date| datetime2(26)  |
| &#128270; | uf\_ack\_no| varchar(8000)  |
| &#128270; | uf\_eng\_project| varchar(8000)  |
| &#128270; | uf\_long\_description| varchar(8000)  |
| &#128270; | uf\_noof\_packs| int  |
| &#128270; | uf\_quantity| decimal(23,8)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON po\_num|
| &#128270;  | ClusteredIndex | ON po\_line|
| &#128270;  | ClusteredIndex | ON po\_release|
| &#128270;  | ClusteredIndex | ON item|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON qty\_ordered|
| &#128270;  | ClusteredIndex | ON qty\_received|
| &#128270;  | ClusteredIndex | ON qty\_rejected|
| &#128270;  | ClusteredIndex | ON qty\_voucher|
| &#128270;  | ClusteredIndex | ON qty\_returned|
| &#128270;  | ClusteredIndex | ON item\_cost|
| &#128270;  | ClusteredIndex | ON ref\_type|
| &#128270;  | ClusteredIndex | ON ref\_num|
| &#128270;  | ClusteredIndex | ON ref\_line\_suf|
| &#128270;  | ClusteredIndex | ON ref\_release|
| &#128270;  | ClusteredIndex | ON due\_date|
| &#128270;  | ClusteredIndex | ON rcvd\_date|
| &#128270;  | ClusteredIndex | ON vend\_item|
| &#128270;  | ClusteredIndex | ON root\_job|
| &#128270;  | ClusteredIndex | ON root\_suf|
| &#128270;  | ClusteredIndex | ON plan\_cost|
| &#128270;  | ClusteredIndex | ON voucher\_cost|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct|
| &#128270;  | ClusteredIndex | ON drop\_ship\_no|
| &#128270;  | ClusteredIndex | ON drop\_seq|
| &#128270;  | ClusteredIndex | ON ship\_addr|
| &#128270;  | ClusteredIndex | ON promise\_date|
| &#128270;  | ClusteredIndex | ON release\_date|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON item\_type|
| &#128270;  | ClusteredIndex | ON cost\_type|
| &#128270;  | ClusteredIndex | ON comm\_code|
| &#128270;  | ClusteredIndex | ON trans\_nat|
| &#128270;  | ClusteredIndex | ON process\_ind|
| &#128270;  | ClusteredIndex | ON unit\_weight|
| &#128270;  | ClusteredIndex | ON delterm|
| &#128270;  | ClusteredIndex | ON origin|
| &#128270;  | ClusteredIndex | ON cons\_num|
| &#128270;  | ClusteredIndex | ON unit\_mat\_cost|
| &#128270;  | ClusteredIndex | ON unit\_duty\_cost|
| &#128270;  | ClusteredIndex | ON unit\_freight\_cost|
| &#128270;  | ClusteredIndex | ON unit\_brokerage\_cost|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON export\_value|
| &#128270;  | ClusteredIndex | ON ec\_code|
| &#128270;  | ClusteredIndex | ON transport|
| &#128270;  | ClusteredIndex | ON req\_num|
| &#128270;  | ClusteredIndex | ON req\_line|
| &#128270;  | ClusteredIndex | ON u\_m|
| &#128270;  | ClusteredIndex | ON qty\_ordered\_conv|
| &#128270;  | ClusteredIndex | ON item\_cost\_conv|
| &#128270;  | ClusteredIndex | ON plan\_cost\_conv|
| &#128270;  | ClusteredIndex | ON unit\_mat\_cost\_conv|
| &#128270;  | ClusteredIndex | ON unit\_duty\_cost\_conv|
| &#128270;  | ClusteredIndex | ON unit\_freight\_cost\_conv|
| &#128270;  | ClusteredIndex | ON unit\_brokerage\_cost\_conv|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON non\_inv\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON lc\_override|
| &#128270;  | ClusteredIndex | ON revision|
| &#128270;  | ClusteredIndex | ON drawing\_nbr|
| &#128270;  | ClusteredIndex | ON po\_vend\_num|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON expedited|
| &#128270;  | ClusteredIndex | ON rcpt\_rqmt|
| &#128270;  | ClusteredIndex | ON unit\_insurance\_cost|
| &#128270;  | ClusteredIndex | ON unit\_insurance\_cost\_conv|
| &#128270;  | ClusteredIndex | ON unit\_loc\_frt\_cost|
| &#128270;  | ClusteredIndex | ON unit\_loc\_frt\_cost\_conv|
| &#128270;  | ClusteredIndex | ON trans\_nat\_2|
| &#128270;  | ClusteredIndex | ON suppl\_qty\_conv\_factor|
| &#128270;  | ClusteredIndex | ON unlinked\_xref|
| &#128270;  | ClusteredIndex | ON due\_date\_day|
| &#128270;  | ClusteredIndex | ON preassign\_lots|
| &#128270;  | ClusteredIndex | ON preassign\_serials|
| &#128270;  | ClusteredIndex | ON ipr\_id|
| &#128270;  | ClusteredIndex | ON ipr\_seq|
| &#128270;  | ClusteredIndex | ON manufacturer\_id|
| &#128270;  | ClusteredIndex | ON manufacturer\_item|
| &#128270;  | ClusteredIndex | ON fa\_num|
| &#128270;  | ClusteredIndex | ON fa\_class|
| &#128270;  | ClusteredIndex | ON dept|
| &#128270;  | ClusteredIndex | ON uf\_ack\_date|
| &#128270;  | ClusteredIndex | ON uf\_ack\_no|
| &#128270;  | ClusteredIndex | ON uf\_eng\_project|
| &#128270;  | ClusteredIndex | ON uf\_long\_description|
| &#128270;  | ClusteredIndex | ON uf\_noof\_packs|
| &#128270;  | ClusteredIndex | ON uf\_quantity|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table sharepoint.proactive_reactive_maintenance 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | proactive| float(53)  |
| &#128270; | target| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON proactive|
| &#128270;  | ClusteredIndex | ON target|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint_staging.proactive_reactive_maintenance 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | proactive| float(53)  |
| &#128270; | target| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON proactive|
| &#128270;  | ClusteredIndex | ON target|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline.product_engineering_productivity_capacity 
|Idx |Name |Data Type |
|---|---|---|
| * &#128270; | warehouse\_prefix| varchar(10)  |
| * &#128270; | daily\_capacity| decimal(18,6)  |
| * &#128270; | target\_value| decimal(18,6)  |
| * &#128270; | is\_approved| bit  |
| * &#128270; | capacity\_basis| varchar(500)  |
| * &#128270; | updated\_ts| datetime2(26)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON warehouse\_prefix|
| &#128270;  | ClusteredIndex | ON daily\_capacity|
| &#128270;  | ClusteredIndex | ON target\_value|
| &#128270;  | ClusteredIndex | ON is\_approved|
| &#128270;  | ClusteredIndex | ON capacity\_basis|
| &#128270;  | ClusteredIndex | ON updated\_ts|



### Table salesforce_staging.project_contact 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | project| varchar(8000)  |
| &#128270; | project\_contact| varchar(8000)  |
| &#128270; | contact\_project\_role| varchar(8000)  |
| &#128270; | involvement| varchar(8000)  |
| &#128270; | project\_key\_contact| varchar(8000)  |
| &#128270; | project\_phone\_number| varchar(8000)  |
| &#128270; | contact| varchar(8000)  |
| &#128270; | company| varchar(8000)  |
| &#128270; | project\_account\_role| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON project|
| &#128270;  | ClusteredIndex | ON project\_contact|
| &#128270;  | ClusteredIndex | ON contact\_project\_role|
| &#128270;  | ClusteredIndex | ON involvement|
| &#128270;  | ClusteredIndex | ON project\_key\_contact|
| &#128270;  | ClusteredIndex | ON project\_phone\_number|
| &#128270;  | ClusteredIndex | ON contact|
| &#128270;  | ClusteredIndex | ON company|
| &#128270;  | ClusteredIndex | ON project\_account\_role|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.proposal_request 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | record\_type\_id| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | status| varchar(8000)  |
| &#128270; | company\_name| varchar(8000)  |
| &#128270; | project\_name| varchar(8000)  |
| &#128270; | contact\_name| varchar(8000)  |
| &#128270; | infor\_reference\_number\_project| varchar(8000)  |
| &#128270; | infor\_reference\_number\_account| varchar(8000)  |
| &#128270; | complexity| varchar(8000)  |
| &#128270; | complete\_by\_date| datetime2(26)  |
| &#128270; | project\_owner| varchar(8000)  |
| &#128270; | project\_secondary\_owner| varchar(8000)  |
| &#128270; | project\_stage| varchar(8000)  |
| &#128270; | project\_probability| varchar(8000)  |
| &#128270; | project\_specification| varchar(8000)  |
| &#128270; | days\_overdue| decimal(38,18)  |
| &#128270; | sharepoint| varchar(8000)  |
| &#128270; | opportunity\_review\_reason| varchar(8000)  |
| &#128270; | review\_date| datetime2(26)  |
| &#128270; | scope\_m2| decimal(38,18)  |
| &#128270; | commercial\_sign\_off\_by| varchar(8000)  |
| &#128270; | design\_sign\_off\_by| varchar(8000)  |
| &#128270; | opened\_date| datetime2(26)  |
| &#128270; | closed\_date| datetime2(26)  |
| &#128270; | specification\_details| varchar(8000)  |
| &#128270; | notes| varchar(8000)  |
| &#128270; | finish| varchar(8000)  |
| &#128270; | previous\_dfm\_signed\_off| bit  |
| &#128270; | previous\_dfm\_date| datetime2(26)  |
| &#128270; | last\_dfm\_request\_no| varchar(8000)  |
| &#128270; | opportunity\_review| bit  |
| &#128270; | npi\_required| bit  |
| &#128270; | dfm\_design\_review| bit  |
| &#128270; | dfm\_design\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_manufacturing\_process\_review| bit  |
| &#128270; | dfm\_manufacturing\_process\_notes| varchar(8000)  |
| &#128270; | dfm\_materials\_review| bit  |
| &#128270; | dfm\_materials\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_3rd\_party\_review| bit  |
| &#128270; | dfm\_3rd\_party\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_samples\_mock\_up\_review| bit  |
| &#128270; | dfm\_samples\_mock\_up\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_finishes\_review| bit  |
| &#128270; | dfm\_finishes\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_tooling\_review| bit  |
| &#128270; | dfm\_tooling\_review\_notes| varchar(8000)  |
| &#128270; | dfm\_signed\_off| bit  |
| &#128270; | dfm\_sign\_off\_date| datetime2(26)  |
| &#128270; | dfm\_summary\_notes| varchar(8000)  |
| &#128270; | factory\_notes\_advised| bit  |
| &#128270; | factory\_design\_notes| varchar(8000)  |
| &#128270; | dfm\_signed\_off\_by| varchar(8000)  |
| &#128270; | days\_taken\_to\_close| decimal(38,18)  |
| &#128270; | proposal\_number| varchar(8000)  |
| &#128270; | estimated\_value| decimal(38,18)  |
| &#128270; | perforation\_mesh\_pattern| varchar(8000)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | colour| varchar(8000)  |
| &#128270; | grid\_detail| varchar(8000)  |
| &#128270; | perimeter\_detail| varchar(8000)  |
| &#128270; | infill\_details| varchar(8000)  |
| &#128270; | overdue| varchar(8000)  |
| &#128270; | overdue\_colour| varchar(8000)  |
| &#128270; | estimated\_completion\_date| datetime2(26)  |
| &#128270; | rating| varchar(8000)  |
| &#128270; | drawing\_quantity| varchar(8000)  |
| &#128270; | drawing\_numbers| varchar(8000)  |
| &#128270; | awaiting\_info\_start\_date| datetime2(26)  |
| &#128270; | awaiting\_info\_end\_date| datetime2(26)  |
| &#128270; | assigned\_start\_date| datetime2(26)  |
| &#128270; | assigned\_end\_date| datetime2(26)  |
| &#128270; | in\_progress\_start\_date| datetime2(26)  |
| &#128270; | in\_progress\_end\_date| datetime2(26)  |
| &#128270; | sign\_off\_required\_start\_date| datetime2(26)  |
| &#128270; | sign\_off\_required\_end\_date| datetime2(26)  |
| &#128270; | proposal\_owner| varchar(8000)  |
| &#128270; | new\_die\_required| bit  |
| &#128270; | technical\_development| bit  |
| &#128270; | secondary\_owner| varchar(8000)  |
| &#128270; | requested\_return\_date| datetime2(26)  |
| &#128270; | days\_in\_progress| decimal(38,18)  |
| &#128270; | rejected\_drawings| decimal(38,18)  |
| &#128270; | sales\_region| varchar(8000)  |
| &#128270; | opportunity\_review\_notes| varchar(8000)  |
| &#128270; | opportunity\_review\_approved| bit  |
| &#128270; | scope\_document\_uploaded| bit  |
| &#128270; | opportunity\_value| decimal(38,18)  |
| &#128270; | cost\_impact| varchar(8000)  |
| &#128270; | issued\_proposal\_drawing| varchar(8000)  |
| &#128270; | tags| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON record\_type\_id|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON company\_name|
| &#128270;  | ClusteredIndex | ON project\_name|
| &#128270;  | ClusteredIndex | ON contact\_name|
| &#128270;  | ClusteredIndex | ON infor\_reference\_number\_project|
| &#128270;  | ClusteredIndex | ON infor\_reference\_number\_account|
| &#128270;  | ClusteredIndex | ON complexity|
| &#128270;  | ClusteredIndex | ON complete\_by\_date|
| &#128270;  | ClusteredIndex | ON project\_owner|
| &#128270;  | ClusteredIndex | ON project\_secondary\_owner|
| &#128270;  | ClusteredIndex | ON project\_stage|
| &#128270;  | ClusteredIndex | ON project\_probability|
| &#128270;  | ClusteredIndex | ON project\_specification|
| &#128270;  | ClusteredIndex | ON days\_overdue|
| &#128270;  | ClusteredIndex | ON sharepoint|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_reason|
| &#128270;  | ClusteredIndex | ON review\_date|
| &#128270;  | ClusteredIndex | ON scope\_m2|
| &#128270;  | ClusteredIndex | ON commercial\_sign\_off\_by|
| &#128270;  | ClusteredIndex | ON design\_sign\_off\_by|
| &#128270;  | ClusteredIndex | ON opened\_date|
| &#128270;  | ClusteredIndex | ON closed\_date|
| &#128270;  | ClusteredIndex | ON specification\_details|
| &#128270;  | ClusteredIndex | ON notes|
| &#128270;  | ClusteredIndex | ON finish|
| &#128270;  | ClusteredIndex | ON previous\_dfm\_signed\_off|
| &#128270;  | ClusteredIndex | ON previous\_dfm\_date|
| &#128270;  | ClusteredIndex | ON last\_dfm\_request\_no|
| &#128270;  | ClusteredIndex | ON opportunity\_review|
| &#128270;  | ClusteredIndex | ON npi\_required|
| &#128270;  | ClusteredIndex | ON dfm\_design\_review|
| &#128270;  | ClusteredIndex | ON dfm\_design\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_manufacturing\_process\_review|
| &#128270;  | ClusteredIndex | ON dfm\_manufacturing\_process\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_materials\_review|
| &#128270;  | ClusteredIndex | ON dfm\_materials\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_3rd\_party\_review|
| &#128270;  | ClusteredIndex | ON dfm\_3rd\_party\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_samples\_mock\_up\_review|
| &#128270;  | ClusteredIndex | ON dfm\_samples\_mock\_up\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_finishes\_review|
| &#128270;  | ClusteredIndex | ON dfm\_finishes\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_tooling\_review|
| &#128270;  | ClusteredIndex | ON dfm\_tooling\_review\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_signed\_off|
| &#128270;  | ClusteredIndex | ON dfm\_sign\_off\_date|
| &#128270;  | ClusteredIndex | ON dfm\_summary\_notes|
| &#128270;  | ClusteredIndex | ON factory\_notes\_advised|
| &#128270;  | ClusteredIndex | ON factory\_design\_notes|
| &#128270;  | ClusteredIndex | ON dfm\_signed\_off\_by|
| &#128270;  | ClusteredIndex | ON days\_taken\_to\_close|
| &#128270;  | ClusteredIndex | ON proposal\_number|
| &#128270;  | ClusteredIndex | ON estimated\_value|
| &#128270;  | ClusteredIndex | ON perforation\_mesh\_pattern|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON colour|
| &#128270;  | ClusteredIndex | ON grid\_detail|
| &#128270;  | ClusteredIndex | ON perimeter\_detail|
| &#128270;  | ClusteredIndex | ON infill\_details|
| &#128270;  | ClusteredIndex | ON overdue|
| &#128270;  | ClusteredIndex | ON overdue\_colour|
| &#128270;  | ClusteredIndex | ON estimated\_completion\_date|
| &#128270;  | ClusteredIndex | ON rating|
| &#128270;  | ClusteredIndex | ON drawing\_quantity|
| &#128270;  | ClusteredIndex | ON drawing\_numbers|
| &#128270;  | ClusteredIndex | ON awaiting\_info\_start\_date|
| &#128270;  | ClusteredIndex | ON awaiting\_info\_end\_date|
| &#128270;  | ClusteredIndex | ON assigned\_start\_date|
| &#128270;  | ClusteredIndex | ON assigned\_end\_date|
| &#128270;  | ClusteredIndex | ON in\_progress\_start\_date|
| &#128270;  | ClusteredIndex | ON in\_progress\_end\_date|
| &#128270;  | ClusteredIndex | ON sign\_off\_required\_start\_date|
| &#128270;  | ClusteredIndex | ON sign\_off\_required\_end\_date|
| &#128270;  | ClusteredIndex | ON proposal\_owner|
| &#128270;  | ClusteredIndex | ON new\_die\_required|
| &#128270;  | ClusteredIndex | ON technical\_development|
| &#128270;  | ClusteredIndex | ON secondary\_owner|
| &#128270;  | ClusteredIndex | ON requested\_return\_date|
| &#128270;  | ClusteredIndex | ON days\_in\_progress|
| &#128270;  | ClusteredIndex | ON rejected\_drawings|
| &#128270;  | ClusteredIndex | ON sales\_region|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_notes|
| &#128270;  | ClusteredIndex | ON opportunity\_review\_approved|
| &#128270;  | ClusteredIndex | ON scope\_document\_uploaded|
| &#128270;  | ClusteredIndex | ON opportunity\_value|
| &#128270;  | ClusteredIndex | ON cost\_impact|
| &#128270;  | ClusteredIndex | ON issued\_proposal\_drawing|
| &#128270;  | ClusteredIndex | ON tags|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.record_type 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | name| varchar(8000)  |
| &#128270; | developer\_name| varchar(8000)  |
| &#128270; | namespace\_prefix| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | business\_process\_id| varchar(8000)  |
| &#128270; | sobject\_type| varchar(8000)  |
| &#128270; | is\_active| bit  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON developer\_name|
| &#128270;  | ClusteredIndex | ON namespace\_prefix|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON business\_process\_id|
| &#128270;  | ClusteredIndex | ON sobject\_type|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.sas_otif_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | line| int  |
| &#128270; | group| varchar(8000)  |
| &#128270; | ship\_date| datetime2(26)  |
| &#128270; | acknowledged\_date| datetime2(26)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | customer| varchar(8000)  |
| &#128270; | shipment\_detail| varchar(8000)  |
| &#128270; | otif| int  |
| &#128270; | commment| varchar(8000)  |
| &#128270; | fail\_code| varchar(8000)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | co\_num| varchar(8000)  |
| &#128270; | year| int  |
| &#128270; | week| int  |
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | in\_workflow| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | qty\_os| bigint  |
| &#128270; | line\_count| int  |
| &#128270; | included| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON line|
| &#128270;  | ClusteredIndex | ON group|
| &#128270;  | ClusteredIndex | ON ship\_date|
| &#128270;  | ClusteredIndex | ON acknowledged\_date|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON customer|
| &#128270;  | ClusteredIndex | ON shipment\_detail|
| &#128270;  | ClusteredIndex | ON otif|
| &#128270;  | ClusteredIndex | ON commment|
| &#128270;  | ClusteredIndex | ON fail\_code|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON co\_num|
| &#128270;  | ClusteredIndex | ON year|
| &#128270;  | ClusteredIndex | ON week|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON qty\_os|
| &#128270;  | ClusteredIndex | ON line\_count|
| &#128270;  | ClusteredIndex | ON included|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.sas_otif_sum_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | year| int  |
| &#128270; | week| int  |
| &#128270; | group| varchar(8000)  |
| &#128270; | otif\_no| int  |
| &#128270; | dels\_no| int  |
| &#128270; | otif\_pc| decimal(11,8)  |
| &#128270; | be| decimal(11,8)  |
| &#128270; | mb| decimal(11,8)  |
| &#128270; | rdg| decimal(11,8)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | in\_workflow| int  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | excl\_no| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON year|
| &#128270;  | ClusteredIndex | ON week|
| &#128270;  | ClusteredIndex | ON group|
| &#128270;  | ClusteredIndex | ON otif\_no|
| &#128270;  | ClusteredIndex | ON dels\_no|
| &#128270;  | ClusteredIndex | ON otif\_pc|
| &#128270;  | ClusteredIndex | ON be|
| &#128270;  | ClusteredIndex | ON mb|
| &#128270;  | ClusteredIndex | ON rdg|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON excl\_no|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.sbqq__quote 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | owner\_id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | record\_type\_id| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_activity\_date| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | sbqq\_\_account| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_city| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_country| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_frequency| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_name| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_postal\_code| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_state| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_street| varchar(8000)  |
| &#128270; | sbqq\_\_consumption\_rate\_override| bit  |
| &#128270; | sbqq\_\_contracting\_method| varchar(8000)  |
| &#128270; | sbqq\_\_customer\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_default\_template| varchar(8000)  |
| &#128270; | sbqq\_\_delivery\_method| varchar(8000)  |
| &#128270; | sbqq\_\_distributor\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_distributor| varchar(8000)  |
| &#128270; | sbqq\_\_document\_status| varchar(8000)  |
| &#128270; | sbqq\_\_email\_template\_id| varchar(8000)  |
| &#128270; | sbqq\_\_end\_date| datetime2(26)  |
| &#128270; | sbqq\_\_first\_segment\_term\_end\_date| datetime2(26)  |
| &#128270; | sbqq\_\_generate\_contracted\_price| varchar(8000)  |
| &#128270; | sbqq\_\_introduction| varchar(8000)  |
| &#128270; | sbqq\_\_key| varchar(8000)  |
| &#128270; | sbqq\_\_last\_calculated\_on| datetime2(26)  |
| &#128270; | sbqq\_\_last\_saved\_on| datetime2(26)  |
| &#128270; | sbqq\_\_line\_items\_grouped| bit  |
| &#128270; | sbqq\_\_line\_items\_printed| bit  |
| &#128270; | sbqq\_\_markup\_rate| decimal(38,18)  |
| &#128270; | sbqq\_\_master\_contract| varchar(8000)  |
| &#128270; | sbqq\_\_master\_evergreen\_contract| varchar(8000)  |
| &#128270; | sbqq\_\_notes| varchar(8000)  |
| &#128270; | sbqq\_\_opportunity2| varchar(8000)  |
| &#128270; | sbqq\_\_order\_by\_quote\_line\_group| bit  |
| &#128270; | sbqq\_\_order\_by| varchar(8000)  |
| &#128270; | sbqq\_\_order\_group\_id| varchar(8000)  |
| &#128270; | sbqq\_\_ordered| bit  |
| &#128270; | sbqq\_\_original\_quote| varchar(8000)  |
| &#128270; | sbqq\_\_paper\_size| varchar(8000)  |
| &#128270; | sbqq\_\_partner\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_partner| varchar(8000)  |
| &#128270; | sbqq\_\_payment\_terms| varchar(8000)  |
| &#128270; | sbqq\_\_price\_book| varchar(8000)  |
| &#128270; | sbqq\_\_pricebook\_id| varchar(8000)  |
| &#128270; | sbqq\_\_primary\_contact| varchar(8000)  |
| &#128270; | sbqq\_\_primary| bit  |
| &#128270; | sbqq\_\_proration\_day\_of\_month| varchar(8000)  |
| &#128270; | sbqq\_\_quote\_language| varchar(8000)  |
| &#128270; | sbqq\_\_quote\_process\_id| varchar(8000)  |
| &#128270; | sbqq\_\_quote\_template\_id| varchar(8000)  |
| &#128270; | sbqq\_\_renewal\_term| decimal(38,18)  |
| &#128270; | sbqq\_\_renewal\_uplift\_rate| decimal(38,18)  |
| &#128270; | sbqq\_\_sales\_rep| varchar(8000)  |
| &#128270; | sbqq\_\_shipping\_city| varchar(8000)  |
| &#128270; | sbqq\_\_shipping\_country| varchar(8000)  |
| &#128270; | sbqq\_\_shipping\_name| varchar(8000)  |
| &#128270; | sbqq\_\_shipping\_postal\_code| varchar(8000)  |
| &#128270; | sbqq\_\_shipping\_state| varchar(8000)  |
| &#128270; | sbqq\_\_shipping\_street| varchar(8000)  |
| &#128270; | sbqq\_\_source| varchar(8000)  |
| &#128270; | sbqq\_\_start\_date| datetime2(26)  |
| &#128270; | sbqq\_\_status| varchar(8000)  |
| &#128270; | sbqq\_\_subscription\_term| decimal(38,18)  |
| &#128270; | sbqq\_\_target\_customer\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_type| varchar(8000)  |
| &#128270; | sbqq\_\_unopened| bit  |
| &#128270; | sbqq\_\_watermark\_shown| bit  |
| &#128270; | sbqq\_\_line\_item\_count| decimal(38,18)  |
| &#128270; | sbqq\_\_additional\_discount\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_average\_customer\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_average\_partner\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_days\_quote\_open| decimal(38,18)  |
| &#128270; | sbqq\_\_expiration\_date| datetime2(26)  |
| &#128270; | sbqq\_\_total\_customer\_discount\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_uncalculated| bit  |
| &#128270; | sbqq\_\_customer\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_list\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_net\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_regular\_amount| decimal(38,18)  |
| &#128270; | account\_name| varchar(8000)  |
| &#128270; | approval\_status| varchar(8000)  |
| &#128270; | approved| bit  |
| &#128270; | approver\_1| varchar(8000)  |
| &#128270; | approver\_2| varchar(8000)  |
| &#128270; | approver\_bcr| varchar(8000)  |
| &#128270; | approver\_commercial\_sales\_manager| varchar(8000)  |
| &#128270; | approver\_estimating\_manager| varchar(8000)  |
| &#128270; | approver\_estimator| varchar(8000)  |
| &#128270; | approver\_senior\_estimator| varchar(8000)  |
| &#128270; | bcr\_escalation| bit  |
| &#128270; | budget\_rate\_text| varchar(8000)  |
| &#128270; | contact\_name\_for\_document| varchar(8000)  |
| &#128270; | estimating\_request| varchar(8000)  |
| &#128270; | estimator\_name\_for\_document| varchar(8000)  |
| &#128270; | expiration\_date\_text| varchar(8000)  |
| &#128270; | net\_amount\_converted| decimal(38,18)  |
| &#128270; | other\_info| varchar(8000)  |
| &#128270; | product\_image\_id| varchar(8000)  |
| &#128270; | project\_name\_for\_document| varchar(8000)  |
| &#128270; | project\_number\_for\_document| varchar(8000)  |
| &#128270; | quote\_complexity| varchar(8000)  |
| &#128270; | quote\_expired| bit  |
| &#128270; | quote\_term\_status| varchar(8000)  |
| &#128270; | quote\_type| varchar(8000)  |
| &#128270; | region| varchar(8000)  |
| &#128270; | submitted\_date| datetime2(26)  |
| &#128270; | submitted\_user| varchar(8000)  |
| &#128270; | todays\_date| datetime2(26)  |
| &#128270; | url| varchar(8000)  |
| &#128270; | total\_transfer\_price| decimal(38,18)  |
| &#128270; | estimating\_approval\_level| varchar(8000)  |
| &#128270; | estimating\_request\_no| varchar(8000)  |
| &#128270; | expiration\_date\_for\_document| varchar(8000)  |
| &#128270; | quoted\_margin| decimal(38,18)  |
| &#128270; | sqft\_rate| decimal(38,18)  |
| &#128270; | sqm\_rate| decimal(38,18)  |
| &#128270; | quote\_lf| decimal(38,18)  |
| &#128270; | quote\_lm| decimal(38,18)  |
| &#128270; | quote\_sqft| decimal(38,18)  |
| &#128270; | quote\_sqm| decimal(38,18)  |
| &#128270; | figures| bit  |
| &#128270; | quote\_date| datetime2(26)  |
| &#128270; | budget| bit  |
| &#128270; | request\_owner\_id| varchar(8000)  |
| &#128270; | infor\_project\_number| varchar(8000)  |
| &#128270; | contact\_first\_name\_formula| varchar(8000)  |
| &#128270; | project\_name\_formula| varchar(8000)  |
| &#128270; | quote\_status\_for\_syteline| varchar(8000)  |
| &#128270; | primary\_for\_syteline| decimal(38,18)  |
| &#128270; | closed\_date| datetime2(26)  |
| &#128270; | currency\_rate| decimal(38,18)  |
| &#128270; | make\_primary\_status| varchar(8000)  |
| &#128270; | a\_complexity\_lines| decimal(38,18)  |
| &#128270; | b\_complexity\_lines| decimal(38,18)  |
| &#128270; | c\_complexity\_lines| decimal(38,18)  |
| &#128270; | d\_complexity\_lines| decimal(38,18)  |
| &#128270; | currency\_mismatch| bit  |
| &#128270; | project\_original\_quoted\_value| decimal(38,18)  |
| &#128270; | project\_figures\_reported\_date| datetime2(26)  |
| &#128270; | lines\_with\_no\_price| decimal(38,18)  |
| &#128270; | target\_price| decimal(38,18)  |
| &#128270; | requested\_return\_date| datetime2(26)  |
| &#128270; | major\_project| bit  |
| &#128270; | lighting| bit  |
| &#128270; | take\_off\_required| bit  |
| &#128270; | freight\_type| varchar(8000)  |
| &#128270; | system\_type| varchar(8000)  |
| &#128270; | finish| varchar(8000)  |
| &#128270; | description| varchar(8000)  |
| &#128270; | dfm\_required| bit  |
| &#128270; | npi\_required| bit  |
| &#128270; | dfm\_design\_review| bit  |
| &#128270; | dfm\_manufacturing\_process\_review| bit  |
| &#128270; | dfm\_materials\_review| bit  |
| &#128270; | dfm\_3rd\_party\_review| bit  |
| &#128270; | dfm\_samples\_mock\_up\_review| bit  |
| &#128270; | dfm\_finishes\_review| bit  |
| &#128270; | dfm\_tooling\_review| bit  |
| &#128270; | dfm\_signed\_off| bit  |
| &#128270; | dfm\_notes| varchar(8000)  |
| &#128270; | bcr\_specification\_drawing\_review| bit  |
| &#128270; | bcr\_selling\_price\_review| bit  |
| &#128270; | bcr\_project\_risk| bit  |
| &#128270; | bcr\_financial\_review| bit  |
| &#128270; | bcr\_other\_considerations| bit  |
| &#128270; | bcr\_signed\_off| bit  |
| &#128270; | bcr\_notes| varchar(8000)  |
| &#128270; | bcr\_required| bit  |
| &#128270; | project\_stage| varchar(8000)  |
| &#128270; | order\_date| datetime2(26)  |
| &#128270; | project\_specification| varchar(8000)  |
| &#128270; | bcr\_value\_to\_be\_reviewed| decimal(38,18)  |
| &#128270; | estimated\_divisional\_margin| decimal(38,18)  |
| &#128270; | square\_meter\_rate\_per\_system| varchar(8000)  |
| &#128270; | investment\_machines\_tools| varchar(8000)  |
| &#128270; | cost\_vs\_tp\_vs\_sell| varchar(8000)  |
| &#128270; | value\_of\_carriage| decimal(38,18)  |
| &#128270; | bcr\_notes\_for\_review\_meeting| varchar(8000)  |
| &#128270; | bcr\_estimated\_through\_margin| varchar(8000)  |
| &#128270; | take\_off| varchar(8000)  |
| &#128270; | special\_materials| varchar(8000)  |
| &#128270; | value\_of\_design| varchar(8000)  |
| &#128270; | value\_of\_shop\_drawings| varchar(8000)  |
| &#128270; | costing\_notes| varchar(8000)  |
| &#128270; | lines\_with\_no\_costing\_method| decimal(38,18)  |
| &#128270; | make\_primary\_message| varchar(8000)  |
| &#128270; | cover\_pages| bit  |
| &#128270; | lines\_with\_no\_complexity| decimal(38,18)  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | office\_city| varchar(8000)  |
| &#128270; | office\_country| varchar(8000)  |
| &#128270; | office\_post\_code| varchar(8000)  |
| &#128270; | office\_street\_1| varchar(8000)  |
| &#128270; | office\_street\_2| varchar(8000)  |
| &#128270; | roe| varchar(8000)  |
| &#128270; | closed\_date\_time| datetime2(26)  |
| &#128270; | created\_date\_time| datetime2(26)  |
| &#128270; | hours\_taken\_to\_close| decimal(38,18)  |
| &#128270; | is\_region\_australia| bit  |
| &#128270; | is\_uk\_or\_export\_region| bit  |
| &#128270; | quote\_measurement| varchar(8000)  |
| &#128270; | project\_id| varchar(8000)  |
| &#128270; | estimating\_request\_id| varchar(8000)  |
| &#128270; | lines\_with\_no\_unit\_cost| decimal(38,18)  |
| &#128270; | quote\_term\_type| varchar(8000)  |
| &#128270; | commission\_payable\_rebates| decimal(38,18)  |
| &#128270; | total\_lines| decimal(38,18)  |
| &#128270; | total\_cost| decimal(38,18)  |
| &#128270; | tooling\_charge| decimal(38,18)  |
| &#128270; | tooling\_cost| decimal(38,18)  |
| &#128270; | freight\_charge| decimal(38,18)  |
| &#128270; | freight\_cost| decimal(38,18)  |
| &#128270; | design\_charge| decimal(38,18)  |
| &#128270; | design\_cost| decimal(38,18)  |
| &#128270; | project\_management\_service\_charge| decimal(38,18)  |
| &#128270; | project\_management\_service\_cost| decimal(38,18)  |
| &#128270; | set\_up\_cost| decimal(38,18)  |
| &#128270; | set\_up\_quantity| decimal(38,18)  |
| &#128270; | list\_margin| decimal(38,18)  |
| &#128270; | tariff| decimal(38,18)  |
| &#128270; | commercial\_margin| decimal(38,18)  |
| &#128270; | commercial\_margin\_percent| decimal(38,18)  |
| &#128270; | manufacturing\_margin| decimal(38,18)  |
| &#128270; | manufacturing\_margin\_percent| decimal(38,18)  |
| &#128270; | through\_margin| decimal(38,18)  |
| &#128270; | through\_margin\_percent| decimal(38,18)  |
| &#128270; | e2e\_division| decimal(38,18)  |
| &#128270; | e2e\_complexity| decimal(38,18)  |
| &#128270; | e2e\_division\_value| decimal(38,18)  |
| &#128270; | e2e\_complexity\_value| decimal(38,18)  |
| &#128270; | e2e\_cost| decimal(38,18)  |
| &#128270; | net\_project\_contribution| decimal(38,18)  |
| &#128270; | net\_project\_contribution\_percentage| decimal(38,18)  |
| &#128270; | division\_estimating| decimal(38,18)  |
| &#128270; | division\_costing| decimal(38,18)  |
| &#128270; | division\_sop| decimal(38,18)  |
| &#128270; | division\_design| decimal(38,18)  |
| &#128270; | division\_pdc| decimal(38,18)  |
| &#128270; | division\_product\_engineering| decimal(38,18)  |
| &#128270; | division\_scheduling| decimal(38,18)  |
| &#128270; | division\_quality| decimal(38,18)  |
| &#128270; | division\_production| decimal(38,18)  |
| &#128270; | division\_pm| decimal(38,18)  |
| &#128270; | complexity\_estimating| decimal(38,18)  |
| &#128270; | complexity\_costing| decimal(38,18)  |
| &#128270; | complexity\_sop| decimal(38,18)  |
| &#128270; | complexity\_design| decimal(38,18)  |
| &#128270; | complexity\_pdc| decimal(38,18)  |
| &#128270; | complexity\_product\_engineering| decimal(38,18)  |
| &#128270; | complexity\_scheduling| decimal(38,18)  |
| &#128270; | complexity\_quality| decimal(38,18)  |
| &#128270; | complexity\_production| decimal(38,18)  |
| &#128270; | complexity\_pm| decimal(38,18)  |
| &#128270; | estimating| decimal(38,18)  |
| &#128270; | costing| decimal(38,18)  |
| &#128270; | sop| decimal(38,18)  |
| &#128270; | design| decimal(38,18)  |
| &#128270; | pdc| decimal(38,18)  |
| &#128270; | production\_engineering| decimal(38,18)  |
| &#128270; | scheduling| decimal(38,18)  |
| &#128270; | quality| decimal(38,18)  |
| &#128270; | production\_management| decimal(38,18)  |
| &#128270; | project\_management| decimal(38,18)  |
| &#128270; | discount\_reason| varchar(8000)  |
| &#128270; | gm\_approval\_required| bit  |
| &#128270; | sales\_quote\_review| bit  |
| &#128270; | sales\_quote\_review\_completed| bit  |
| &#128270; | original\_quoted\_margin| decimal(38,18)  |
| &#128270; | agreed\_margin| decimal(38,18)  |
| &#128270; | sales\_quote\_review\_notes| varchar(8000)  |
| &#128270; | original\_net\_amount| decimal(38,18)  |
| &#128270; | change\_order\_number| varchar(8000)  |
| &#128270; | basis\_of\_change\_order| varchar(8000)  |
| &#128270; | co\_design\_value| decimal(38,18)  |
| &#128270; | co\_freight\_value| decimal(38,18)  |
| &#128270; | co\_material\_value| decimal(38,18)  |
| &#128270; | client\_approval\_status| varchar(8000)  |
| &#128270; | approved\_by| varchar(8000)  |
| &#128270; | approved\_date| datetime2(26)  |
| &#128270; | base\_customer\_po\_number| varchar(8000)  |
| &#128270; | base\_customer\_po\_date| datetime2(26)  |
| &#128270; | internal\_notes| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON owner\_id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON record\_type\_id|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_activity\_date|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_account|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_city|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_country|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_frequency|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_name|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_postal\_code|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_state|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_street|
| &#128270;  | ClusteredIndex | ON sbqq\_\_consumption\_rate\_override|
| &#128270;  | ClusteredIndex | ON sbqq\_\_contracting\_method|
| &#128270;  | ClusteredIndex | ON sbqq\_\_customer\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_default\_template|
| &#128270;  | ClusteredIndex | ON sbqq\_\_delivery\_method|
| &#128270;  | ClusteredIndex | ON sbqq\_\_distributor\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_distributor|
| &#128270;  | ClusteredIndex | ON sbqq\_\_document\_status|
| &#128270;  | ClusteredIndex | ON sbqq\_\_email\_template\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_end\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_first\_segment\_term\_end\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_generate\_contracted\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_introduction|
| &#128270;  | ClusteredIndex | ON sbqq\_\_key|
| &#128270;  | ClusteredIndex | ON sbqq\_\_last\_calculated\_on|
| &#128270;  | ClusteredIndex | ON sbqq\_\_last\_saved\_on|
| &#128270;  | ClusteredIndex | ON sbqq\_\_line\_items\_grouped|
| &#128270;  | ClusteredIndex | ON sbqq\_\_line\_items\_printed|
| &#128270;  | ClusteredIndex | ON sbqq\_\_markup\_rate|
| &#128270;  | ClusteredIndex | ON sbqq\_\_master\_contract|
| &#128270;  | ClusteredIndex | ON sbqq\_\_master\_evergreen\_contract|
| &#128270;  | ClusteredIndex | ON sbqq\_\_notes|
| &#128270;  | ClusteredIndex | ON sbqq\_\_opportunity2|
| &#128270;  | ClusteredIndex | ON sbqq\_\_order\_by\_quote\_line\_group|
| &#128270;  | ClusteredIndex | ON sbqq\_\_order\_by|
| &#128270;  | ClusteredIndex | ON sbqq\_\_order\_group\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_ordered|
| &#128270;  | ClusteredIndex | ON sbqq\_\_original\_quote|
| &#128270;  | ClusteredIndex | ON sbqq\_\_paper\_size|
| &#128270;  | ClusteredIndex | ON sbqq\_\_partner\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_partner|
| &#128270;  | ClusteredIndex | ON sbqq\_\_payment\_terms|
| &#128270;  | ClusteredIndex | ON sbqq\_\_price\_book|
| &#128270;  | ClusteredIndex | ON sbqq\_\_pricebook\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_primary\_contact|
| &#128270;  | ClusteredIndex | ON sbqq\_\_primary|
| &#128270;  | ClusteredIndex | ON sbqq\_\_proration\_day\_of\_month|
| &#128270;  | ClusteredIndex | ON sbqq\_\_quote\_language|
| &#128270;  | ClusteredIndex | ON sbqq\_\_quote\_process\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_quote\_template\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_renewal\_term|
| &#128270;  | ClusteredIndex | ON sbqq\_\_renewal\_uplift\_rate|
| &#128270;  | ClusteredIndex | ON sbqq\_\_sales\_rep|
| &#128270;  | ClusteredIndex | ON sbqq\_\_shipping\_city|
| &#128270;  | ClusteredIndex | ON sbqq\_\_shipping\_country|
| &#128270;  | ClusteredIndex | ON sbqq\_\_shipping\_name|
| &#128270;  | ClusteredIndex | ON sbqq\_\_shipping\_postal\_code|
| &#128270;  | ClusteredIndex | ON sbqq\_\_shipping\_state|
| &#128270;  | ClusteredIndex | ON sbqq\_\_shipping\_street|
| &#128270;  | ClusteredIndex | ON sbqq\_\_source|
| &#128270;  | ClusteredIndex | ON sbqq\_\_start\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_status|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_term|
| &#128270;  | ClusteredIndex | ON sbqq\_\_target\_customer\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_unopened|
| &#128270;  | ClusteredIndex | ON sbqq\_\_watermark\_shown|
| &#128270;  | ClusteredIndex | ON sbqq\_\_line\_item\_count|
| &#128270;  | ClusteredIndex | ON sbqq\_\_additional\_discount\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_average\_customer\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_average\_partner\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_days\_quote\_open|
| &#128270;  | ClusteredIndex | ON sbqq\_\_expiration\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_total\_customer\_discount\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_uncalculated|
| &#128270;  | ClusteredIndex | ON sbqq\_\_customer\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_list\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_net\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_regular\_amount|
| &#128270;  | ClusteredIndex | ON account\_name|
| &#128270;  | ClusteredIndex | ON approval\_status|
| &#128270;  | ClusteredIndex | ON approved|
| &#128270;  | ClusteredIndex | ON approver\_1|
| &#128270;  | ClusteredIndex | ON approver\_2|
| &#128270;  | ClusteredIndex | ON approver\_bcr|
| &#128270;  | ClusteredIndex | ON approver\_commercial\_sales\_manager|
| &#128270;  | ClusteredIndex | ON approver\_estimating\_manager|
| &#128270;  | ClusteredIndex | ON approver\_estimator|
| &#128270;  | ClusteredIndex | ON approver\_senior\_estimator|
| &#128270;  | ClusteredIndex | ON bcr\_escalation|
| &#128270;  | ClusteredIndex | ON budget\_rate\_text|
| &#128270;  | ClusteredIndex | ON contact\_name\_for\_document|
| &#128270;  | ClusteredIndex | ON estimating\_request|
| &#128270;  | ClusteredIndex | ON estimator\_name\_for\_document|
| &#128270;  | ClusteredIndex | ON expiration\_date\_text|
| &#128270;  | ClusteredIndex | ON net\_amount\_converted|
| &#128270;  | ClusteredIndex | ON other\_info|
| &#128270;  | ClusteredIndex | ON product\_image\_id|
| &#128270;  | ClusteredIndex | ON project\_name\_for\_document|
| &#128270;  | ClusteredIndex | ON project\_number\_for\_document|
| &#128270;  | ClusteredIndex | ON quote\_complexity|
| &#128270;  | ClusteredIndex | ON quote\_expired|
| &#128270;  | ClusteredIndex | ON quote\_term\_status|
| &#128270;  | ClusteredIndex | ON quote\_type|
| &#128270;  | ClusteredIndex | ON region|
| &#128270;  | ClusteredIndex | ON submitted\_date|
| &#128270;  | ClusteredIndex | ON submitted\_user|
| &#128270;  | ClusteredIndex | ON todays\_date|
| &#128270;  | ClusteredIndex | ON url|
| &#128270;  | ClusteredIndex | ON total\_transfer\_price|
| &#128270;  | ClusteredIndex | ON estimating\_approval\_level|
| &#128270;  | ClusteredIndex | ON estimating\_request\_no|
| &#128270;  | ClusteredIndex | ON expiration\_date\_for\_document|
| &#128270;  | ClusteredIndex | ON quoted\_margin|
| &#128270;  | ClusteredIndex | ON sqft\_rate|
| &#128270;  | ClusteredIndex | ON sqm\_rate|
| &#128270;  | ClusteredIndex | ON quote\_lf|
| &#128270;  | ClusteredIndex | ON quote\_lm|
| &#128270;  | ClusteredIndex | ON quote\_sqft|
| &#128270;  | ClusteredIndex | ON quote\_sqm|
| &#128270;  | ClusteredIndex | ON figures|
| &#128270;  | ClusteredIndex | ON quote\_date|
| &#128270;  | ClusteredIndex | ON budget|
| &#128270;  | ClusteredIndex | ON request\_owner\_id|
| &#128270;  | ClusteredIndex | ON infor\_project\_number|
| &#128270;  | ClusteredIndex | ON contact\_first\_name\_formula|
| &#128270;  | ClusteredIndex | ON project\_name\_formula|
| &#128270;  | ClusteredIndex | ON quote\_status\_for\_syteline|
| &#128270;  | ClusteredIndex | ON primary\_for\_syteline|
| &#128270;  | ClusteredIndex | ON closed\_date|
| &#128270;  | ClusteredIndex | ON currency\_rate|
| &#128270;  | ClusteredIndex | ON make\_primary\_status|
| &#128270;  | ClusteredIndex | ON a\_complexity\_lines|
| &#128270;  | ClusteredIndex | ON b\_complexity\_lines|
| &#128270;  | ClusteredIndex | ON c\_complexity\_lines|
| &#128270;  | ClusteredIndex | ON d\_complexity\_lines|
| &#128270;  | ClusteredIndex | ON currency\_mismatch|
| &#128270;  | ClusteredIndex | ON project\_original\_quoted\_value|
| &#128270;  | ClusteredIndex | ON project\_figures\_reported\_date|
| &#128270;  | ClusteredIndex | ON lines\_with\_no\_price|
| &#128270;  | ClusteredIndex | ON target\_price|
| &#128270;  | ClusteredIndex | ON requested\_return\_date|
| &#128270;  | ClusteredIndex | ON major\_project|
| &#128270;  | ClusteredIndex | ON lighting|
| &#128270;  | ClusteredIndex | ON take\_off\_required|
| &#128270;  | ClusteredIndex | ON freight\_type|
| &#128270;  | ClusteredIndex | ON system\_type|
| &#128270;  | ClusteredIndex | ON finish|
| &#128270;  | ClusteredIndex | ON description|
| &#128270;  | ClusteredIndex | ON dfm\_required|
| &#128270;  | ClusteredIndex | ON npi\_required|
| &#128270;  | ClusteredIndex | ON dfm\_design\_review|
| &#128270;  | ClusteredIndex | ON dfm\_manufacturing\_process\_review|
| &#128270;  | ClusteredIndex | ON dfm\_materials\_review|
| &#128270;  | ClusteredIndex | ON dfm\_3rd\_party\_review|
| &#128270;  | ClusteredIndex | ON dfm\_samples\_mock\_up\_review|
| &#128270;  | ClusteredIndex | ON dfm\_finishes\_review|
| &#128270;  | ClusteredIndex | ON dfm\_tooling\_review|
| &#128270;  | ClusteredIndex | ON dfm\_signed\_off|
| &#128270;  | ClusteredIndex | ON dfm\_notes|
| &#128270;  | ClusteredIndex | ON bcr\_specification\_drawing\_review|
| &#128270;  | ClusteredIndex | ON bcr\_selling\_price\_review|
| &#128270;  | ClusteredIndex | ON bcr\_project\_risk|
| &#128270;  | ClusteredIndex | ON bcr\_financial\_review|
| &#128270;  | ClusteredIndex | ON bcr\_other\_considerations|
| &#128270;  | ClusteredIndex | ON bcr\_signed\_off|
| &#128270;  | ClusteredIndex | ON bcr\_notes|
| &#128270;  | ClusteredIndex | ON bcr\_required|
| &#128270;  | ClusteredIndex | ON project\_stage|
| &#128270;  | ClusteredIndex | ON order\_date|
| &#128270;  | ClusteredIndex | ON project\_specification|
| &#128270;  | ClusteredIndex | ON bcr\_value\_to\_be\_reviewed|
| &#128270;  | ClusteredIndex | ON estimated\_divisional\_margin|
| &#128270;  | ClusteredIndex | ON square\_meter\_rate\_per\_system|
| &#128270;  | ClusteredIndex | ON investment\_machines\_tools|
| &#128270;  | ClusteredIndex | ON cost\_vs\_tp\_vs\_sell|
| &#128270;  | ClusteredIndex | ON value\_of\_carriage|
| &#128270;  | ClusteredIndex | ON bcr\_notes\_for\_review\_meeting|
| &#128270;  | ClusteredIndex | ON bcr\_estimated\_through\_margin|
| &#128270;  | ClusteredIndex | ON take\_off|
| &#128270;  | ClusteredIndex | ON special\_materials|
| &#128270;  | ClusteredIndex | ON value\_of\_design|
| &#128270;  | ClusteredIndex | ON value\_of\_shop\_drawings|
| &#128270;  | ClusteredIndex | ON costing\_notes|
| &#128270;  | ClusteredIndex | ON lines\_with\_no\_costing\_method|
| &#128270;  | ClusteredIndex | ON make\_primary\_message|
| &#128270;  | ClusteredIndex | ON cover\_pages|
| &#128270;  | ClusteredIndex | ON lines\_with\_no\_complexity|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON office\_city|
| &#128270;  | ClusteredIndex | ON office\_country|
| &#128270;  | ClusteredIndex | ON office\_post\_code|
| &#128270;  | ClusteredIndex | ON office\_street\_1|
| &#128270;  | ClusteredIndex | ON office\_street\_2|
| &#128270;  | ClusteredIndex | ON roe|
| &#128270;  | ClusteredIndex | ON closed\_date\_time|
| &#128270;  | ClusteredIndex | ON created\_date\_time|
| &#128270;  | ClusteredIndex | ON hours\_taken\_to\_close|
| &#128270;  | ClusteredIndex | ON is\_region\_australia|
| &#128270;  | ClusteredIndex | ON is\_uk\_or\_export\_region|
| &#128270;  | ClusteredIndex | ON quote\_measurement|
| &#128270;  | ClusteredIndex | ON project\_id|
| &#128270;  | ClusteredIndex | ON estimating\_request\_id|
| &#128270;  | ClusteredIndex | ON lines\_with\_no\_unit\_cost|
| &#128270;  | ClusteredIndex | ON quote\_term\_type|
| &#128270;  | ClusteredIndex | ON commission\_payable\_rebates|
| &#128270;  | ClusteredIndex | ON total\_lines|
| &#128270;  | ClusteredIndex | ON total\_cost|
| &#128270;  | ClusteredIndex | ON tooling\_charge|
| &#128270;  | ClusteredIndex | ON tooling\_cost|
| &#128270;  | ClusteredIndex | ON freight\_charge|
| &#128270;  | ClusteredIndex | ON freight\_cost|
| &#128270;  | ClusteredIndex | ON design\_charge|
| &#128270;  | ClusteredIndex | ON design\_cost|
| &#128270;  | ClusteredIndex | ON project\_management\_service\_charge|
| &#128270;  | ClusteredIndex | ON project\_management\_service\_cost|
| &#128270;  | ClusteredIndex | ON set\_up\_cost|
| &#128270;  | ClusteredIndex | ON set\_up\_quantity|
| &#128270;  | ClusteredIndex | ON list\_margin|
| &#128270;  | ClusteredIndex | ON tariff|
| &#128270;  | ClusteredIndex | ON commercial\_margin|
| &#128270;  | ClusteredIndex | ON commercial\_margin\_percent|
| &#128270;  | ClusteredIndex | ON manufacturing\_margin|
| &#128270;  | ClusteredIndex | ON manufacturing\_margin\_percent|
| &#128270;  | ClusteredIndex | ON through\_margin|
| &#128270;  | ClusteredIndex | ON through\_margin\_percent|
| &#128270;  | ClusteredIndex | ON e2e\_division|
| &#128270;  | ClusteredIndex | ON e2e\_complexity|
| &#128270;  | ClusteredIndex | ON e2e\_division\_value|
| &#128270;  | ClusteredIndex | ON e2e\_complexity\_value|
| &#128270;  | ClusteredIndex | ON e2e\_cost|
| &#128270;  | ClusteredIndex | ON net\_project\_contribution|
| &#128270;  | ClusteredIndex | ON net\_project\_contribution\_percentage|
| &#128270;  | ClusteredIndex | ON division\_estimating|
| &#128270;  | ClusteredIndex | ON division\_costing|
| &#128270;  | ClusteredIndex | ON division\_sop|
| &#128270;  | ClusteredIndex | ON division\_design|
| &#128270;  | ClusteredIndex | ON division\_pdc|
| &#128270;  | ClusteredIndex | ON division\_product\_engineering|
| &#128270;  | ClusteredIndex | ON division\_scheduling|
| &#128270;  | ClusteredIndex | ON division\_quality|
| &#128270;  | ClusteredIndex | ON division\_production|
| &#128270;  | ClusteredIndex | ON division\_pm|
| &#128270;  | ClusteredIndex | ON complexity\_estimating|
| &#128270;  | ClusteredIndex | ON complexity\_costing|
| &#128270;  | ClusteredIndex | ON complexity\_sop|
| &#128270;  | ClusteredIndex | ON complexity\_design|
| &#128270;  | ClusteredIndex | ON complexity\_pdc|
| &#128270;  | ClusteredIndex | ON complexity\_product\_engineering|
| &#128270;  | ClusteredIndex | ON complexity\_scheduling|
| &#128270;  | ClusteredIndex | ON complexity\_quality|
| &#128270;  | ClusteredIndex | ON complexity\_production|
| &#128270;  | ClusteredIndex | ON complexity\_pm|
| &#128270;  | ClusteredIndex | ON estimating|
| &#128270;  | ClusteredIndex | ON costing|
| &#128270;  | ClusteredIndex | ON sop|
| &#128270;  | ClusteredIndex | ON design|
| &#128270;  | ClusteredIndex | ON pdc|
| &#128270;  | ClusteredIndex | ON production\_engineering|
| &#128270;  | ClusteredIndex | ON scheduling|
| &#128270;  | ClusteredIndex | ON quality|
| &#128270;  | ClusteredIndex | ON production\_management|
| &#128270;  | ClusteredIndex | ON project\_management|
| &#128270;  | ClusteredIndex | ON discount\_reason|
| &#128270;  | ClusteredIndex | ON gm\_approval\_required|
| &#128270;  | ClusteredIndex | ON sales\_quote\_review|
| &#128270;  | ClusteredIndex | ON sales\_quote\_review\_completed|
| &#128270;  | ClusteredIndex | ON original\_quoted\_margin|
| &#128270;  | ClusteredIndex | ON agreed\_margin|
| &#128270;  | ClusteredIndex | ON sales\_quote\_review\_notes|
| &#128270;  | ClusteredIndex | ON original\_net\_amount|
| &#128270;  | ClusteredIndex | ON change\_order\_number|
| &#128270;  | ClusteredIndex | ON basis\_of\_change\_order|
| &#128270;  | ClusteredIndex | ON co\_design\_value|
| &#128270;  | ClusteredIndex | ON co\_freight\_value|
| &#128270;  | ClusteredIndex | ON co\_material\_value|
| &#128270;  | ClusteredIndex | ON client\_approval\_status|
| &#128270;  | ClusteredIndex | ON approved\_by|
| &#128270;  | ClusteredIndex | ON approved\_date|
| &#128270;  | ClusteredIndex | ON base\_customer\_po\_number|
| &#128270;  | ClusteredIndex | ON base\_customer\_po\_date|
| &#128270;  | ClusteredIndex | ON internal\_notes|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.sbqq__quote_line 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | is\_deleted| bit  |
| &#128270; | name| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | sbqq\_\_quote| varchar(8000)  |
| &#128270; | sbqq\_\_additional\_discount\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_additional\_quantity| decimal(38,18)  |
| &#128270; | sbqq\_\_allow\_asset\_refund| bit  |
| &#128270; | sbqq\_\_batch\_quantity| decimal(38,18)  |
| &#128270; | sbqq\_\_billing\_frequency| varchar(8000)  |
| &#128270; | sbqq\_\_billing\_type| varchar(8000)  |
| &#128270; | sbqq\_\_block\_price| varchar(8000)  |
| &#128270; | sbqq\_\_bundle| bit  |
| &#128270; | sbqq\_\_bundled\_quantity| decimal(38,18)  |
| &#128270; | sbqq\_\_bundled| bit  |
| &#128270; | sbqq\_\_carryover\_line| bit  |
| &#128270; | sbqq\_\_charge\_type| varchar(8000)  |
| &#128270; | sbqq\_\_component\_cost| decimal(38,18)  |
| &#128270; | sbqq\_\_component\_discounted\_by\_package| bit  |
| &#128270; | sbqq\_\_component\_list\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_component\_subscription\_scope| varchar(8000)  |
| &#128270; | sbqq\_\_component\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_component\_uplifted\_by\_package| bit  |
| &#128270; | sbqq\_\_compound\_discount\_rate| decimal(38,18)  |
| &#128270; | sbqq\_\_configuration\_required| bit  |
| &#128270; | sbqq\_\_contracted\_price| varchar(8000)  |
| &#128270; | sbqq\_\_cost\_editable| bit  |
| &#128270; | sbqq\_\_cost| varchar(8000)  |
| &#128270; | sbqq\_\_customer\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_default\_subscription\_term| decimal(38,18)  |
| &#128270; | sbqq\_\_description| varchar(8000)  |
| &#128270; | sbqq\_\_dimension| varchar(8000)  |
| &#128270; | sbqq\_\_discount\_schedule\_type| varchar(8000)  |
| &#128270; | sbqq\_\_discount\_schedule| varchar(8000)  |
| &#128270; | sbqq\_\_discount\_tier| varchar(8000)  |
| &#128270; | sbqq\_\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_distributor\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_dynamic\_option\_id| varchar(8000)  |
| &#128270; | sbqq\_\_earliest\_valid\_amendment\_start\_date| datetime2(26)  |
| &#128270; | sbqq\_\_end\_date| datetime2(26)  |
| &#128270; | sbqq\_\_existing| bit  |
| &#128270; | sbqq\_\_favorite| varchar(8000)  |
| &#128270; | sbqq\_\_generate\_contracted\_price| varchar(8000)  |
| &#128270; | sbqq\_\_gross\_profit| decimal(38,18)  |
| &#128270; | sbqq\_\_group| varchar(8000)  |
| &#128270; | sbqq\_\_guidance| decimal(38,18)  |
| &#128270; | sbqq\_\_has\_consumption\_schedule| bit  |
| &#128270; | sbqq\_\_hidden| bit  |
| &#128270; | sbqq\_\_incomplete| bit  |
| &#128270; | sbqq\_\_list\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_markup\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_markup\_rate| decimal(38,18)  |
| &#128270; | sbqq\_\_maximum\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_minimum\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_net\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_non\_discountable| bit  |
| &#128270; | sbqq\_\_non\_partner\_discountable| bit  |
| &#128270; | sbqq\_\_number| decimal(38,18)  |
| &#128270; | sbqq\_\_option\_discount\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_option\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_option\_level| decimal(38,18)  |
| &#128270; | sbqq\_\_option\_type| varchar(8000)  |
| &#128270; | sbqq\_\_optional| bit  |
| &#128270; | sbqq\_\_original\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_original\_quote\_line\_id| varchar(8000)  |
| &#128270; | sbqq\_\_original\_unit\_cost| decimal(38,18)  |
| &#128270; | sbqq\_\_package\_product\_code| varchar(8000)  |
| &#128270; | sbqq\_\_package\_product\_description| varchar(8000)  |
| &#128270; | sbqq\_\_partner\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_partner\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_previous\_segment\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_previous\_segment\_uplift| decimal(38,18)  |
| &#128270; | sbqq\_\_price\_editable| bit  |
| &#128270; | sbqq\_\_pricebook\_entry\_id| varchar(8000)  |
| &#128270; | sbqq\_\_pricing\_method\_editable| bit  |
| &#128270; | sbqq\_\_pricing\_method| varchar(8000)  |
| &#128270; | sbqq\_\_prior\_quantity| decimal(38,18)  |
| &#128270; | sbqq\_\_product\_option| varchar(8000)  |
| &#128270; | sbqq\_\_product\_subscription\_type| varchar(8000)  |
| &#128270; | sbqq\_\_product| varchar(8000)  |
| &#128270; | sbqq\_\_prorate\_multiplier| decimal(38,18)  |
| &#128270; | sbqq\_\_prorated\_list\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_prorated\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_quantity| decimal(38,18)  |
| &#128270; | sbqq\_\_regular\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_renewal| bit  |
| &#128270; | sbqq\_\_renewed\_asset| varchar(8000)  |
| &#128270; | sbqq\_\_renewed\_subscription| varchar(8000)  |
| &#128270; | sbqq\_\_required\_by| varchar(8000)  |
| &#128270; | sbqq\_\_segment\_index| decimal(38,18)  |
| &#128270; | sbqq\_\_segment\_key| varchar(8000)  |
| &#128270; | sbqq\_\_segment\_label| varchar(8000)  |
| &#128270; | sbqq\_\_source| varchar(8000)  |
| &#128270; | sbqq\_\_special\_price\_description| varchar(8000)  |
| &#128270; | sbqq\_\_special\_price\_type| varchar(8000)  |
| &#128270; | sbqq\_\_special\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_start\_date| datetime2(26)  |
| &#128270; | sbqq\_\_subscribed\_asset\_ids| varchar(8000)  |
| &#128270; | sbqq\_\_subscription\_base| varchar(8000)  |
| &#128270; | sbqq\_\_subscription\_category| varchar(8000)  |
| &#128270; | sbqq\_\_subscription\_percent| decimal(38,18)  |
| &#128270; | sbqq\_\_subscription\_pricing| varchar(8000)  |
| &#128270; | sbqq\_\_subscription\_scope| varchar(8000)  |
| &#128270; | sbqq\_\_subscription\_target\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_subscription\_term| decimal(38,18)  |
| &#128270; | sbqq\_\_tax\_code| varchar(8000)  |
| &#128270; | sbqq\_\_taxable| bit  |
| &#128270; | sbqq\_\_term\_discount\_schedule| varchar(8000)  |
| &#128270; | sbqq\_\_term\_discount\_tier| varchar(8000)  |
| &#128270; | sbqq\_\_term\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_unit\_cost| decimal(38,18)  |
| &#128270; | sbqq\_\_unprorated\_net\_price| decimal(38,18)  |
| &#128270; | sbqq\_\_upgraded\_asset| varchar(8000)  |
| &#128270; | sbqq\_\_upgraded\_quantity| decimal(38,18)  |
| &#128270; | sbqq\_\_upgraded\_subscription| varchar(8000)  |
| &#128270; | sbqq\_\_uplift\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_uplift| decimal(38,18)  |
| &#128270; | sbqq\_\_volume\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_additional\_discount| decimal(38,18)  |
| &#128270; | sbqq\_\_component\_visibility| varchar(8000)  |
| &#128270; | sbqq\_\_customer\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_effective\_end\_date| datetime2(26)  |
| &#128270; | sbqq\_\_effective\_quantity| decimal(38,18)  |
| &#128270; | sbqq\_\_effective\_start\_date| datetime2(26)  |
| &#128270; | sbqq\_\_effective\_subscription\_term| decimal(38,18)  |
| &#128270; | sbqq\_\_list\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_markup| decimal(38,18)  |
| &#128270; | sbqq\_\_net\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_package\_cost| decimal(38,18)  |
| &#128270; | sbqq\_\_package\_list\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_package\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_partner\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_product\_code| varchar(8000)  |
| &#128270; | sbqq\_\_product\_family| varchar(8000)  |
| &#128270; | sbqq\_\_product\_name| varchar(8000)  |
| &#128270; | sbqq\_\_regular\_total| decimal(38,18)  |
| &#128270; | sbqq\_\_subscription\_type| varchar(8000)  |
| &#128270; | sbqq\_\_total\_discount\_amount| decimal(38,18)  |
| &#128270; | sbqq\_\_total\_discount\_rate| decimal(38,18)  |
| &#128270; | abutment\_detail| varchar(8000)  |
| &#128270; | additional\_information| varchar(8000)  |
| &#128270; | aperture\_offset| varchar(8000)  |
| &#128270; | aperture\_size| varchar(8000)  |
| &#128270; | aperture\_type| varchar(8000)  |
| &#128270; | area\_m| decimal(38,18)  |
| &#128270; | birdsmouth\_detail| varchar(8000)  |
| &#128270; | border| varchar(8000)  |
| &#128270; | budget\_rate\_description| varchar(8000)  |
| &#128270; | c\_profile\_noggin\_width\_mm| decimal(38,18)  |
| &#128270; | c\_profile\_type| varchar(8000)  |
| &#128270; | c\_profile\_width\_mm| varchar(8000)  |
| &#128270; | calculation\_type| varchar(8000)  |
| &#128270; | calculation| varchar(8000)  |
| &#128270; | carrier\_centres\_m| decimal(38,18)  |
| &#128270; | cell\_size| varchar(8000)  |
| &#128270; | centres| decimal(38,18)  |
| &#128270; | configuration| varchar(8000)  |
| &#128270; | corridor\_length\_m| decimal(38,18)  |
| &#128270; | custom\_estimating\_product| bit  |
| &#128270; | diameter\_offset| varchar(8000)  |
| &#128270; | diameter\_size| decimal(38,18)  |
| &#128270; | edge\_detail\_grid| varchar(8000)  |
| &#128270; | emac\_channel\_centres| varchar(8000)  |
| &#128270; | finish| varchar(8000)  |
| &#128270; | galv| bit  |
| &#128270; | gasket| varchar(8000)  |
| &#128270; | grid\_work| varchar(8000)  |
| &#128270; | high\_risk| decimal(38,18)  |
| &#128270; | insulation\_type| varchar(8000)  |
| &#128270; | lm\_rate| decimal(38,18)  |
| &#128270; | length| decimal(38,18)  |
| &#128270; | low\_risk| decimal(38,18)  |
| &#128270; | margin| decimal(38,18)  |
| &#128270; | market\_price\_reference| varchar(8000)  |
| &#128270; | material\_type| varchar(8000)  |
| &#128270; | medium\_risk| decimal(38,18)  |
| &#128270; | module\_type| varchar(8000)  |
| &#128270; | module| varchar(8000)  |
| &#128270; | nominal\_width| decimal(38,18)  |
| &#128270; | nominal\_length| decimal(38,18)  |
| &#128270; | notes| varchar(8000)  |
| &#128270; | parent\_product| varchar(8000)  |
| &#128270; | perf| varchar(8000)  |
| &#128270; | product\_type| varchar(8000)  |
| &#128270; | profile\_centres\_m| decimal(38,18)  |
| &#128270; | profile\_depth\_mm| varchar(8000)  |
| &#128270; | profile\_width\_mm| varchar(8000)  |
| &#128270; | profile| varchar(8000)  |
| &#128270; | qualification| varchar(8000)  |
| &#128270; | quant\_calc\_1\_quantity| decimal(38,18)  |
| &#128270; | ral\_colour| varchar(8000)  |
| &#128270; | rate| decimal(38,18)  |
| &#128270; | ref\_for\_doc| varchar(8000)  |
| &#128270; | sq\_m\_quantity| decimal(38,18)  |
| &#128270; | sqm\_rate| decimal(38,18)  |
| &#128270; | summary\_product| bit  |
| &#128270; | system\_type| varchar(8000)  |
| &#128270; | tile\_flange\_config| varchar(8000)  |
| &#128270; | tile\_length\_coefficient| decimal(38,18)  |
| &#128270; | tile\_length\_mm| decimal(38,18)  |
| &#128270; | tile\_quantity\_ea| decimal(38,18)  |
| &#128270; | tile\_size\_j\_bar\_side\_mm| decimal(38,18)  |
| &#128270; | tile\_size\_mm| decimal(38,18)  |
| &#128270; | tile\_width\_mm| decimal(38,18)  |
| &#128270; | tiles\_per\_box| decimal(38,18)  |
| &#128270; | tiles| varchar(8000)  |
| &#128270; | total\_area\_m2| decimal(38,18)  |
| &#128270; | total\_tile\_quantity| decimal(38,18)  |
| &#128270; | tube\_centres\_m| decimal(38,18)  |
| &#128270; | tube\_diameter| varchar(8000)  |
| &#128270; | uom\_n\_only| varchar(8000)  |
| &#128270; | width| decimal(38,18)  |
| &#128270; | estimating\_product\_description| varchar(8000)  |
| &#128270; | grid\_type| varchar(8000)  |
| &#128270; | item\_l\_f| decimal(38,18)  |
| &#128270; | item\_l\_m| decimal(38,18)  |
| &#128270; | item\_sqft| decimal(38,18)  |
| &#128270; | item\_sqm| decimal(38,18)  |
| &#128270; | lf| decimal(38,18)  |
| &#128270; | lm| decimal(38,18)  |
| &#128270; | length\_inches| decimal(38,18)  |
| &#128270; | line\_l\_f| decimal(38,18)  |
| &#128270; | line\_l\_m| decimal(38,18)  |
| &#128270; | line\_sqft| decimal(38,18)  |
| &#128270; | line\_sqm| decimal(38,18)  |
| &#128270; | product\_image| varchar(8000)  |
| &#128270; | risk\_level\_formula| varchar(8000)  |
| &#128270; | risk| varchar(8000)  |
| &#128270; | sqft| decimal(38,18)  |
| &#128270; | sqm| decimal(38,18)  |
| &#128270; | unit\_ft| varchar(8000)  |
| &#128270; | unit\_m| varchar(8000)  |
| &#128270; | width\_inches| decimal(38,18)  |
| &#128270; | product\_name\_formula| varchar(8000)  |
| &#128270; | costing\_method| varchar(8000)  |
| &#128270; | uom\_ea\_only| varchar(8000)  |
| &#128270; | unit\_cost\_gbp| decimal(38,18)  |
| &#128270; | complexity| varchar(8000)  |
| &#128270; | quote\_discount| decimal(38,18)  |
| &#128270; | price\_excluded| bit  |
| &#128270; | measurement\_type| varchar(8000)  |
| &#128270; | length\_ft| decimal(38,18)  |
| &#128270; | length\_inch| decimal(38,18)  |
| &#128270; | width\_ft| decimal(38,18)  |
| &#128270; | width\_inch| decimal(38,18)  |
| &#128270; | clip\_finish| varchar(8000)  |
| &#128270; | manufacture\_source| varchar(8000)  |
| &#128270; | source\_reason| varchar(8000)  |
| &#128270; | item\_cost| decimal(38,18)  |
| &#128270; | line\_cost| decimal(38,18)  |
| &#128270; | costed\_item\_number| varchar(8000)  |
| &#128270; | total\_cost\_4\_r| decimal(38,18)  |
| &#128270; | product\_name\_4\_r| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON is\_deleted|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_quote|
| &#128270;  | ClusteredIndex | ON sbqq\_\_additional\_discount\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_additional\_quantity|
| &#128270;  | ClusteredIndex | ON sbqq\_\_allow\_asset\_refund|
| &#128270;  | ClusteredIndex | ON sbqq\_\_batch\_quantity|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_frequency|
| &#128270;  | ClusteredIndex | ON sbqq\_\_billing\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_block\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_bundle|
| &#128270;  | ClusteredIndex | ON sbqq\_\_bundled\_quantity|
| &#128270;  | ClusteredIndex | ON sbqq\_\_bundled|
| &#128270;  | ClusteredIndex | ON sbqq\_\_carryover\_line|
| &#128270;  | ClusteredIndex | ON sbqq\_\_charge\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_component\_cost|
| &#128270;  | ClusteredIndex | ON sbqq\_\_component\_discounted\_by\_package|
| &#128270;  | ClusteredIndex | ON sbqq\_\_component\_list\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_component\_subscription\_scope|
| &#128270;  | ClusteredIndex | ON sbqq\_\_component\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_component\_uplifted\_by\_package|
| &#128270;  | ClusteredIndex | ON sbqq\_\_compound\_discount\_rate|
| &#128270;  | ClusteredIndex | ON sbqq\_\_configuration\_required|
| &#128270;  | ClusteredIndex | ON sbqq\_\_contracted\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_cost\_editable|
| &#128270;  | ClusteredIndex | ON sbqq\_\_cost|
| &#128270;  | ClusteredIndex | ON sbqq\_\_customer\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_default\_subscription\_term|
| &#128270;  | ClusteredIndex | ON sbqq\_\_description|
| &#128270;  | ClusteredIndex | ON sbqq\_\_dimension|
| &#128270;  | ClusteredIndex | ON sbqq\_\_discount\_schedule\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_discount\_schedule|
| &#128270;  | ClusteredIndex | ON sbqq\_\_discount\_tier|
| &#128270;  | ClusteredIndex | ON sbqq\_\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_distributor\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_dynamic\_option\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_earliest\_valid\_amendment\_start\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_end\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_existing|
| &#128270;  | ClusteredIndex | ON sbqq\_\_favorite|
| &#128270;  | ClusteredIndex | ON sbqq\_\_generate\_contracted\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_gross\_profit|
| &#128270;  | ClusteredIndex | ON sbqq\_\_group|
| &#128270;  | ClusteredIndex | ON sbqq\_\_guidance|
| &#128270;  | ClusteredIndex | ON sbqq\_\_has\_consumption\_schedule|
| &#128270;  | ClusteredIndex | ON sbqq\_\_hidden|
| &#128270;  | ClusteredIndex | ON sbqq\_\_incomplete|
| &#128270;  | ClusteredIndex | ON sbqq\_\_list\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_markup\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_markup\_rate|
| &#128270;  | ClusteredIndex | ON sbqq\_\_maximum\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_minimum\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_net\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_non\_discountable|
| &#128270;  | ClusteredIndex | ON sbqq\_\_non\_partner\_discountable|
| &#128270;  | ClusteredIndex | ON sbqq\_\_number|
| &#128270;  | ClusteredIndex | ON sbqq\_\_option\_discount\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_option\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_option\_level|
| &#128270;  | ClusteredIndex | ON sbqq\_\_option\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_optional|
| &#128270;  | ClusteredIndex | ON sbqq\_\_original\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_original\_quote\_line\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_original\_unit\_cost|
| &#128270;  | ClusteredIndex | ON sbqq\_\_package\_product\_code|
| &#128270;  | ClusteredIndex | ON sbqq\_\_package\_product\_description|
| &#128270;  | ClusteredIndex | ON sbqq\_\_partner\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_partner\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_previous\_segment\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_previous\_segment\_uplift|
| &#128270;  | ClusteredIndex | ON sbqq\_\_price\_editable|
| &#128270;  | ClusteredIndex | ON sbqq\_\_pricebook\_entry\_id|
| &#128270;  | ClusteredIndex | ON sbqq\_\_pricing\_method\_editable|
| &#128270;  | ClusteredIndex | ON sbqq\_\_pricing\_method|
| &#128270;  | ClusteredIndex | ON sbqq\_\_prior\_quantity|
| &#128270;  | ClusteredIndex | ON sbqq\_\_product\_option|
| &#128270;  | ClusteredIndex | ON sbqq\_\_product\_subscription\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_product|
| &#128270;  | ClusteredIndex | ON sbqq\_\_prorate\_multiplier|
| &#128270;  | ClusteredIndex | ON sbqq\_\_prorated\_list\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_prorated\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_quantity|
| &#128270;  | ClusteredIndex | ON sbqq\_\_regular\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_renewal|
| &#128270;  | ClusteredIndex | ON sbqq\_\_renewed\_asset|
| &#128270;  | ClusteredIndex | ON sbqq\_\_renewed\_subscription|
| &#128270;  | ClusteredIndex | ON sbqq\_\_required\_by|
| &#128270;  | ClusteredIndex | ON sbqq\_\_segment\_index|
| &#128270;  | ClusteredIndex | ON sbqq\_\_segment\_key|
| &#128270;  | ClusteredIndex | ON sbqq\_\_segment\_label|
| &#128270;  | ClusteredIndex | ON sbqq\_\_source|
| &#128270;  | ClusteredIndex | ON sbqq\_\_special\_price\_description|
| &#128270;  | ClusteredIndex | ON sbqq\_\_special\_price\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_special\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_start\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscribed\_asset\_ids|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_base|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_category|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_percent|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_pricing|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_scope|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_target\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_term|
| &#128270;  | ClusteredIndex | ON sbqq\_\_tax\_code|
| &#128270;  | ClusteredIndex | ON sbqq\_\_taxable|
| &#128270;  | ClusteredIndex | ON sbqq\_\_term\_discount\_schedule|
| &#128270;  | ClusteredIndex | ON sbqq\_\_term\_discount\_tier|
| &#128270;  | ClusteredIndex | ON sbqq\_\_term\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_unit\_cost|
| &#128270;  | ClusteredIndex | ON sbqq\_\_unprorated\_net\_price|
| &#128270;  | ClusteredIndex | ON sbqq\_\_upgraded\_asset|
| &#128270;  | ClusteredIndex | ON sbqq\_\_upgraded\_quantity|
| &#128270;  | ClusteredIndex | ON sbqq\_\_upgraded\_subscription|
| &#128270;  | ClusteredIndex | ON sbqq\_\_uplift\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_uplift|
| &#128270;  | ClusteredIndex | ON sbqq\_\_volume\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_additional\_discount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_component\_visibility|
| &#128270;  | ClusteredIndex | ON sbqq\_\_customer\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_effective\_end\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_effective\_quantity|
| &#128270;  | ClusteredIndex | ON sbqq\_\_effective\_start\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_effective\_subscription\_term|
| &#128270;  | ClusteredIndex | ON sbqq\_\_list\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_markup|
| &#128270;  | ClusteredIndex | ON sbqq\_\_net\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_package\_cost|
| &#128270;  | ClusteredIndex | ON sbqq\_\_package\_list\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_package\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_partner\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_product\_code|
| &#128270;  | ClusteredIndex | ON sbqq\_\_product\_family|
| &#128270;  | ClusteredIndex | ON sbqq\_\_product\_name|
| &#128270;  | ClusteredIndex | ON sbqq\_\_regular\_total|
| &#128270;  | ClusteredIndex | ON sbqq\_\_subscription\_type|
| &#128270;  | ClusteredIndex | ON sbqq\_\_total\_discount\_amount|
| &#128270;  | ClusteredIndex | ON sbqq\_\_total\_discount\_rate|
| &#128270;  | ClusteredIndex | ON abutment\_detail|
| &#128270;  | ClusteredIndex | ON additional\_information|
| &#128270;  | ClusteredIndex | ON aperture\_offset|
| &#128270;  | ClusteredIndex | ON aperture\_size|
| &#128270;  | ClusteredIndex | ON aperture\_type|
| &#128270;  | ClusteredIndex | ON area\_m|
| &#128270;  | ClusteredIndex | ON birdsmouth\_detail|
| &#128270;  | ClusteredIndex | ON border|
| &#128270;  | ClusteredIndex | ON budget\_rate\_description|
| &#128270;  | ClusteredIndex | ON c\_profile\_noggin\_width\_mm|
| &#128270;  | ClusteredIndex | ON c\_profile\_type|
| &#128270;  | ClusteredIndex | ON c\_profile\_width\_mm|
| &#128270;  | ClusteredIndex | ON calculation\_type|
| &#128270;  | ClusteredIndex | ON calculation|
| &#128270;  | ClusteredIndex | ON carrier\_centres\_m|
| &#128270;  | ClusteredIndex | ON cell\_size|
| &#128270;  | ClusteredIndex | ON centres|
| &#128270;  | ClusteredIndex | ON configuration|
| &#128270;  | ClusteredIndex | ON corridor\_length\_m|
| &#128270;  | ClusteredIndex | ON custom\_estimating\_product|
| &#128270;  | ClusteredIndex | ON diameter\_offset|
| &#128270;  | ClusteredIndex | ON diameter\_size|
| &#128270;  | ClusteredIndex | ON edge\_detail\_grid|
| &#128270;  | ClusteredIndex | ON emac\_channel\_centres|
| &#128270;  | ClusteredIndex | ON finish|
| &#128270;  | ClusteredIndex | ON galv|
| &#128270;  | ClusteredIndex | ON gasket|
| &#128270;  | ClusteredIndex | ON grid\_work|
| &#128270;  | ClusteredIndex | ON high\_risk|
| &#128270;  | ClusteredIndex | ON insulation\_type|
| &#128270;  | ClusteredIndex | ON lm\_rate|
| &#128270;  | ClusteredIndex | ON length|
| &#128270;  | ClusteredIndex | ON low\_risk|
| &#128270;  | ClusteredIndex | ON margin|
| &#128270;  | ClusteredIndex | ON market\_price\_reference|
| &#128270;  | ClusteredIndex | ON material\_type|
| &#128270;  | ClusteredIndex | ON medium\_risk|
| &#128270;  | ClusteredIndex | ON module\_type|
| &#128270;  | ClusteredIndex | ON module|
| &#128270;  | ClusteredIndex | ON nominal\_width|
| &#128270;  | ClusteredIndex | ON nominal\_length|
| &#128270;  | ClusteredIndex | ON notes|
| &#128270;  | ClusteredIndex | ON parent\_product|
| &#128270;  | ClusteredIndex | ON perf|
| &#128270;  | ClusteredIndex | ON product\_type|
| &#128270;  | ClusteredIndex | ON profile\_centres\_m|
| &#128270;  | ClusteredIndex | ON profile\_depth\_mm|
| &#128270;  | ClusteredIndex | ON profile\_width\_mm|
| &#128270;  | ClusteredIndex | ON profile|
| &#128270;  | ClusteredIndex | ON qualification|
| &#128270;  | ClusteredIndex | ON quant\_calc\_1\_quantity|
| &#128270;  | ClusteredIndex | ON ral\_colour|
| &#128270;  | ClusteredIndex | ON rate|
| &#128270;  | ClusteredIndex | ON ref\_for\_doc|
| &#128270;  | ClusteredIndex | ON sq\_m\_quantity|
| &#128270;  | ClusteredIndex | ON sqm\_rate|
| &#128270;  | ClusteredIndex | ON summary\_product|
| &#128270;  | ClusteredIndex | ON system\_type|
| &#128270;  | ClusteredIndex | ON tile\_flange\_config|
| &#128270;  | ClusteredIndex | ON tile\_length\_coefficient|
| &#128270;  | ClusteredIndex | ON tile\_length\_mm|
| &#128270;  | ClusteredIndex | ON tile\_quantity\_ea|
| &#128270;  | ClusteredIndex | ON tile\_size\_j\_bar\_side\_mm|
| &#128270;  | ClusteredIndex | ON tile\_size\_mm|
| &#128270;  | ClusteredIndex | ON tile\_width\_mm|
| &#128270;  | ClusteredIndex | ON tiles\_per\_box|
| &#128270;  | ClusteredIndex | ON tiles|
| &#128270;  | ClusteredIndex | ON total\_area\_m2|
| &#128270;  | ClusteredIndex | ON total\_tile\_quantity|
| &#128270;  | ClusteredIndex | ON tube\_centres\_m|
| &#128270;  | ClusteredIndex | ON tube\_diameter|
| &#128270;  | ClusteredIndex | ON uom\_n\_only|
| &#128270;  | ClusteredIndex | ON width|
| &#128270;  | ClusteredIndex | ON estimating\_product\_description|
| &#128270;  | ClusteredIndex | ON grid\_type|
| &#128270;  | ClusteredIndex | ON item\_l\_f|
| &#128270;  | ClusteredIndex | ON item\_l\_m|
| &#128270;  | ClusteredIndex | ON item\_sqft|
| &#128270;  | ClusteredIndex | ON item\_sqm|
| &#128270;  | ClusteredIndex | ON lf|
| &#128270;  | ClusteredIndex | ON lm|
| &#128270;  | ClusteredIndex | ON length\_inches|
| &#128270;  | ClusteredIndex | ON line\_l\_f|
| &#128270;  | ClusteredIndex | ON line\_l\_m|
| &#128270;  | ClusteredIndex | ON line\_sqft|
| &#128270;  | ClusteredIndex | ON line\_sqm|
| &#128270;  | ClusteredIndex | ON product\_image|
| &#128270;  | ClusteredIndex | ON risk\_level\_formula|
| &#128270;  | ClusteredIndex | ON risk|
| &#128270;  | ClusteredIndex | ON sqft|
| &#128270;  | ClusteredIndex | ON sqm|
| &#128270;  | ClusteredIndex | ON unit\_ft|
| &#128270;  | ClusteredIndex | ON unit\_m|
| &#128270;  | ClusteredIndex | ON width\_inches|
| &#128270;  | ClusteredIndex | ON product\_name\_formula|
| &#128270;  | ClusteredIndex | ON costing\_method|
| &#128270;  | ClusteredIndex | ON uom\_ea\_only|
| &#128270;  | ClusteredIndex | ON unit\_cost\_gbp|
| &#128270;  | ClusteredIndex | ON complexity|
| &#128270;  | ClusteredIndex | ON quote\_discount|
| &#128270;  | ClusteredIndex | ON price\_excluded|
| &#128270;  | ClusteredIndex | ON measurement\_type|
| &#128270;  | ClusteredIndex | ON length\_ft|
| &#128270;  | ClusteredIndex | ON length\_inch|
| &#128270;  | ClusteredIndex | ON width\_ft|
| &#128270;  | ClusteredIndex | ON width\_inch|
| &#128270;  | ClusteredIndex | ON clip\_finish|
| &#128270;  | ClusteredIndex | ON manufacture\_source|
| &#128270;  | ClusteredIndex | ON source\_reason|
| &#128270;  | ClusteredIndex | ON item\_cost|
| &#128270;  | ClusteredIndex | ON line\_cost|
| &#128270;  | ClusteredIndex | ON costed\_item\_number|
| &#128270;  | ClusteredIndex | ON total\_cost\_4\_r|
| &#128270;  | ClusteredIndex | ON product\_name\_4\_r|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table freshservice_staging.surveys 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | question| varchar(8000)  |
| &#128270; | choice| float(53)  |
| &#128270; | question\_score| float(53)  |
| &#128270; | maximum\_score| float(53)  |
| &#128270; | associated\_ticket\_id| varchar(8000)  |
| &#128270; | response\_time| varchar(8000)  |
| &#128270; | survey\_name| varchar(8000)  |
| &#128270; | short\_text\_response| varchar(8000)  |
| &#128270; | multi\_select\_choice| float(53)  |
| &#128270; | workspace| varchar(8000)  |
| &#128270; | associated\_agent\_group\_name| varchar(8000)  |
| &#128270; | associated\_requester\_primary\_email| varchar(8000)  |
| &#128270; | question\_type| varchar(8000)  |
| &#128270; | nps\_rating\_group| float(53)  |
| &#128270; | nps\_rating| float(53)  |
| &#128270; | channel| varchar(8000)  |
| &#128270; | associated\_ticket\_urgency| varchar(8000)  |
| &#128270; | associated\_ticket\_impact| varchar(8000)  |
| &#128270; | associated\_ticket\_subject| varchar(8000)  |
| &#128270; | associated\_ticket\_source| varchar(8000)  |
| &#128270; | associated\_ticket\_created\_date| datetime2(26)  |
| &#128270; | associated\_ticket\_issue\_type| varchar(8000)  |
| &#128270; | associated\_ticket\_priority| varchar(8000)  |
| &#128270; | associated\_ticket\_associated\_assets\_count| bigint  |
| &#128270; | associated\_ticket\_resolved\_date| datetime2(26)  |
| &#128270; | associated\_ticket\_closed\_date| datetime2(26)  |
| &#128270; | associated\_ticket\_top\_three| bit  |
| &#128270; | associated\_ticket\_status| varchar(8000)  |
| &#128270; | associated\_ticket\_survey\_score| float(53)  |
| &#128270; | associated\_ticket\_maximum\_survey\_score| float(53)  |
| &#128270; | associated\_ticket\_survey\_response\_time| varchar(8000)  |
| &#128270; | associated\_ticket\_survey\_sent| varchar(8000)  |
| &#128270; | associated\_ticket\_agent\_name| varchar(8000)  |
| &#128270; | associated\_ticket\_agent\_group\_name| varchar(8000)  |
| &#128270; | associated\_ticket\_requester\_name| varchar(8000)  |
| &#128270; | associated\_department\_name| varchar(8000)  |
| &#128270; | associated\_agent\_name| varchar(8000)  |
| &#128270; | associated\_requester\_name| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON question|
| &#128270;  | ClusteredIndex | ON choice|
| &#128270;  | ClusteredIndex | ON question\_score|
| &#128270;  | ClusteredIndex | ON maximum\_score|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_id|
| &#128270;  | ClusteredIndex | ON response\_time|
| &#128270;  | ClusteredIndex | ON survey\_name|
| &#128270;  | ClusteredIndex | ON short\_text\_response|
| &#128270;  | ClusteredIndex | ON multi\_select\_choice|
| &#128270;  | ClusteredIndex | ON workspace|
| &#128270;  | ClusteredIndex | ON associated\_agent\_group\_name|
| &#128270;  | ClusteredIndex | ON associated\_requester\_primary\_email|
| &#128270;  | ClusteredIndex | ON question\_type|
| &#128270;  | ClusteredIndex | ON nps\_rating\_group|
| &#128270;  | ClusteredIndex | ON nps\_rating|
| &#128270;  | ClusteredIndex | ON channel|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_urgency|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_impact|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_subject|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_source|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_created\_date|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_issue\_type|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_priority|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_associated\_assets\_count|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_resolved\_date|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_closed\_date|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_top\_three|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_status|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_survey\_score|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_maximum\_survey\_score|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_survey\_response\_time|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_survey\_sent|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_agent\_name|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_agent\_group\_name|
| &#128270;  | ClusteredIndex | ON associated\_ticket\_requester\_name|
| &#128270;  | ClusteredIndex | ON associated\_department\_name|
| &#128270;  | ClusteredIndex | ON associated\_agent\_name|
| &#128270;  | ClusteredIndex | ON associated\_requester\_name|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table freshservice_staging.tickets 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | subject| varchar(8000)  |
| &#128270; | status| varchar(8000)  |
| &#128270; | priority| varchar(8000)  |
| &#128270; | source| varchar(8000)  |
| &#128270; | last\_updated\_date| varchar(8000)  |
| &#128270; | urgency| varchar(8000)  |
| &#128270; | first\_response\_date| varchar(8000)  |
| &#128270; | impact| varchar(8000)  |
| &#128270; | category| varchar(8000)  |
| &#128270; | assigned\_date| varchar(8000)  |
| &#128270; | resolution\_time\_in\_bhrs| varchar(8000)  |
| &#128270; | type| varchar(8000)  |
| &#128270; | avg\_response\_time\_in\_bhrs| varchar(8000)  |
| &#128270; | created\_date| varchar(8000)  |
| &#128270; | avg\_response\_time| varchar(8000)  |
| &#128270; | first\_response\_status| varchar(8000)  |
| &#128270; | first\_response\_time\_in\_bhrs| varchar(8000)  |
| &#128270; | associated\_assets\_count| varchar(8000)  |
| &#128270; | resolved\_date| varchar(8000)  |
| &#128270; | closed\_date| varchar(8000)  |
| &#128270; | resolution\_status| varchar(8000)  |
| &#128270; | service\_item| varchar(8000)  |
| &#128270; | service\_category| varchar(8000)  |
| &#128270; | agent\_name| varchar(8000)  |
| &#128270; | requester\_primary\_email| varchar(8000)  |
| &#128270; | department\_name| varchar(8000)  |
| &#128270; | requester\_address| varchar(8000)  |
| &#128270; | requested\_for\_name| varchar(8000)  |
| &#128270; | created\_by\_name| varchar(8000)  |
| &#128270; | created\_by\_created\_date| varchar(8000)  |
| &#128270; | associated\_assets\_product| varchar(8000)  |
| &#128270; | associated\_assets\_asset\_name| varchar(8000)  |
| &#128270; | associated\_assets\_warranty\_expiry\_date| varchar(8000)  |
| &#128270; | associated\_assets\_created\_by| varchar(8000)  |
| &#128270; | associated\_assets\_created\_date| varchar(8000)  |
| &#128270; | associated\_assets\_location| varchar(8000)  |
| &#128270; | associated\_assets\_used\_by\_primary\_email| varchar(8000)  |
| &#128270; | associated\_assets\_usage\_type| varchar(8000)  |
| &#128270; | resolution\_note| varchar(8000)  |
| &#128270; | agent\_group\_name| varchar(8000)  |
| &#128270; | requester\_name| varchar(8000)  |
| &#128270; | alert\_severity| varchar(8000)  |
| &#128270; | alert\_alert\_id| varchar(8000)  |
| &#128270; | alert\_id| float(53)  |
| &#128270; | alert\_resource| varchar(8000)  |
| &#128270; | alert\_status| varchar(8000)  |
| &#128270; | alert\_occurrence\_time| varchar(8000)  |
| &#128270; | alert\_alert\_source| varchar(8000)  |
| &#128270; | alert\_metric\_name| varchar(8000)  |
| &#128270; | alert\_metric\_value| varchar(8000)  |
| &#128270; | alert\_node| varchar(8000)  |
| &#128270; | alert\_alert\_profile\_name| varchar(8000)  |
| &#128270; | alert\_integration\_name| varchar(8000)  |
| &#128270; | alert\_workspace| varchar(8000)  |
| &#128270; | alert\_subject| varchar(8000)  |
| &#128270; | requester\_location| varchar(8000)  |
| &#128270; | top\_three| varchar(8000)  |
| &#128270; | survey\_score| varchar(8000)  |
| &#128270; | requested\_for\_primary\_email| varchar(8000)  |
| &#128270; | \_ingestion\_unit| varchar(8000)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON subject|
| &#128270;  | ClusteredIndex | ON status|
| &#128270;  | ClusteredIndex | ON priority|
| &#128270;  | ClusteredIndex | ON source|
| &#128270;  | ClusteredIndex | ON last\_updated\_date|
| &#128270;  | ClusteredIndex | ON urgency|
| &#128270;  | ClusteredIndex | ON first\_response\_date|
| &#128270;  | ClusteredIndex | ON impact|
| &#128270;  | ClusteredIndex | ON category|
| &#128270;  | ClusteredIndex | ON assigned\_date|
| &#128270;  | ClusteredIndex | ON resolution\_time\_in\_bhrs|
| &#128270;  | ClusteredIndex | ON type|
| &#128270;  | ClusteredIndex | ON avg\_response\_time\_in\_bhrs|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON avg\_response\_time|
| &#128270;  | ClusteredIndex | ON first\_response\_status|
| &#128270;  | ClusteredIndex | ON first\_response\_time\_in\_bhrs|
| &#128270;  | ClusteredIndex | ON associated\_assets\_count|
| &#128270;  | ClusteredIndex | ON resolved\_date|
| &#128270;  | ClusteredIndex | ON closed\_date|
| &#128270;  | ClusteredIndex | ON resolution\_status|
| &#128270;  | ClusteredIndex | ON service\_item|
| &#128270;  | ClusteredIndex | ON service\_category|
| &#128270;  | ClusteredIndex | ON agent\_name|
| &#128270;  | ClusteredIndex | ON requester\_primary\_email|
| &#128270;  | ClusteredIndex | ON department\_name|
| &#128270;  | ClusteredIndex | ON requester\_address|
| &#128270;  | ClusteredIndex | ON requested\_for\_name|
| &#128270;  | ClusteredIndex | ON created\_by\_name|
| &#128270;  | ClusteredIndex | ON created\_by\_created\_date|
| &#128270;  | ClusteredIndex | ON associated\_assets\_product|
| &#128270;  | ClusteredIndex | ON associated\_assets\_asset\_name|
| &#128270;  | ClusteredIndex | ON associated\_assets\_warranty\_expiry\_date|
| &#128270;  | ClusteredIndex | ON associated\_assets\_created\_by|
| &#128270;  | ClusteredIndex | ON associated\_assets\_created\_date|
| &#128270;  | ClusteredIndex | ON associated\_assets\_location|
| &#128270;  | ClusteredIndex | ON associated\_assets\_used\_by\_primary\_email|
| &#128270;  | ClusteredIndex | ON associated\_assets\_usage\_type|
| &#128270;  | ClusteredIndex | ON resolution\_note|
| &#128270;  | ClusteredIndex | ON agent\_group\_name|
| &#128270;  | ClusteredIndex | ON requester\_name|
| &#128270;  | ClusteredIndex | ON alert\_severity|
| &#128270;  | ClusteredIndex | ON alert\_alert\_id|
| &#128270;  | ClusteredIndex | ON alert\_id|
| &#128270;  | ClusteredIndex | ON alert\_resource|
| &#128270;  | ClusteredIndex | ON alert\_status|
| &#128270;  | ClusteredIndex | ON alert\_occurrence\_time|
| &#128270;  | ClusteredIndex | ON alert\_alert\_source|
| &#128270;  | ClusteredIndex | ON alert\_metric\_name|
| &#128270;  | ClusteredIndex | ON alert\_metric\_value|
| &#128270;  | ClusteredIndex | ON alert\_node|
| &#128270;  | ClusteredIndex | ON alert\_alert\_profile\_name|
| &#128270;  | ClusteredIndex | ON alert\_integration\_name|
| &#128270;  | ClusteredIndex | ON alert\_workspace|
| &#128270;  | ClusteredIndex | ON alert\_subject|
| &#128270;  | ClusteredIndex | ON requester\_location|
| &#128270;  | ClusteredIndex | ON top\_three|
| &#128270;  | ClusteredIndex | ON survey\_score|
| &#128270;  | ClusteredIndex | ON requested\_for\_primary\_email|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint.tp_be 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | tp\_actual\_bridgend| float(53)  |
| &#128270; | bridgend\_gas\_kwh| float(53)  |
| &#128270; | conversion\_factor\_gas| float(53)  |
| &#128270; | co2e\_gas| float(53)  |
| &#128270; | bridgend\_electricity\_kwh| float(53)  |
| &#128270; | conversion\_factor\_electricity| float(53)  |
| &#128270; | co2e\_electricity| float(53)  |
| &#128270; | co2e\_total| float(53)  |
| &#128270; | intensity\_total| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON tp\_actual\_bridgend|
| &#128270;  | ClusteredIndex | ON bridgend\_gas\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_gas|
| &#128270;  | ClusteredIndex | ON co2e\_gas|
| &#128270;  | ClusteredIndex | ON bridgend\_electricity\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_total|
| &#128270;  | ClusteredIndex | ON intensity\_total|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint_staging.tp_be 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | tp\_actual\_bridgend| float(53)  |
| &#128270; | bridgend\_gas\_kwh| float(53)  |
| &#128270; | conversion\_factor\_gas| float(53)  |
| &#128270; | co2e\_gas| float(53)  |
| &#128270; | bridgend\_electricity\_kwh| float(53)  |
| &#128270; | conversion\_factor\_electricity| float(53)  |
| &#128270; | co2e\_electricity| float(53)  |
| &#128270; | co2e\_total| float(53)  |
| &#128270; | intensity\_total| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON tp\_actual\_bridgend|
| &#128270;  | ClusteredIndex | ON bridgend\_gas\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_gas|
| &#128270;  | ClusteredIndex | ON co2e\_gas|
| &#128270;  | ClusteredIndex | ON bridgend\_electricity\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_total|
| &#128270;  | ClusteredIndex | ON intensity\_total|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table sharepoint.tp_mb 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | tp\_actual\_maybole| float(53)  |
| &#128270; | maybole\_gas\_kwh| float(53)  |
| &#128270; | conversion\_factor\_gas| float(53)  |
| &#128270; | co2e\_gas| float(53)  |
| &#128270; | maybole\_electricity\_kwh| float(53)  |
| &#128270; | conversion\_factor\_electricity| float(53)  |
| &#128270; | co2e\_electricity| float(53)  |
| &#128270; | co2e\_total| float(53)  |
| &#128270; | intensity\_total| float(53)  |
| &#128270; | unnamed\_10| varchar(8000)  |
| &#128270; | m3| float(53)  |
| &#128270; | correction\_factor| float(53)  |
| &#128270; | correction\_factor\_1| float(53)  |
| &#128270; | calorific\_value| float(53)  |
| &#128270; | kwh| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON tp\_actual\_maybole|
| &#128270;  | ClusteredIndex | ON maybole\_gas\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_gas|
| &#128270;  | ClusteredIndex | ON co2e\_gas|
| &#128270;  | ClusteredIndex | ON maybole\_electricity\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_total|
| &#128270;  | ClusteredIndex | ON intensity\_total|
| &#128270;  | ClusteredIndex | ON unnamed\_10|
| &#128270;  | ClusteredIndex | ON m3|
| &#128270;  | ClusteredIndex | ON correction\_factor|
| &#128270;  | ClusteredIndex | ON correction\_factor\_1|
| &#128270;  | ClusteredIndex | ON calorific\_value|
| &#128270;  | ClusteredIndex | ON kwh|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|



### Table sharepoint_staging.tp_mb 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | week\_no| int  |
| &#128270; | tp\_actual\_maybole| float(53)  |
| &#128270; | maybole\_gas\_kwh| float(53)  |
| &#128270; | conversion\_factor\_gas| float(53)  |
| &#128270; | co2e\_gas| float(53)  |
| &#128270; | maybole\_electricity\_kwh| float(53)  |
| &#128270; | conversion\_factor\_electricity| float(53)  |
| &#128270; | co2e\_electricity| float(53)  |
| &#128270; | co2e\_total| float(53)  |
| &#128270; | intensity\_total| float(53)  |
| &#128270; | unnamed\_10| varchar(8000)  |
| &#128270; | m3| float(53)  |
| &#128270; | correction\_factor| float(53)  |
| &#128270; | correction\_factor\_1| float(53)  |
| &#128270; | calorific\_value| float(53)  |
| &#128270; | kwh| float(53)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON week\_no|
| &#128270;  | ClusteredIndex | ON tp\_actual\_maybole|
| &#128270;  | ClusteredIndex | ON maybole\_gas\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_gas|
| &#128270;  | ClusteredIndex | ON co2e\_gas|
| &#128270;  | ClusteredIndex | ON maybole\_electricity\_kwh|
| &#128270;  | ClusteredIndex | ON conversion\_factor\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_electricity|
| &#128270;  | ClusteredIndex | ON co2e\_total|
| &#128270;  | ClusteredIndex | ON intensity\_total|
| &#128270;  | ClusteredIndex | ON unnamed\_10|
| &#128270;  | ClusteredIndex | ON m3|
| &#128270;  | ClusteredIndex | ON correction\_factor|
| &#128270;  | ClusteredIndex | ON correction\_factor\_1|
| &#128270;  | ClusteredIndex | ON calorific\_value|
| &#128270;  | ClusteredIndex | ON kwh|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table salesforce_staging.user 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | id| varchar(8000)  |
| &#128270; | username| varchar(8000)  |
| &#128270; | last\_name| varchar(8000)  |
| &#128270; | first\_name| varchar(8000)  |
| &#128270; | middle\_name| varchar(8000)  |
| &#128270; | suffix| varchar(8000)  |
| &#128270; | name| varchar(8000)  |
| &#128270; | company\_name| varchar(8000)  |
| &#128270; | division| varchar(8000)  |
| &#128270; | department| varchar(8000)  |
| &#128270; | title| varchar(8000)  |
| &#128270; | street| varchar(8000)  |
| &#128270; | city| varchar(8000)  |
| &#128270; | state| varchar(8000)  |
| &#128270; | postal\_code| varchar(8000)  |
| &#128270; | country| varchar(8000)  |
| &#128270; | state\_code| varchar(8000)  |
| &#128270; | country\_code| varchar(8000)  |
| &#128270; | latitude| decimal(38,18)  |
| &#128270; | longitude| decimal(38,18)  |
| &#128270; | geocode\_accuracy| varchar(8000)  |
| &#128270; | email| varchar(8000)  |
| &#128270; | email\_preferences\_auto\_bcc| bit  |
| &#128270; | email\_preferences\_auto\_bcc\_stay\_in\_touch| bit  |
| &#128270; | email\_preferences\_stay\_in\_touch\_reminder| bit  |
| &#128270; | sender\_email| varchar(8000)  |
| &#128270; | sender\_name| varchar(8000)  |
| &#128270; | signature| varchar(8000)  |
| &#128270; | stay\_in\_touch\_subject| varchar(8000)  |
| &#128270; | stay\_in\_touch\_signature| varchar(8000)  |
| &#128270; | stay\_in\_touch\_note| varchar(8000)  |
| &#128270; | phone| varchar(8000)  |
| &#128270; | fax| varchar(8000)  |
| &#128270; | mobile\_phone| varchar(8000)  |
| &#128270; | alias| varchar(8000)  |
| &#128270; | community\_nickname| varchar(8000)  |
| &#128270; | badge\_text| varchar(8000)  |
| &#128270; | is\_active| bit  |
| &#128270; | time\_zone\_sid\_key| varchar(8000)  |
| &#128270; | user\_role\_id| varchar(8000)  |
| &#128270; | locale\_sid\_key| varchar(8000)  |
| &#128270; | receives\_info\_emails| bit  |
| &#128270; | receives\_admin\_info\_emails| bit  |
| &#128270; | email\_encoding\_key| varchar(8000)  |
| &#128270; | default\_currency\_iso\_code| varchar(8000)  |
| &#128270; | currency\_iso\_code| varchar(8000)  |
| &#128270; | profile\_id| varchar(8000)  |
| &#128270; | user\_type| varchar(8000)  |
| &#128270; | start\_day| varchar(8000)  |
| &#128270; | end\_day| varchar(8000)  |
| &#128270; | language\_locale\_key| varchar(8000)  |
| &#128270; | employee\_number| varchar(8000)  |
| &#128270; | delegated\_approver\_id| varchar(8000)  |
| &#128270; | manager\_id| varchar(8000)  |
| &#128270; | last\_password\_change\_date| datetime2(26)  |
| &#128270; | created\_date| datetime2(26)  |
| &#128270; | created\_by\_id| varchar(8000)  |
| &#128270; | last\_modified\_date| datetime2(26)  |
| &#128270; | last\_modified\_by\_id| varchar(8000)  |
| &#128270; | system\_modstamp| datetime2(26)  |
| &#128270; | password\_expiration\_date| datetime2(26)  |
| &#128270; | number\_of\_failed\_logins| int  |
| &#128270; | su\_access\_expiration\_date| datetime2(26)  |
| &#128270; | offline\_trial\_expiration\_date| datetime2(26)  |
| &#128270; | offline\_pda\_trial\_expiration\_date| datetime2(26)  |
| &#128270; | user\_permissions\_marketing\_user| bit  |
| &#128270; | user\_permissions\_offline\_user| bit  |
| &#128270; | user\_permissions\_avantgo\_user| bit  |
| &#128270; | user\_permissions\_call\_center\_auto\_login| bit  |
| &#128270; | user\_permissions\_sf\_content\_user| bit  |
| &#128270; | user\_permissions\_knowledge\_user| bit  |
| &#128270; | user\_permissions\_interaction\_user| bit  |
| &#128270; | user\_permissions\_support\_user| bit  |
| &#128270; | forecast\_enabled| bit  |
| &#128270; | user\_preferences\_activity\_reminders\_popup| bit  |
| &#128270; | user\_preferences\_event\_reminders\_checkbox\_default| bit  |
| &#128270; | user\_preferences\_task\_reminders\_checkbox\_default| bit  |
| &#128270; | user\_preferences\_reminder\_sound\_off| bit  |
| &#128270; | user\_preferences\_disable\_all\_feeds\_email| bit  |
| &#128270; | user\_preferences\_disable\_followers\_email| bit  |
| &#128270; | user\_preferences\_disable\_profile\_post\_email| bit  |
| &#128270; | user\_preferences\_disable\_change\_comment\_email| bit  |
| &#128270; | user\_preferences\_disable\_later\_comment\_email| bit  |
| &#128270; | user\_preferences\_dis\_prof\_post\_comment\_email| bit  |
| &#128270; | user\_preferences\_apex\_pages\_developer\_mode| bit  |
| &#128270; | user\_preferences\_receive\_no\_notifications\_as\_approver| bit  |
| &#128270; | user\_preferences\_receive\_notifications\_as\_delegated\_approver| bit  |
| &#128270; | user\_preferences\_hide\_csn\_get\_chatter\_mobile\_task| bit  |
| &#128270; | user\_preferences\_disable\_mentions\_post\_email| bit  |
| &#128270; | user\_preferences\_dis\_mentions\_comment\_email| bit  |
| &#128270; | user\_preferences\_hide\_csn\_desktop\_task| bit  |
| &#128270; | user\_preferences\_hide\_chatter\_onboarding\_splash| bit  |
| &#128270; | user\_preferences\_hide\_second\_chatter\_onboarding\_splash| bit  |
| &#128270; | user\_preferences\_dis\_comment\_after\_like\_email| bit  |
| &#128270; | user\_preferences\_disable\_like\_email| bit  |
| &#128270; | user\_preferences\_sort\_feed\_by\_comment| bit  |
| &#128270; | user\_preferences\_disable\_message\_email| bit  |
| &#128270; | user\_preferences\_disable\_bookmark\_email| bit  |
| &#128270; | user\_preferences\_disable\_share\_post\_email| bit  |
| &#128270; | user\_preferences\_enable\_auto\_sub\_for\_feeds| bit  |
| &#128270; | user\_preferences\_disable\_file\_share\_notifications\_for\_api| bit  |
| &#128270; | user\_preferences\_show\_title\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_manager\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_email\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_work\_phone\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_mobile\_phone\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_fax\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_street\_address\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_city\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_state\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_postal\_code\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_country\_to\_external\_users| bit  |
| &#128270; | user\_preferences\_show\_profile\_pic\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_title\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_city\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_state\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_postal\_code\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_country\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_hide\_s1\_browser\_ui| bit  |
| &#128270; | user\_preferences\_disable\_endorsement\_email| bit  |
| &#128270; | user\_preferences\_path\_assistant\_collapsed| bit  |
| &#128270; | user\_preferences\_cache\_diagnostics| bit  |
| &#128270; | user\_preferences\_show\_email\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_manager\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_work\_phone\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_mobile\_phone\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_fax\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_show\_street\_address\_to\_guest\_users| bit  |
| &#128270; | user\_preferences\_lightning\_experience\_preferred| bit  |
| &#128270; | user\_preferences\_preview\_lightning| bit  |
| &#128270; | user\_preferences\_hide\_end\_user\_onboarding\_assistant\_modal| bit  |
| &#128270; | user\_preferences\_hide\_lightning\_migration\_modal| bit  |
| &#128270; | user\_preferences\_hide\_sfx\_welcome\_mat| bit  |
| &#128270; | user\_preferences\_hide\_bigger\_photo\_callout| bit  |
| &#128270; | user\_preferences\_global\_nav\_bar\_wt\_shown| bit  |
| &#128270; | user\_preferences\_global\_nav\_grid\_menu\_wt\_shown| bit  |
| &#128270; | user\_preferences\_create\_lex\_apps\_wt\_shown| bit  |
| &#128270; | user\_preferences\_favorites\_wt\_shown| bit  |
| &#128270; | user\_preferences\_record\_home\_section\_collapse\_wt\_shown| bit  |
| &#128270; | user\_preferences\_record\_home\_reserved\_wt\_shown| bit  |
| &#128270; | user\_preferences\_favorites\_show\_top\_favorites| bit  |
| &#128270; | user\_preferences\_exclude\_mail\_app\_attachments| bit  |
| &#128270; | user\_preferences\_suppress\_task\_sfx\_reminders| bit  |
| &#128270; | user\_preferences\_suppress\_event\_sfx\_reminders| bit  |
| &#128270; | user\_preferences\_preview\_custom\_theme| bit  |
| &#128270; | user\_preferences\_has\_celebration\_badge| bit  |
| &#128270; | user\_preferences\_user\_debug\_mode\_pref| bit  |
| &#128270; | user\_preferences\_srh\_override\_activities| bit  |
| &#128270; | user\_preferences\_new\_lightning\_report\_run\_page\_enabled| bit  |
| &#128270; | user\_preferences\_native\_email\_client| bit  |
| &#128270; | contact\_id| varchar(8000)  |
| &#128270; | account\_id| varchar(8000)  |
| &#128270; | call\_center\_id| varchar(8000)  |
| &#128270; | extension| varchar(8000)  |
| &#128270; | portal\_role| varchar(8000)  |
| &#128270; | is\_portal\_enabled| bit  |
| &#128270; | federation\_identifier| varchar(8000)  |
| &#128270; | about\_me| varchar(8000)  |
| &#128270; | full\_photo\_url| varchar(8000)  |
| &#128270; | small\_photo\_url| varchar(8000)  |
| &#128270; | is\_ext\_indicator\_visible| bit  |
| &#128270; | out\_of\_office\_message| varchar(8000)  |
| &#128270; | medium\_photo\_url| varchar(8000)  |
| &#128270; | digest\_frequency| varchar(8000)  |
| &#128270; | default\_group\_notification\_frequency| varchar(8000)  |
| &#128270; | last\_viewed\_date| datetime2(26)  |
| &#128270; | last\_referenced\_date| datetime2(26)  |
| &#128270; | banner\_photo\_url| varchar(8000)  |
| &#128270; | small\_banner\_photo\_url| varchar(8000)  |
| &#128270; | medium\_banner\_photo\_url| varchar(8000)  |
| &#128270; | is\_profile\_photo\_active| bit  |
| &#128270; | individual\_id| varchar(8000)  |
| &#128270; | dashboard\_pal\_\_default\_dashboard| varchar(8000)  |
| &#128270; | pi\_\_can\_view\_not\_assigned\_prospects| bit  |
| &#128270; | pi\_\_pardot\_api\_version| varchar(8000)  |
| &#128270; | pi\_\_pardot\_user\_role| varchar(8000)  |
| &#128270; | currency\_code| varchar(8000)  |
| &#128270; | profile\_name| varchar(8000)  |
| &#128270; | sas\_by\_pass\_validation\_rules| bit  |
| &#128270; | sales\_division| varchar(8000)  |
| &#128270; | sales\_support| varchar(8000)  |
| &#128270; | infor\_ref| varchar(8000)  |
| &#128270; | mock\_up\_sign\_off| bit  |
| &#128270; | sbqq\_\_default\_product\_lookup\_tab| varchar(8000)  |
| &#128270; | last\_login\_date| datetime2(26)  |
| &#128270; | sbqq\_\_diagnostic\_tool\_enabled| bit  |
| &#128270; | sbqq\_\_output\_format\_change\_allowed| bit  |
| &#128270; | sbqq\_\_product\_sort\_preference| varchar(8000)  |
| &#128270; | sbqq\_\_reset\_product\_lookup| bit  |
| &#128270; | sbqq\_\_theme| varchar(8000)  |
| &#128270; | estimating\_approval\_level| varchar(8000)  |
| &#128270; | estimating| bit  |
| &#128270; | infor\_processed\_by| varchar(8000)  |
| &#128270; | full\_name| varchar(8000)  |
| &#128270; | sales\_team| varchar(8000)  |
| &#128270; | timesheet\_rate| decimal(38,18)  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON id|
| &#128270;  | ClusteredIndex | ON username|
| &#128270;  | ClusteredIndex | ON last\_name|
| &#128270;  | ClusteredIndex | ON first\_name|
| &#128270;  | ClusteredIndex | ON middle\_name|
| &#128270;  | ClusteredIndex | ON suffix|
| &#128270;  | ClusteredIndex | ON name|
| &#128270;  | ClusteredIndex | ON company\_name|
| &#128270;  | ClusteredIndex | ON division|
| &#128270;  | ClusteredIndex | ON department|
| &#128270;  | ClusteredIndex | ON title|
| &#128270;  | ClusteredIndex | ON street|
| &#128270;  | ClusteredIndex | ON city|
| &#128270;  | ClusteredIndex | ON state|
| &#128270;  | ClusteredIndex | ON postal\_code|
| &#128270;  | ClusteredIndex | ON country|
| &#128270;  | ClusteredIndex | ON state\_code|
| &#128270;  | ClusteredIndex | ON country\_code|
| &#128270;  | ClusteredIndex | ON latitude|
| &#128270;  | ClusteredIndex | ON longitude|
| &#128270;  | ClusteredIndex | ON geocode\_accuracy|
| &#128270;  | ClusteredIndex | ON email|
| &#128270;  | ClusteredIndex | ON email\_preferences\_auto\_bcc|
| &#128270;  | ClusteredIndex | ON email\_preferences\_auto\_bcc\_stay\_in\_touch|
| &#128270;  | ClusteredIndex | ON email\_preferences\_stay\_in\_touch\_reminder|
| &#128270;  | ClusteredIndex | ON sender\_email|
| &#128270;  | ClusteredIndex | ON sender\_name|
| &#128270;  | ClusteredIndex | ON signature|
| &#128270;  | ClusteredIndex | ON stay\_in\_touch\_subject|
| &#128270;  | ClusteredIndex | ON stay\_in\_touch\_signature|
| &#128270;  | ClusteredIndex | ON stay\_in\_touch\_note|
| &#128270;  | ClusteredIndex | ON phone|
| &#128270;  | ClusteredIndex | ON fax|
| &#128270;  | ClusteredIndex | ON mobile\_phone|
| &#128270;  | ClusteredIndex | ON alias|
| &#128270;  | ClusteredIndex | ON community\_nickname|
| &#128270;  | ClusteredIndex | ON badge\_text|
| &#128270;  | ClusteredIndex | ON is\_active|
| &#128270;  | ClusteredIndex | ON time\_zone\_sid\_key|
| &#128270;  | ClusteredIndex | ON user\_role\_id|
| &#128270;  | ClusteredIndex | ON locale\_sid\_key|
| &#128270;  | ClusteredIndex | ON receives\_info\_emails|
| &#128270;  | ClusteredIndex | ON receives\_admin\_info\_emails|
| &#128270;  | ClusteredIndex | ON email\_encoding\_key|
| &#128270;  | ClusteredIndex | ON default\_currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON currency\_iso\_code|
| &#128270;  | ClusteredIndex | ON profile\_id|
| &#128270;  | ClusteredIndex | ON user\_type|
| &#128270;  | ClusteredIndex | ON start\_day|
| &#128270;  | ClusteredIndex | ON end\_day|
| &#128270;  | ClusteredIndex | ON language\_locale\_key|
| &#128270;  | ClusteredIndex | ON employee\_number|
| &#128270;  | ClusteredIndex | ON delegated\_approver\_id|
| &#128270;  | ClusteredIndex | ON manager\_id|
| &#128270;  | ClusteredIndex | ON last\_password\_change\_date|
| &#128270;  | ClusteredIndex | ON created\_date|
| &#128270;  | ClusteredIndex | ON created\_by\_id|
| &#128270;  | ClusteredIndex | ON last\_modified\_date|
| &#128270;  | ClusteredIndex | ON last\_modified\_by\_id|
| &#128270;  | ClusteredIndex | ON system\_modstamp|
| &#128270;  | ClusteredIndex | ON password\_expiration\_date|
| &#128270;  | ClusteredIndex | ON number\_of\_failed\_logins|
| &#128270;  | ClusteredIndex | ON su\_access\_expiration\_date|
| &#128270;  | ClusteredIndex | ON offline\_trial\_expiration\_date|
| &#128270;  | ClusteredIndex | ON offline\_pda\_trial\_expiration\_date|
| &#128270;  | ClusteredIndex | ON user\_permissions\_marketing\_user|
| &#128270;  | ClusteredIndex | ON user\_permissions\_offline\_user|
| &#128270;  | ClusteredIndex | ON user\_permissions\_avantgo\_user|
| &#128270;  | ClusteredIndex | ON user\_permissions\_call\_center\_auto\_login|
| &#128270;  | ClusteredIndex | ON user\_permissions\_sf\_content\_user|
| &#128270;  | ClusteredIndex | ON user\_permissions\_knowledge\_user|
| &#128270;  | ClusteredIndex | ON user\_permissions\_interaction\_user|
| &#128270;  | ClusteredIndex | ON user\_permissions\_support\_user|
| &#128270;  | ClusteredIndex | ON forecast\_enabled|
| &#128270;  | ClusteredIndex | ON user\_preferences\_activity\_reminders\_popup|
| &#128270;  | ClusteredIndex | ON user\_preferences\_event\_reminders\_checkbox\_default|
| &#128270;  | ClusteredIndex | ON user\_preferences\_task\_reminders\_checkbox\_default|
| &#128270;  | ClusteredIndex | ON user\_preferences\_reminder\_sound\_off|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_all\_feeds\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_followers\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_profile\_post\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_change\_comment\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_later\_comment\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_dis\_prof\_post\_comment\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_apex\_pages\_developer\_mode|
| &#128270;  | ClusteredIndex | ON user\_preferences\_receive\_no\_notifications\_as\_approver|
| &#128270;  | ClusteredIndex | ON user\_preferences\_receive\_notifications\_as\_delegated\_approver|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_csn\_get\_chatter\_mobile\_task|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_mentions\_post\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_dis\_mentions\_comment\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_csn\_desktop\_task|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_chatter\_onboarding\_splash|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_second\_chatter\_onboarding\_splash|
| &#128270;  | ClusteredIndex | ON user\_preferences\_dis\_comment\_after\_like\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_like\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_sort\_feed\_by\_comment|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_message\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_bookmark\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_share\_post\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_enable\_auto\_sub\_for\_feeds|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_file\_share\_notifications\_for\_api|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_title\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_manager\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_email\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_work\_phone\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_mobile\_phone\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_fax\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_street\_address\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_city\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_state\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_postal\_code\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_country\_to\_external\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_profile\_pic\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_title\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_city\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_state\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_postal\_code\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_country\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_s1\_browser\_ui|
| &#128270;  | ClusteredIndex | ON user\_preferences\_disable\_endorsement\_email|
| &#128270;  | ClusteredIndex | ON user\_preferences\_path\_assistant\_collapsed|
| &#128270;  | ClusteredIndex | ON user\_preferences\_cache\_diagnostics|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_email\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_manager\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_work\_phone\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_mobile\_phone\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_fax\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_show\_street\_address\_to\_guest\_users|
| &#128270;  | ClusteredIndex | ON user\_preferences\_lightning\_experience\_preferred|
| &#128270;  | ClusteredIndex | ON user\_preferences\_preview\_lightning|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_end\_user\_onboarding\_assistant\_modal|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_lightning\_migration\_modal|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_sfx\_welcome\_mat|
| &#128270;  | ClusteredIndex | ON user\_preferences\_hide\_bigger\_photo\_callout|
| &#128270;  | ClusteredIndex | ON user\_preferences\_global\_nav\_bar\_wt\_shown|
| &#128270;  | ClusteredIndex | ON user\_preferences\_global\_nav\_grid\_menu\_wt\_shown|
| &#128270;  | ClusteredIndex | ON user\_preferences\_create\_lex\_apps\_wt\_shown|
| &#128270;  | ClusteredIndex | ON user\_preferences\_favorites\_wt\_shown|
| &#128270;  | ClusteredIndex | ON user\_preferences\_record\_home\_section\_collapse\_wt\_shown|
| &#128270;  | ClusteredIndex | ON user\_preferences\_record\_home\_reserved\_wt\_shown|
| &#128270;  | ClusteredIndex | ON user\_preferences\_favorites\_show\_top\_favorites|
| &#128270;  | ClusteredIndex | ON user\_preferences\_exclude\_mail\_app\_attachments|
| &#128270;  | ClusteredIndex | ON user\_preferences\_suppress\_task\_sfx\_reminders|
| &#128270;  | ClusteredIndex | ON user\_preferences\_suppress\_event\_sfx\_reminders|
| &#128270;  | ClusteredIndex | ON user\_preferences\_preview\_custom\_theme|
| &#128270;  | ClusteredIndex | ON user\_preferences\_has\_celebration\_badge|
| &#128270;  | ClusteredIndex | ON user\_preferences\_user\_debug\_mode\_pref|
| &#128270;  | ClusteredIndex | ON user\_preferences\_srh\_override\_activities|
| &#128270;  | ClusteredIndex | ON user\_preferences\_new\_lightning\_report\_run\_page\_enabled|
| &#128270;  | ClusteredIndex | ON user\_preferences\_native\_email\_client|
| &#128270;  | ClusteredIndex | ON contact\_id|
| &#128270;  | ClusteredIndex | ON account\_id|
| &#128270;  | ClusteredIndex | ON call\_center\_id|
| &#128270;  | ClusteredIndex | ON extension|
| &#128270;  | ClusteredIndex | ON portal\_role|
| &#128270;  | ClusteredIndex | ON is\_portal\_enabled|
| &#128270;  | ClusteredIndex | ON federation\_identifier|
| &#128270;  | ClusteredIndex | ON about\_me|
| &#128270;  | ClusteredIndex | ON full\_photo\_url|
| &#128270;  | ClusteredIndex | ON small\_photo\_url|
| &#128270;  | ClusteredIndex | ON is\_ext\_indicator\_visible|
| &#128270;  | ClusteredIndex | ON out\_of\_office\_message|
| &#128270;  | ClusteredIndex | ON medium\_photo\_url|
| &#128270;  | ClusteredIndex | ON digest\_frequency|
| &#128270;  | ClusteredIndex | ON default\_group\_notification\_frequency|
| &#128270;  | ClusteredIndex | ON last\_viewed\_date|
| &#128270;  | ClusteredIndex | ON last\_referenced\_date|
| &#128270;  | ClusteredIndex | ON banner\_photo\_url|
| &#128270;  | ClusteredIndex | ON small\_banner\_photo\_url|
| &#128270;  | ClusteredIndex | ON medium\_banner\_photo\_url|
| &#128270;  | ClusteredIndex | ON is\_profile\_photo\_active|
| &#128270;  | ClusteredIndex | ON individual\_id|
| &#128270;  | ClusteredIndex | ON dashboard\_pal\_\_default\_dashboard|
| &#128270;  | ClusteredIndex | ON pi\_\_can\_view\_not\_assigned\_prospects|
| &#128270;  | ClusteredIndex | ON pi\_\_pardot\_api\_version|
| &#128270;  | ClusteredIndex | ON pi\_\_pardot\_user\_role|
| &#128270;  | ClusteredIndex | ON currency\_code|
| &#128270;  | ClusteredIndex | ON profile\_name|
| &#128270;  | ClusteredIndex | ON sas\_by\_pass\_validation\_rules|
| &#128270;  | ClusteredIndex | ON sales\_division|
| &#128270;  | ClusteredIndex | ON sales\_support|
| &#128270;  | ClusteredIndex | ON infor\_ref|
| &#128270;  | ClusteredIndex | ON mock\_up\_sign\_off|
| &#128270;  | ClusteredIndex | ON sbqq\_\_default\_product\_lookup\_tab|
| &#128270;  | ClusteredIndex | ON last\_login\_date|
| &#128270;  | ClusteredIndex | ON sbqq\_\_diagnostic\_tool\_enabled|
| &#128270;  | ClusteredIndex | ON sbqq\_\_output\_format\_change\_allowed|
| &#128270;  | ClusteredIndex | ON sbqq\_\_product\_sort\_preference|
| &#128270;  | ClusteredIndex | ON sbqq\_\_reset\_product\_lookup|
| &#128270;  | ClusteredIndex | ON sbqq\_\_theme|
| &#128270;  | ClusteredIndex | ON estimating\_approval\_level|
| &#128270;  | ClusteredIndex | ON estimating|
| &#128270;  | ClusteredIndex | ON infor\_processed\_by|
| &#128270;  | ClusteredIndex | ON full\_name|
| &#128270;  | ClusteredIndex | ON sales\_team|
| &#128270;  | ClusteredIndex | ON timesheet\_rate|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|



### Table syteline_staging.vendor_mst 
|Idx |Name |Data Type |
|---|---|---|
| &#128270; | site\_ref| varchar(8000)  |
| &#128270; | vend\_num| varchar(8000)  |
| &#128270; | contact| varchar(8000)  |
| &#128270; | phone| varchar(8000)  |
| &#128270; | vend\_type| varchar(8000)  |
| &#128270; | terms\_code| varchar(8000)  |
| &#128270; | ship\_code| varchar(8000)  |
| &#128270; | fob| varchar(8000)  |
| &#128270; | print\_price| int  |
| &#128270; | stat| varchar(8000)  |
| &#128270; | last\_purch| datetime2(26)  |
| &#128270; | last\_paid| datetime2(26)  |
| &#128270; | purch\_ytd| decimal(23,8)  |
| &#128270; | purch\_lst\_yr| decimal(23,8)  |
| &#128270; | disc\_ytd| decimal(23,8)  |
| &#128270; | disc\_lst\_yr| decimal(23,8)  |
| &#128270; | pay\_ytd| decimal(23,8)  |
| &#128270; | vend\_remit| varchar(8000)  |
| &#128270; | whse| varchar(8000)  |
| &#128270; | charfld1| varchar(8000)  |
| &#128270; | charfld2| varchar(8000)  |
| &#128270; | charfld3| varchar(8000)  |
| &#128270; | decifld1| decimal(10,2)  |
| &#128270; | decifld2| decimal(10,2)  |
| &#128270; | decifld3| decimal(10,2)  |
| &#128270; | logifld| int  |
| &#128270; | datefld| datetime2(26)  |
| &#128270; | curr\_code| varchar(8000)  |
| &#128270; | tax\_reg\_num1| varchar(8000)  |
| &#128270; | bank\_code| varchar(8000)  |
| &#128270; | pay\_type| varchar(8000)  |
| &#128270; | pay\_lst\_yr| decimal(23,8)  |
| &#128270; | edi\_vend| int  |
| &#128270; | branch\_id| varchar(8000)  |
| &#128270; | trans\_nat| varchar(8000)  |
| &#128270; | delterm| varchar(8000)  |
| &#128270; | process\_ind| varchar(8000)  |
| &#128270; | tax\_reg\_num2| varchar(8000)  |
| &#128270; | tax\_code1| varchar(8000)  |
| &#128270; | tax\_code2| varchar(8000)  |
| &#128270; | lang\_code| varchar(8000)  |
| &#128270; | pur\_acct| varchar(8000)  |
| &#128270; | pur\_acct\_unit1| varchar(8000)  |
| &#128270; | pur\_acct\_unit2| varchar(8000)  |
| &#128270; | pur\_acct\_unit3| varchar(8000)  |
| &#128270; | pur\_acct\_unit4| varchar(8000)  |
| &#128270; | lcr\_reqd| int  |
| &#128270; | category| varchar(8000)  |
| &#128270; | note\_exists\_flag| int  |
| &#128270; | record\_date| datetime2(26)  |
| &#128270; | row\_pointer| varchar(8000)  |
| &#128270; | created\_by| varchar(8000)  |
| &#128270; | updated\_by| varchar(8000)  |
| &#128270; | create\_date| datetime2(26)  |
| &#128270; | in\_workflow| int  |
| &#128270; | account| varchar(8000)  |
| &#128270; | account\_name| varchar(8000)  |
| &#128270; | eft\_bank\_num| varchar(8000)  |
| &#128270; | print\_vat\_on\_po| int  |
| &#128270; | price\_by| varchar(8000)  |
| &#128270; | include\_tax\_in\_cost| int  |
| &#128270; | trans\_nat\_2| varchar(8000)  |
| &#128270; | active\_for\_data\_integration| int  |
| &#128270; | vch\_over\_po\_cost\_tolerance| decimal(7,4)  |
| &#128270; | vch\_under\_po\_cost\_tolerance| decimal(7,4)  |
| &#128270; | pay\_fiscal\_ytd| decimal(23,8)  |
| &#128270; | pay\_lst\_fiscal\_yr| decimal(23,8)  |
| &#128270; | supply\_web\_vendor| int  |
| &#128270; | request\_acknowledgement| int  |
| &#128270; | synchronized\_to\_bus| int  |
| &#128270; | show\_in\_drop\_down\_list| int  |
| &#128270; | auto\_voucher| int  |
| &#128270; | auto\_voucher\_method| varchar(8000)  |
| &#128270; | international\_bank\_account| varchar(8000)  |
| &#128270; | buyer| varchar(8000)  |
| &#128270; | deposit\_acct\_type| varchar(8000)  |
| &#128270; | allow\_to\_firm\_plns| int  |
| &#128270; | firm\_pln\_target| varchar(8000)  |
| &#128270; | firmed\_poitem\_stat| varchar(8000)  |
| &#128270; | replen\_po\_num| varchar(8000)  |
| &#128270; | transit\_reference| varchar(8000)  |
| &#128270; | misc1099\_ytd| decimal(23,8)  |
| &#128270; | misc1099\_lst\_yr| decimal(23,8)  |
| &#128270; | source\_site| varchar(8000)  |
| &#128270; | source\_site\_cust\_num| varchar(8000)  |
| &#128270; | auto\_receive\_demanding\_site\_po| int  |
| &#128270; | auto\_ship\_demanding\_site\_co| int  |
| &#128270; | minority\_owned| int  |
| &#128270; | th\_wht\_type| varchar(8000)  |
| &#128270; | mx\_tax\_reg\_num\_type| varchar(8000)  |
| &#128270; | mx\_vendor\_diot\_type| varchar(8000)  |
| &#128270; | tax\_reg\_num1\_exp\_date| datetime2(26)  |
| &#128270; | jp\_eft\_bank\_fee\_terms| int  |
| &#128270; | jp\_bank\_branch\_name| varchar(8000)  |
| &#128270; | jp\_account\_owner\_name| varchar(8000)  |
| &#128270; | jp\_zengin\_bank\_code| decimal(4,0)  |
| &#128270; | jp\_zengin\_branch\_code| decimal(3,0)  |
| &#128270; | jp\_zengin\_acct\_no| decimal(7,0)  |
| &#128270; | jp\_account\_ref\_1| varchar(8000)  |
| &#128270; | jp\_account\_ref\_2| varchar(8000)  |
| &#128270; | cust\_num| varchar(8000)  |
| &#128270; | vend\_bank| varchar(8000)  |
| &#128270; | bank\_file\_format| varchar(8000)  |
| &#128270; | picture| varbinary(8000)  |
| &#128270; | fiscal\_rpt\_system| varchar(8000)  |
| &#128270; | fiscal\_rpt\_system\_type| varchar(8000)  |
| &#128270; | business\_identification\_num| varchar(8000)  |
| &#128270; | profession| varchar(8000)  |
| &#128270; | au\_contract\_price\_method| varchar(8000)  |
| &#128270; | bank\_authority\_party\_id| varchar(8000)  |
| &#128270; | bank\_transit\_num| varchar(8000)  |
| &#128270; | override\_bank\_transit\_num| int  |
| &#128270; | head\_office| int  |
| &#128270; | branch\_name| varchar(8000)  |
| &#128270; | active\_for\_anonymization| int  |
| &#128270; | uf\_company\_reg| varchar(8000)  |
| &#128270; | uf\_ni\_number| varchar(8000)  |
| &#128270; | uf\_partner\_name| varchar(8000)  |
| &#128270; | uf\_tax\_treatment| varchar(8000)  |
| &#128270; | uf\_utr\_no| varchar(8000)  |
| &#128270; | uf\_vn| varchar(8000)  |
| &#128270; | uf\_bank\_address\_details| varchar(8000)  |
| &#128270; | uf\_bank\_int\_code| varchar(8000)  |
| &#128270; | uf\_beneficiary| varchar(8000)  |
| &#128270; | uf\_managed\_by| varchar(8000)  |
| &#128270; | uf\_vend\_qty\_tol| int  |
| &#128270; | \_ingestion\_unit| varchar(500)  |
| &#128270; | \_run\_id| varchar(20)  |
| &#128270; | \_execution\_id| varchar(20)  |
| &#128270; | \_loaded\_at| varchar(33)  |


##### Indexes 
|Type |Name |On |
|---|---|---|
| &#128270;  | ClusteredIndex | ON site\_ref|
| &#128270;  | ClusteredIndex | ON vend\_num|
| &#128270;  | ClusteredIndex | ON contact|
| &#128270;  | ClusteredIndex | ON phone|
| &#128270;  | ClusteredIndex | ON vend\_type|
| &#128270;  | ClusteredIndex | ON terms\_code|
| &#128270;  | ClusteredIndex | ON ship\_code|
| &#128270;  | ClusteredIndex | ON fob|
| &#128270;  | ClusteredIndex | ON print\_price|
| &#128270;  | ClusteredIndex | ON stat|
| &#128270;  | ClusteredIndex | ON last\_purch|
| &#128270;  | ClusteredIndex | ON last\_paid|
| &#128270;  | ClusteredIndex | ON purch\_ytd|
| &#128270;  | ClusteredIndex | ON purch\_lst\_yr|
| &#128270;  | ClusteredIndex | ON disc\_ytd|
| &#128270;  | ClusteredIndex | ON disc\_lst\_yr|
| &#128270;  | ClusteredIndex | ON pay\_ytd|
| &#128270;  | ClusteredIndex | ON vend\_remit|
| &#128270;  | ClusteredIndex | ON whse|
| &#128270;  | ClusteredIndex | ON charfld1|
| &#128270;  | ClusteredIndex | ON charfld2|
| &#128270;  | ClusteredIndex | ON charfld3|
| &#128270;  | ClusteredIndex | ON decifld1|
| &#128270;  | ClusteredIndex | ON decifld2|
| &#128270;  | ClusteredIndex | ON decifld3|
| &#128270;  | ClusteredIndex | ON logifld|
| &#128270;  | ClusteredIndex | ON datefld|
| &#128270;  | ClusteredIndex | ON curr\_code|
| &#128270;  | ClusteredIndex | ON tax\_reg\_num1|
| &#128270;  | ClusteredIndex | ON bank\_code|
| &#128270;  | ClusteredIndex | ON pay\_type|
| &#128270;  | ClusteredIndex | ON pay\_lst\_yr|
| &#128270;  | ClusteredIndex | ON edi\_vend|
| &#128270;  | ClusteredIndex | ON branch\_id|
| &#128270;  | ClusteredIndex | ON trans\_nat|
| &#128270;  | ClusteredIndex | ON delterm|
| &#128270;  | ClusteredIndex | ON process\_ind|
| &#128270;  | ClusteredIndex | ON tax\_reg\_num2|
| &#128270;  | ClusteredIndex | ON tax\_code1|
| &#128270;  | ClusteredIndex | ON tax\_code2|
| &#128270;  | ClusteredIndex | ON lang\_code|
| &#128270;  | ClusteredIndex | ON pur\_acct|
| &#128270;  | ClusteredIndex | ON pur\_acct\_unit1|
| &#128270;  | ClusteredIndex | ON pur\_acct\_unit2|
| &#128270;  | ClusteredIndex | ON pur\_acct\_unit3|
| &#128270;  | ClusteredIndex | ON pur\_acct\_unit4|
| &#128270;  | ClusteredIndex | ON lcr\_reqd|
| &#128270;  | ClusteredIndex | ON category|
| &#128270;  | ClusteredIndex | ON note\_exists\_flag|
| &#128270;  | ClusteredIndex | ON record\_date|
| &#128270;  | ClusteredIndex | ON row\_pointer|
| &#128270;  | ClusteredIndex | ON created\_by|
| &#128270;  | ClusteredIndex | ON updated\_by|
| &#128270;  | ClusteredIndex | ON create\_date|
| &#128270;  | ClusteredIndex | ON in\_workflow|
| &#128270;  | ClusteredIndex | ON account|
| &#128270;  | ClusteredIndex | ON account\_name|
| &#128270;  | ClusteredIndex | ON eft\_bank\_num|
| &#128270;  | ClusteredIndex | ON print\_vat\_on\_po|
| &#128270;  | ClusteredIndex | ON price\_by|
| &#128270;  | ClusteredIndex | ON include\_tax\_in\_cost|
| &#128270;  | ClusteredIndex | ON trans\_nat\_2|
| &#128270;  | ClusteredIndex | ON active\_for\_data\_integration|
| &#128270;  | ClusteredIndex | ON vch\_over\_po\_cost\_tolerance|
| &#128270;  | ClusteredIndex | ON vch\_under\_po\_cost\_tolerance|
| &#128270;  | ClusteredIndex | ON pay\_fiscal\_ytd|
| &#128270;  | ClusteredIndex | ON pay\_lst\_fiscal\_yr|
| &#128270;  | ClusteredIndex | ON supply\_web\_vendor|
| &#128270;  | ClusteredIndex | ON request\_acknowledgement|
| &#128270;  | ClusteredIndex | ON synchronized\_to\_bus|
| &#128270;  | ClusteredIndex | ON show\_in\_drop\_down\_list|
| &#128270;  | ClusteredIndex | ON auto\_voucher|
| &#128270;  | ClusteredIndex | ON auto\_voucher\_method|
| &#128270;  | ClusteredIndex | ON international\_bank\_account|
| &#128270;  | ClusteredIndex | ON buyer|
| &#128270;  | ClusteredIndex | ON deposit\_acct\_type|
| &#128270;  | ClusteredIndex | ON allow\_to\_firm\_plns|
| &#128270;  | ClusteredIndex | ON firm\_pln\_target|
| &#128270;  | ClusteredIndex | ON firmed\_poitem\_stat|
| &#128270;  | ClusteredIndex | ON replen\_po\_num|
| &#128270;  | ClusteredIndex | ON transit\_reference|
| &#128270;  | ClusteredIndex | ON misc1099\_ytd|
| &#128270;  | ClusteredIndex | ON misc1099\_lst\_yr|
| &#128270;  | ClusteredIndex | ON source\_site|
| &#128270;  | ClusteredIndex | ON source\_site\_cust\_num|
| &#128270;  | ClusteredIndex | ON auto\_receive\_demanding\_site\_po|
| &#128270;  | ClusteredIndex | ON auto\_ship\_demanding\_site\_co|
| &#128270;  | ClusteredIndex | ON minority\_owned|
| &#128270;  | ClusteredIndex | ON th\_wht\_type|
| &#128270;  | ClusteredIndex | ON mx\_tax\_reg\_num\_type|
| &#128270;  | ClusteredIndex | ON mx\_vendor\_diot\_type|
| &#128270;  | ClusteredIndex | ON tax\_reg\_num1\_exp\_date|
| &#128270;  | ClusteredIndex | ON jp\_eft\_bank\_fee\_terms|
| &#128270;  | ClusteredIndex | ON jp\_bank\_branch\_name|
| &#128270;  | ClusteredIndex | ON jp\_account\_owner\_name|
| &#128270;  | ClusteredIndex | ON jp\_zengin\_bank\_code|
| &#128270;  | ClusteredIndex | ON jp\_zengin\_branch\_code|
| &#128270;  | ClusteredIndex | ON jp\_zengin\_acct\_no|
| &#128270;  | ClusteredIndex | ON jp\_account\_ref\_1|
| &#128270;  | ClusteredIndex | ON jp\_account\_ref\_2|
| &#128270;  | ClusteredIndex | ON cust\_num|
| &#128270;  | ClusteredIndex | ON vend\_bank|
| &#128270;  | ClusteredIndex | ON bank\_file\_format|
| &#128270;  | ClusteredIndex | ON picture|
| &#128270;  | ClusteredIndex | ON fiscal\_rpt\_system|
| &#128270;  | ClusteredIndex | ON fiscal\_rpt\_system\_type|
| &#128270;  | ClusteredIndex | ON business\_identification\_num|
| &#128270;  | ClusteredIndex | ON profession|
| &#128270;  | ClusteredIndex | ON au\_contract\_price\_method|
| &#128270;  | ClusteredIndex | ON bank\_authority\_party\_id|
| &#128270;  | ClusteredIndex | ON bank\_transit\_num|
| &#128270;  | ClusteredIndex | ON override\_bank\_transit\_num|
| &#128270;  | ClusteredIndex | ON head\_office|
| &#128270;  | ClusteredIndex | ON branch\_name|
| &#128270;  | ClusteredIndex | ON active\_for\_anonymization|
| &#128270;  | ClusteredIndex | ON uf\_company\_reg|
| &#128270;  | ClusteredIndex | ON uf\_ni\_number|
| &#128270;  | ClusteredIndex | ON uf\_partner\_name|
| &#128270;  | ClusteredIndex | ON uf\_tax\_treatment|
| &#128270;  | ClusteredIndex | ON uf\_utr\_no|
| &#128270;  | ClusteredIndex | ON uf\_vn|
| &#128270;  | ClusteredIndex | ON uf\_bank\_address\_details|
| &#128270;  | ClusteredIndex | ON uf\_bank\_int\_code|
| &#128270;  | ClusteredIndex | ON uf\_beneficiary|
| &#128270;  | ClusteredIndex | ON uf\_managed\_by|
| &#128270;  | ClusteredIndex | ON uf\_vend\_qty\_tol|
| &#128270;  | ClusteredIndex | ON \_ingestion\_unit|
| &#128270;  | ClusteredIndex | ON \_run\_id|
| &#128270;  | ClusteredIndex | ON \_execution\_id|
| &#128270;  | ClusteredIndex | ON \_loaded\_at|




## View vw_active_dataset_config

Query vw_active_dataset_config
```
/* ===================================================================
   sql/40\_views/01\_monitoring\_views.sql
   =================================================================== */
/* Operational monitoring views over the metadata schema. */

CREATE   VIEW metadata.vw\_active\_dataset\_config
AS
SELECT
    dataset\_config\_row.dataset\_id,
    dataset\_config\_row.dataset\_name,
    dataset\_config\_row.execution\_order,
    dataset\_config\_row.load\_mode,
    dataset\_config\_row.source\_lakehouse,
    dataset\_config\_row.source\_schema,
    dataset\_config\_row.source\_table,
    dataset\_config\_row.staging\_schema,
    dataset\_config\_row.staging\_table,
    dataset\_config\_row.staging\_inbound\_table,
    dataset\_config\_row.watermark\_column,
    dataset\_config\_row.initial\_watermark,
    dataset\_config\_row.merge\_keys,
    dataset\_watermark\_row.last\_successful\_watermark,
    dataset\_watermark\_row.last\_successful\_run\_id,
    dataset\_config\_row.updated\_at AS config\_updated\_at
FROM metadata.dataset\_config dataset\_config\_row
LEFT JOIN metadata.dataset\_watermark dataset\_watermark\_row ON dataset\_watermark\_row.dataset\_id = dataset\_config\_row.dataset\_id
WHERE dataset\_config\_row.is\_active = 1
```

|Idx |Name |Type |
|---|---|---|
| * | dataset\_id| bigint  |
| * | dataset\_name| varchar(128)  |
| * | execution\_order| int  |
| * | load\_mode| varchar(20)  |
| * | source\_lakehouse| varchar(128)  |
| * | source\_schema| varchar(128)  |
| * | source\_table| varchar(128)  |
| * | staging\_schema| varchar(128)  |
| * | staging\_table| varchar(128)  |
|  | staging\_inbound\_table| varchar(128)  |
|  | watermark\_column| varchar(128)  |
|  | initial\_watermark| datetime2(26)  |
|  | merge\_keys| varchar(400)  |
|  | last\_successful\_watermark| datetime2(26)  |
|  | last\_successful\_run\_id| bigint  |
| * | config\_updated\_at| datetime2(26)  |


## View vw_curation_execution_history

Query vw_curation_execution_history
```
CREATE   VIEW ${schemaName}.${viewName}
AS
SELECT
    curation\_execution\_row.execution\_id,
    curation\_execution\_row.run\_id,
    gold\_run\_row.trigger\_time AS run\_trigger\_time,
    curation\_execution\_row.procedure\_id,
    curation\_execution\_row.schema\_name,
    curation\_execution\_row.procedure\_name,
    curation\_execution\_row.execution\_group,
    curation\_execution\_row.execution\_order,
    curation\_execution\_row.status,
    curation\_execution\_row.start\_time,
    curation\_execution\_row.end\_time,
    DATEDIFF(SECOND, curation\_execution\_row.start\_time, ISNULL(curation\_execution\_row.end\_time, SYSUTCDATETIME())) AS duration\_seconds,
    curation\_execution\_row.error\_number,
    curation\_execution\_row.error\_message
FROM metadata.curation\_execution curation\_execution\_row
INNER JOIN metadata.gold\_run gold\_run\_row ON gold\_run\_row.run\_id = curation\_execution\_row.run\_id
```

|Idx |Name |Type |
|---|---|---|
| * | execution\_id| bigint  |
| * | run\_id| bigint  |
| * | run\_trigger\_time| datetime2(26)  |
| * | procedure\_id| bigint  |
| * | schema\_name| varchar(128)  |
| * | procedure\_name| varchar(128)  |
| * | execution\_group| int  |
| * | execution\_order| int  |
| * | status| varchar(30)  |
| * | start\_time| datetime2(26)  |
|  | end\_time| datetime2(26)  |
|  | duration\_seconds| int  |
|  | error\_number| int  |
|  | error\_message| varchar(4000)  |


## View vw_current_run_status

Query vw_current_run_status
```
CREATE   VIEW ${schemaName}.${viewName}
AS
SELECT
    gold\_run\_row.run\_id,
    gold\_run\_row.pipeline\_run\_id,
    gold\_run\_row.trigger\_time,
    gold\_run\_row.start\_time,
    gold\_run\_row.status AS run\_status,
    (SELECT COUNT(execution\_id) FROM metadata.dataset\_execution dataset\_execution\_row WHERE dataset\_execution\_row.run\_id = gold\_run\_row.run\_id AND dataset\_execution\_row.status = 'running')   AS datasets\_running,
    (SELECT COUNT(execution\_id) FROM metadata.dataset\_execution dataset\_execution\_row WHERE dataset\_execution\_row.run\_id = gold\_run\_row.run\_id AND dataset\_execution\_row.status = 'succeeded') AS datasets\_succeeded,
    (SELECT COUNT(execution\_id) FROM metadata.dataset\_execution dataset\_execution\_row WHERE dataset\_execution\_row.run\_id = gold\_run\_row.run\_id AND dataset\_execution\_row.status = 'failed')    AS datasets\_failed,
    (SELECT COUNT(execution\_id) FROM metadata.curation\_execution curation\_execution\_row WHERE curation\_execution\_row.run\_id = gold\_run\_row.run\_id AND curation\_execution\_row.status = 'running')   AS curation\_running,
    (SELECT COUNT(execution\_id) FROM metadata.curation\_execution curation\_execution\_row WHERE curation\_execution\_row.run\_id = gold\_run\_row.run\_id AND curation\_execution\_row.status = 'succeeded') AS curation\_succeeded,
    (SELECT COUNT(execution\_id) FROM metadata.curation\_execution curation\_execution\_row WHERE curation\_execution\_row.run\_id = gold\_run\_row.run\_id AND curation\_execution\_row.status = 'failed')    AS curation\_failed
FROM metadata.gold\_run gold\_run\_row
WHERE gold\_run\_row.status = 'running'
```

|Idx |Name |Type |
|---|---|---|
| * | run\_id| bigint identity  |
|  | pipeline\_run\_id| varchar(100)  |
| * | trigger\_time| datetime2(26)  |
| * | start\_time| datetime2(26)  |
| * | run\_status| varchar(30)  |
|  | datasets\_running| int  |
|  | datasets\_succeeded| int  |
|  | datasets\_failed| int  |
|  | curation\_running| int  |
|  | curation\_succeeded| int  |
|  | curation\_failed| int  |


## View vw_dataset_execution_history

Query vw_dataset_execution_history
```
CREATE   VIEW ${schemaName}.${viewName}
AS
SELECT
    dataset\_execution\_row.execution\_id,
    dataset\_execution\_row.run\_id,
    gold\_run\_row.trigger\_time AS run\_trigger\_time,
    dataset\_execution\_row.dataset\_id,
    dataset\_execution\_row.dataset\_name,
    dataset\_execution\_row.load\_mode,
    dataset\_execution\_row.data\_from\_timestamp,
    dataset\_execution\_row.data\_to\_timestamp,
    dataset\_execution\_row.status,
    dataset\_execution\_row.row\_count,
    dataset\_execution\_row.start\_time,
    dataset\_execution\_row.end\_time,
    DATEDIFF(SECOND, dataset\_execution\_row.start\_time, ISNULL(dataset\_execution\_row.end\_time, SYSUTCDATETIME())) AS duration\_seconds,
    dataset\_execution\_row.error\_number,
    dataset\_execution\_row.error\_message
FROM metadata.dataset\_execution dataset\_execution\_row
INNER JOIN metadata.gold\_run gold\_run\_row ON gold\_run\_row.run\_id = dataset\_execution\_row.run\_id
```

|Idx |Name |Type |
|---|---|---|
| * | execution\_id| bigint  |
| * | run\_id| bigint  |
| * | run\_trigger\_time| datetime2(26)  |
| * | dataset\_id| bigint  |
| * | dataset\_name| varchar(128)  |
| * | load\_mode| varchar(20)  |
|  | data\_from\_timestamp| datetime2(26)  |
|  | data\_to\_timestamp| datetime2(26)  |
| * | status| varchar(30)  |
|  | row\_count| bigint  |
| * | start\_time| datetime2(26)  |
|  | end\_time| datetime2(26)  |
|  | duration\_seconds| int  |
|  | error\_number| int  |
|  | error\_message| varchar(4000)  |


## View vw_gold_run_history

Query vw_gold_run_history
```
CREATE   VIEW ${schemaName}.${viewName}
AS
SELECT
    run\_id,
    pipeline\_run\_id,
    trigger\_time,
    start\_time,
    end\_time,
    status,
    DATEDIFF(SECOND, start\_time, ISNULL(end\_time, SYSUTCDATETIME())) AS duration\_seconds
FROM metadata.gold\_run
```

|Idx |Name |Type |
|---|---|---|
| * | run\_id| bigint identity  |
|  | pipeline\_run\_id| varchar(100)  |
| * | trigger\_time| datetime2(26)  |
| * | start\_time| datetime2(26)  |
|  | end\_time| datetime2(26)  |
| * | status| varchar(30)  |
|  | duration\_seconds| int  |


## View vw_recent_failures

Query vw_recent_failures
```
CREATE   VIEW ${schemaName}.${viewName}
AS
SELECT 'dataset' AS item\_type, dataset\_execution\_row.execution\_id, dataset\_execution\_row.run\_id, dataset\_execution\_row.dataset\_name AS item\_name,
       dataset\_execution\_row.status, dataset\_execution\_row.error\_number, dataset\_execution\_row.error\_message, dataset\_execution\_row.end\_time
FROM metadata.dataset\_execution dataset\_execution\_row
WHERE dataset\_execution\_row.status = 'failed'
UNION ALL
SELECT 'curation\_procedure', curation\_execution\_row.execution\_id, curation\_execution\_row.run\_id,
       curation\_execution\_row.schema\_name + '.' + curation\_execution\_row.procedure\_name,
       curation\_execution\_row.status, curation\_execution\_row.error\_number, curation\_execution\_row.error\_message, curation\_execution\_row.end\_time
FROM metadata.curation\_execution curation\_execution\_row
WHERE curation\_execution\_row.status = 'failed'
```

|Idx |Name |Type |
|---|---|---|
| * | item\_type| varchar(18)  |
| * | execution\_id| bigint  |
| * | run\_id| bigint  |
| * | item\_name| varchar(257)  |
| * | status| varchar(30)  |
|  | error\_number| int  |
|  | error\_message| varchar(4000)  |
|  | end\_time| datetime2(26)  |
## Schema metadata
### Functions 
usp\_complete\_curation\_execution 
```

```
usp\_complete\_dataset\_execution 
```

```
usp\_complete\_gold\_run 
```

```
usp\_fail\_curation\_execution 
```

```
usp\_fail\_dataset\_execution 
```

```
usp\_finalize\_dataset\_staging 
```

```
usp\_get\_active\_curation\_procedures 
```

```
usp\_get\_active\_datasets 
```

```
usp\_skip\_curation\_execution 
```

```
usp\_skip\_dataset\_execution 
```

```
usp\_start\_config\_import\_batch 
```

```
usp\_start\_curation\_execution 
```

```
usp\_start\_dataset\_execution 
```

```
usp\_start\_gold\_run 
```

```
usp\_update\_dataset\_watermark 
```

```
usp\_upsert\_curation\_procedure\_config 
```

```
usp\_upsert\_dataset\_config 
```

```
### Procedures
usp\_complete\_curation\_execution 
```

```
usp\_complete\_dataset\_execution 
```

```
usp\_complete\_gold\_run 
```

```
usp\_fail\_curation\_execution 
```

```
usp\_fail\_dataset\_execution 
```

```
usp\_finalize\_dataset\_staging 
```

```
usp\_get\_active\_curation\_procedures 
```

```
usp\_get\_active\_datasets 
```

```
usp\_skip\_curation\_execution 
```

```
usp\_skip\_dataset\_execution 
```

```
usp\_start\_config\_import\_batch 
```

```
usp\_start\_curation\_execution 
```

```
usp\_start\_dataset\_execution 
```

```
usp\_start\_gold\_run 
```

```
usp\_update\_dataset\_watermark 
```

```
usp\_upsert\_curation\_procedure\_config 
```

```
usp\_upsert\_dataset\_config 
```

```


## Schema reporting
### Functions 
usp\_build\_dim\_date 
```

```
usp\_load\_fact\_kpi\_result 
```

```
### Procedures
usp\_build\_dim\_date 
```

```
usp\_load\_fact\_kpi\_result 
```

```


## Schema salesforce
### Functions 
usp\_build\_design\_rnd\_facts 
```

```
usp\_build\_fact\_estimating 
```

```
usp\_build\_kpi\_result\_design\_rnd 
```

```
usp\_publish\_design\_rnd\_kpis 
```

```
### Procedures
usp\_build\_design\_rnd\_facts 
```

```
usp\_build\_fact\_estimating 
```

```
usp\_build\_kpi\_result\_design\_rnd 
```

```
usp\_publish\_design\_rnd\_kpis 
```

```


## Schema safety_culture
### Functions 
usp\_build\_ehs\_safetyculture\_all 
```

```
usp\_build\_fact\_ehs\_visual\_inspection 
```

```
usp\_build\_fact\_ehs\_visual\_inspection\_weekly 
```

```
usp\_build\_kpi\_result\_ehs\_safetyculture 
```

```
usp\_publish\_ehs\_safetyculture\_kpis 
```

```
### Procedures
usp\_build\_ehs\_safetyculture\_all 
```

```
usp\_build\_fact\_ehs\_visual\_inspection 
```

```
usp\_build\_fact\_ehs\_visual\_inspection\_weekly 
```

```
usp\_build\_kpi\_result\_ehs\_safetyculture 
```

```
usp\_publish\_ehs\_safetyculture\_kpis 
```

```


## Schema freshservice
### Functions 
usp\_build\_and\_publish\_freshservice\_all 
```

```
usp\_build\_fact\_it\_freshservice\_survey 
```

```
usp\_build\_fact\_it\_freshservice\_survey\_weekly 
```

```
usp\_build\_fact\_it\_freshservice\_ticket 
```

```
usp\_build\_fact\_it\_freshservice\_ticket\_weekly 
```

```
usp\_build\_freshservice\_all 
```

```
usp\_build\_kpi\_result\_it\_freshservice 
```

```
usp\_publish\_freshservice\_kpis 
```

```
### Procedures
usp\_build\_and\_publish\_freshservice\_all 
```

```
usp\_build\_fact\_it\_freshservice\_survey 
```

```
usp\_build\_fact\_it\_freshservice\_survey\_weekly 
```

```
usp\_build\_fact\_it\_freshservice\_ticket 
```

```
usp\_build\_fact\_it\_freshservice\_ticket\_weekly 
```

```
usp\_build\_freshservice\_all 
```

```
usp\_build\_kpi\_result\_it\_freshservice 
```

```
usp\_publish\_freshservice\_kpis 
```

```


## Schema syteline
### Functions 
usp\_Publish\_Product\_Engineering\_Cost 
```

```
usp\_build\_and\_publish\_product\_engineering\_cost 
```

```
usp\_build\_and\_publish\_product\_engineering\_productivity\_all 
```

```
usp\_build\_fact\_product\_engineering\_4\_week\_value\_weekly 
```

```
usp\_build\_kpi\_result\_product\_engineering\_cost 
```

```
usp\_build\_kpi\_result\_product\_engineering\_productivity 
```

```
usp\_build\_product\_engineering\_cost 
```

```
usp\_build\_product\_engineering\_items\_completed\_daily 
```

```
usp\_build\_product\_engineering\_productivity\_all 
```

```
usp\_build\_product\_engineering\_productivity\_facts 
```

```
usp\_capture\_product\_engineering\_4\_week\_value\_snapshot 
```

```
usp\_capture\_product\_engineering\_productivity\_inputs 
```

```
usp\_publish\_product\_engineering\_productivity 
```

```
### Procedures
usp\_Publish\_Product\_Engineering\_Cost 
```

```
usp\_build\_and\_publish\_product\_engineering\_cost 
```

```
usp\_build\_and\_publish\_product\_engineering\_productivity\_all 
```

```
usp\_build\_fact\_product\_engineering\_4\_week\_value\_weekly 
```

```
usp\_build\_kpi\_result\_product\_engineering\_cost 
```

```
usp\_build\_kpi\_result\_product\_engineering\_productivity 
```

```
usp\_build\_product\_engineering\_cost 
```

```
usp\_build\_product\_engineering\_items\_completed\_daily 
```

```
usp\_build\_product\_engineering\_productivity\_all 
```

```
usp\_build\_product\_engineering\_productivity\_facts 
```

```
usp\_capture\_product\_engineering\_4\_week\_value\_snapshot 
```

```
usp\_capture\_product\_engineering\_productivity\_inputs 
```

```
usp\_publish\_product\_engineering\_productivity 
```

```




