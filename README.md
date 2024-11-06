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

![Sales dat](https://github.com/user-attachments/assets/90ba3756-9082-4e17-8c19-9924d5342571)

![Screenshot (26)](https://github.com/user-attachments/assets/91f27232-1618-4b1d-a694-83d742f43b27)

![Screenshot (25)](https://github.com/user-attachments/assets/b191072c-6e44-4ffa-9548-0440c098f0ce)

![Screenshot (24)](https://github.com/user-attachments/assets/b98f358b-e1f2-44e2-9273-fb3448c88ac9)

![Screenshot (23)](https://github.com/user-attachments/assets/2543d6aa-715f-4ac4-be55-1529d5f4e2ef)

![Screenshot (29)](https://github.com/user-attachments/assets/f2dcf69c-6ab4-4c0f-887a-2508fcedfd40)

![Screenshot (28)](https://github.com/user-attachments/assets/d1870df9-de64-4453-af7d-f0bc38f2e9f8)

![Screenshot (27)](https://github.com/user-attachments/assets/a0601715-50e9-4a98-b64c-96ba850a7178)

![Screenshot (66)](https://github.com/user-attachments/assets/374ef17e-16cf-40fa-b551-103c1a55f05a)

![Screenshot (65)](https://github.com/user-attachments/assets/d73e915b-33c0-42b8-81c9-2395f01f33b2)

![Screenshot (64)](https://github.com/user-attachments/assets/18244588-4ad3-4264-8f9b-1d470772aea2)

![Screenshot (62)](https://github.com/user-attachments/assets/7d2e95c0-2903-4b03-af95-6599e614dd0e)

![Screenshot (61)](https://github.com/user-attachments/assets/2c7227c4-6fce-4bdb-a9a9-b1fcc0669fe8)

![Screenshot (67)](https://github.com/user-attachments/assets/8fa48c1b-f547-4add-be28-6eeab35d6ac4)

![Screenshot (69)](https://github.com/user-attachments/assets/27af6c6e-c9ea-4e5d-b1d3-2ccf83e53516)


#### Inference.
It was discovered through the analysis that Shoes generated the highest revenue (#6,133,380), followed by Shirts (#485,600), Hats (#3,161,950), Gloves (#296,900), Jackets (#208,230), and Socks (#180,785).
Although Shoes generated the highest revenue, it does not have the highest units sold (14,402), Hats had the highest units sold (15,929). Jackets, however, sold the lowest at 5,452 units.

By region, the total revenue was highest in the South (#927,820) and lowest in the West (#300,345).

In 2023, the highest sales were recorded in July (#237,600) with 5,940 units sold, the lowest sales in April (#7,425) with 1,485 units.  
In 2024, the highest sales occurred in February (#298,800) with 4,980 units, while the lowest was recorded in July (#37,200) with 2,480 units.

In addition, 

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
