# Every click counts

## Backstory
Thank you for helping Fabrikam save its reputation in the last Act. Now, we are ready to look at the demand, and adjust our supply chain accordingly. Fabrikam is getting a huge number of orders due to sudden surge in demand after some celebrities posted about our products on their social media handles. We want to capture clickstream data through various sources, analyze it and take actions to maximize our revenue.

## Setup
For running this Act, 
1. New Eventstream that captures clickstream data.
2. Use the attached "Clickstream Simulator" notebook to generate clickstream data. The notebook will generate data and push it to an Eventstream that you can configure.
3. Knowledge of Kusto Query Language (KQL) to analyze the data.
4. Data Factory to create pipelines.
5. Power BI to create reports.

## Challenges 

## Filter Clickstream data for US traffic only and aggregate total clicks by product and website for 10 minutes.
    Hint: Use filter transformation to filter origin country
    Hint: Use aggregate transformation

## Increase the cost of top 3 most demanded products of all time by 15% each day
    Hint: Use the power of KQL to find top 3 products
    Hint: You can update tables in KQL
    Hint: Setup everyday pipeline to run updates

## Create a “Growth Opportunity” Report
1. Create a Power BI report that shows the following information
2. Filters – Time, and Products
3. Card Visuals – In-demand product, Website with Highest traffic
4. Time charts - Product clicks over time, Products bought over time
5. Pie charts – Website traffic distribution, Device traffic distribution
