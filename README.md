# LITA_Projects - SalesData.
This repository will contain my project analyses and visualizations.

## PROJECT TITLE: Sales Data

### Project Overview 
---
This Data Analysis Project aims to generate insight into the sales performance of an organization over the past 2 years. Analysing the paramaters in the data, I sought to gather enough insight to make reasonable decisions, enabling me to tell a compelling story around the data from the insight gotten and to determine the best performance from the data.
---
### Tables of Content
[Data Sources](#Data-Sources)
[Tools used](#Tools-used)
[Data Cleaning and Preparation](Data-Cleaning-and-Preparation)
[Exploratory Data Analysis.](Exploratory-Data-Analysis.)
[Data Analysis](Data-Analysis)

Result

Recommendation

Contribution

### Data Sources
The primary source of data used is an Excel datasheet provided by the LITA Data Analysis Team.

### Tools used
- Microsoft Excel for Data Cleaning, Analysis and Visualization.
- Structured Query Language - SQL for Querying of data.
- Power Bi for Visualization.
- GitHub for Portfolio Building

### Data Cleaning and Preparation.
After obtaining the dataset, the following action was performed;
1. Data Loading and Inspection.
2. Handling missing variables.
3. Data Cleaning and Formatting.

### Exploratory Data Analysis.
EDA involved the exploring of the data to answer some questions about the data;
- What are the total sales for each product category?
- The number of sales transactions in each region.
- The highest-selling product by total sales value.
- The average sales per product.
- The total revenue by region.


### Data Analysis
These are some of the codes, queries and formula used in the course of the analysis;

```SQL
SELECT month(OrderDate) AS month, SUM(Quantity * UnitPrice) AS Monthly_Total
FROM salesdata WHERE YEAR(OrderDate) = YEAR(curdate()) GROUP BY month(OrderDate) 
ORDER BY MONTH(OrderDate);

```SQL
SELECT `Customer Id`, SUM(Quantity * UnitPrice) AS Total_Purchase
FROM salesdata group by `Customer Id` ORDER BY Total_Purchase DESC LIMIT 5;





Perform an initial exploration of the sales data. Use pivot tables to summarize 
total sales by product, region, and month.
o Use Excel formulas to calculate metrics such as 
o Create any other interesting report
2. SQL:
Hint – You need to load the dataset into your SQL Server environment to write and 
validate your queries.
Write queries to extract key insights based on the following questions. 
o retrieve the 
o calculate total revenue per product.
o calculate monthly sales totals for the current year.
o find the top 5 customers by total purchase amount.
o calculate the percentage of total sales contributed by each region.
o identify products with no sales in the last quarter.


###SALESDATA
