# LITA_Projects - SalesData.
This repository will contain my Sales Data-project analyses and visualizations.

## PROJECT TITLE: Sales Data

### Project Overview 
---
This Data Analysis Project aims to generate insight into the sales performance of an organization over the past 2 years. Analysing the paramaters in the data, I sought to gather enough insight to make reasonable decisions, enabling me to tell a compelling story around the data from the insight gotten and to determine the best performance from the data.
---
### Tables of Content
[Data Sources](#Data-Sources)

[Data Collected](#Data-Collected)

[Tools used](#Tools-used)

[Data Cleaning and Preparation](Data-Cleaning-and-Preparation)

[Exploratory Data Analysis.](Exploratory-Data-Analysis.)

[Data Analysis, Visual Analysis and Inference](Data-Analysis-Visual-Analysis-and-Inference)

[Visual Analysis and Inference](Visual-Analysis-and-Inference)

[Recommendation](Recommendation)

### Data Sources
The primary source of data used is an Excel datasheet provided by the LITA Data Analysis Team.

### Data Collected
1. OrderID: A unique identifier assigned to a customer's order used for tracking orders, inventory management E.t.c
2. Customer Id: A unique identifier assigned to a customer, it helps in efficient customer management and tracking
3. Product: A good/service offered by a business to meet the needs and wants of its customers.
4. Region: The geographical area where the business operates.
5. OrderDate: The date on which a particular order/sale was made.
6. Quantity: The number of units sold per transaction/sale.
7. UnitPrice: The cost of a single unit of a product or service.

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
It provides insight into sales patterns, product popularity, and customer behaviour.

### Data Analysis
These are some of the codes, queries and formula used in the course of the analysis;

```SQL
SELECT month(OrderDate) AS month, SUM(Quantity * UnitPrice) AS Monthly_Total
FROM salesdata WHERE YEAR(OrderDate) = YEAR(curdate()) GROUP BY month(OrderDate) 
ORDER BY MONTH(OrderDate);

```SQL
SELECT `Customer Id`, SUM(Quantity * UnitPrice) AS Total_Purchase
FROM salesdata group by `Customer Id` ORDER BY Total_Purchase DESC LIMIT 5;

```EXCEL
	TotalSales = Quantity * UnitPrice
```

### Visual Analysis and Inference





![Screenshot (49)](https://github.com/user-attachments/assets/3b5edf4e-c95d-46c3-a713-68d9a56bf1af)

![Screenshot (50)](https://github.com/user-attachments/assets/67448b3f-f1e5-4185-ab5b-d80fd2181194)



![Screenshot (23)](https://github.com/user-attachments/assets/11cbaaa0-17ad-49e1-aa18-1ea0204f565d)

![Screenshot (24)](https://github.com/user-attachments/assets/852830d2-1893-494c-bd9a-2ea84c6e89af)

![Screenshot (25)](https://github.com/user-attachments/assets/4aa14c7c-331b-4040-aa27-ab7fcf81b07a)

![Screenshot (26)](https://github.com/user-attachments/assets/4dbe944c-4ff6-4dee-bfc3-11284774dfa6)

![Screenshot (27)](https://github.com/user-attachments/assets/164a2157-cdb3-4b7b-9b97-66627700980c)

![Screenshot (28)](https://github.com/user-attachments/assets/a08184d6-af79-47cb-991d-f0ac0fe50eed)

![Screenshot (29)](https://github.com/user-attachments/assets/143a0995-12ce-4f4b-8b8d-d4d4e461af10)


It was discovered through the analysis that Shoes generated the highest revenue (#6,133,380), followed by Shirts (#485,600), Hats (#3,161,950), Gloves (#296,900), Jackets (#208,230), and Socks (#180,785).
Although Shoes generated the highest revenue, it does not have the highest units sold (#14,402), Hats had the highest units sold (#15,929). Jackets, however, sold the lowest at #5,452 units.

By region, the total revenue was highest in the South (#927,820) and lowest in the West (#300,345).

In 2023, the highest sales were recorded in July (#237,600), with the lowest in April (#7,425).  
In 2024, the highest sales occurred in February (#298,800), while the lowest was in July (#37,200).

Purchase volume was greatest in the East (2,483 transactions) and lowest in the West (2,477 transactions).

The sales percentage was highest in the South (44.159%) and lowest in the West (14.295%).


### Recommendations.

Here are some recommendations based on the data inference:

1. Focus on High-Revenue Products:
   - Shoes generate the highest revenue, followed by Shirts and Hats. Increasing marketing efforts or expanding the product line for these categories could drive further sales. For example, promoting new shoe styles or seasonal clothing releases might attract additional purchases.

2. Boost Sales in Low-Performing Categories:
   - Jackets and Socks are among the lowest-revenue products. Increase their appeal by combining them with top-selling items or offering special discounts. Alternatively, evaluate the customer demand for these items if sales continue to lag.

3. Increase Focus in the South Region
   - The Southern region is leading in revenue and also has the highest sales percentage (44.159%). To maximize revenue potential, consider increasing stock availability, opening new locations, or launching targeted promotions in this region to leverage its high demand. 

4. Enhance Marketing in the West Region
   - With the lowest revenue and sales percentage, the West represents an area with potential for growth. Implement targeted marketing campaigns, promotions, or community engagement in this region to build brand awareness and increase sales.

5. Optimize Inventory and Supply Chain
   - The distribution of purchases across regions (East, North, South, and West) shows relatively even demand, with slight variation. Maintaining a balanced inventory across regions could help meet demand without overstocking.
Additionally, focusing on inventory for high-demand items like Shoes and Shirts in regions with high sales could optimize stock turnover and reduce costs.

6. Leverage Customer Insights for Loyalty Programs
   - Since the East had a high number of purchases and produced the highest revenue, it may be beneficial to implement loyalty programs in this region to retain these valuable customers. Engaging repeat customers with rewards, early access to new products, or exclusive discounts could drive repeat purchases.

7. Prepare for Expected Demand in High-Sales Months
   - With sales spikes in July 2023 and February 2024, planning for stock replenishment in advance of these months can help prevent stockouts and missed sales opportunities. Ensure adequate staffing and logistics support during these peak months.

- For months with lower sales (e.g., April 2023 and July 2024), consider running special promotions to stimulate demand during these periods.

8. Enhance Data Collection for Further Insights.
   - Gathering more detailed data on customer demographics, purchasing behavior, and feedback could help refine strategies. For example, understanding why specific regions or products underperform may provide insights to address these gaps effectively.
