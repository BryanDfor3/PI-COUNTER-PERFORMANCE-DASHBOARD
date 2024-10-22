# PI Counter Performance Dashboard

![PI_Counter_Performance_Dashboard_Screenshot](https://github.com/user-attachments/assets/4d7fd8fb-21fd-4cbc-82bb-ebeef9a285c1)

(Note: The actual data used for the client engagement has been scrubbed and replaced with dummy data in the sceenshot above)

## Business Problem
To meet its compliance standards, an automotive manufacturer needed to perform quarterly physical inventory (PI) counts until its goal threshold was met (90% accuracy). These physical inventory counts required the manufacturing plant to have to temporarily shut down, and in the previous quarter, the manufacturer not only severely missed its target accuracy, but also had to use 9 days to complete the inventory count. This resulted in significant downtime for the factory that led to the underproduction of vehicles assembled.

After a successful implementation of the [PI Count Dashboard]([url](https://github.com/BryanDfor3/PI-COUNT-TRACKING-DASHBOARD)), the client wanted a way to view the performance of individual counters to be able to reward the best counters who were contributing the most positively towards the accuracy target (90%), and have insight into which counters may need to replacing due to their contributions hurting the overall counting accuracy.  

## Methodology
1. Leverage the data being ETL'd for the PI Count Dashboard, with a separate flow of data transformation steps incorporated into Alteryx to produce a new Tableau data source for counter performance visuals
2. Incorporate counter performance rank calculation into the Alteryx data flow

**`Counter Rank = RANK(([Accurate Count Percentage] / 0.9)^([Number of Counts Performed]))`**

3. Develop the Tableau visualizations, clearly highlighting the subset of counters who are positively contributing to the accuracy target (green shaded area)


## Skills
1. Data Extraction - SQL
2. Data Transformation, Data Cleansing - Alteryx
3. Data Visualization - Tableau / Tableau Server


## Results
The client was able to realize a 27% improvement in their inventory accuracy, and was eventually able to meet their accuracy target of 90%, in part due to having the visibility offered by the Counter Performance dashboard.

