# Advanced-Reporting-and-Analytics-for-Guyus-Real-Estate

## Problem Statement

Guyus Real Estate, a successful company, has a hard time with its reporting and analytical processes. The company relies on manual Excel reports, which are time-consuming, prone to errors, and limited in analytical capabilities. This leads to delayed decision-making, affecting the company's competitive edge and market responsiveness.

To solve this, Guyus Real Estate plans to implement an automated reporting system using Power BI. This will enable:

- Automated data reporting, eliminating manual errors and saving time
- A comprehensive data model, structuring data for easier analysis and reporting
- Integration of diverse data sources, ensuring data integrity and consistency
- Enhanced analytical capabilities, uncovering market trends, performance metrics, and actionable insights

By implementing Power BI, Guyus Real Estate aims to streamline its reporting process, improve data accuracy, and enhance its analytical capabilities, ultimately enabling informed, timely decision-making and maintaining its competitive edge in the market.

### Steps followed 

- Step 1 : Load data into Power BI Desktop, it's folder that contains multiple files so  combine it.
- Step 2 : Open power query editor & clean the data.
- Step 3 : In the Power BI model view, create a new table for the calender dimension.
- Step 4 :  Define the table structure (e.g., columns, data types).
- Step 5 :  Establish relationships between tables using keys (e.g., fact table to property Dim), Use the "Manage Relationships" dialog to define cardinality and cross-filtering. Also Create measures and calculated columns as needed
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 :  A new visual was added using the three ellipses in the visualizations pane in report view. 
- Step 8 : Visual filters (Slicers) were added for three fields named "Quater", "property Type" & "Month Name".
- Step 9 : Four card visuals were added to the canvas, representing No of Transactions, Average Sales, Total Sales Amount & Max of Sales Price.
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
- Step 10 : A map chart was added to the report design area representing total sales amount by state a line chart representing sum of sales price by month name, a doughnut chart representing total sales amount by proprty type, a clustered bar chart representing no of transaction by city and property type and a decomposition tree breaking down tnh property type, state and agent name.
- Step 11 : card Visual was used to represent different transactions 
 

- Step 12 : In the report view, Drag and drop fields from the "Fields" pane to the visualization.
- Step 13 : Use the "Format" pane to customize appearance. 
- Step 14 :Table was created for the calculated measures

- Step 15 : New measure was created to find count of total no of transaction.
Following DAX expression was written for the same,
        
        No of transaction = COUNTROWS('Guyus Real Estate'[ID])
        
A card visual was used to represent count of customers.

        
 - Step 16 : New measure was created to find  Total sales amount,
 
 Following DAX expression was written to find Total sales amount,
 
         Total sales amount=SUM('Guyus Real Estate'[SalesPrice])
 
 A card visual was used to represent this.
 
 
 - Step 17 : New measure was created to calculate Average Sales & a card visual was used to represent this.
 
 Following DAX expression was written to find Average Sales,
 
         Average Sales =Average('Guyus Real Estate'[SalesPrice])
    
 
 
 - Step 18 : The report was then published to Power BI Service.
 
 

# Snapshot of Dashboard 

![GE](https://github.com/user-attachments/assets/b65a9bbd-5394-4775-8b10-2c97146960bf)

 #  Snapshot (Power BI DESKTOP)

 
![6e03b7c8-846d-4121-b02f-afbd780a9d03](https://github.com/user-attachments/assets/42e8368a-26df-4cbe-a312-37061315dc60)

# Insights

 Report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] KPIs
- Total sales amount - $3bn
- No of transactions - 6K
- Average Sales - $553K
- Max of Sales Price - $1,000k


   
           
### [2] Analysis on Property
- The land property had the highest sales
- The total sales dropped by 50% in the third quarter

Guyus real estate can leverage on Brand partnerships that will help the organization reach new audiences, increase their following, and drive revenue through strategic collaboration 
with complementary brands.

  ### [3] State Analysis
  
- The decomposition tree shows how each agent performs in different state. The agent in A2 and PA performed exceedingly low.
- Agents need to be contacted as to why their performance was that low. They could be linked to higher performang agents to learn strategies for a better performance

 ### [4] Some other insights
 
 ### February Analysis.
- Total Sales of $422m (a major drop of $52M from January).
- Total nunber of with an average sales of 556K.
- Highest sales from land with a total of $1.48M and Texas had the highest sales.
- Willam Johnson is the top agent with total sales of $3.372 916.
 
 ### Recommendation
 - Analyse the reasons behind disparity in Agents transactions. Has Top performance like Robert Davis specializing Property type or location Implement mentorship program to support other least performing Agents like  Linda and James.
- Adapt some strategies that resulted to higher sales in January, April and June to increase sales
in February and othermonths.
- Special offer should be introduced for the least Property Sales type.
- There should be Price discount for the sales of Commercial
and Residential Property Types
- Price discount and sales promotion should be introduced in the Cities with low sales.


# Guyus Real Estate Dashboard.md.txt
