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

### Data Analysis, Visual Analysis and Inference
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


![Screenshot (47)](https://github.com/user-attachments/assets/95210d48-ae51-4d60-96f3-eee969c35954)

![Screenshot (48)](https://github.com/user-attachments/assets/d8e7ca85-21d8-48f3-89a8-2ddc61deefc6)

![Screenshot (49)](https://github.com/user-attachments/assets/3b5edf4e-c95d-46c3-a713-68d9a56bf1af)

![Screenshot (50)](https://github.com/user-attachments/assets/67448b3f-f1e5-4185-ab5b-d80fd2181194)

![Screenshot (51)](https://github.com/user-attachments/assets/45a32a1f-d413-4faf-872f-4ce23fcc0d73)

![Screenshot (23)](https://github.com/user-attachments/assets/11cbaaa0-17ad-49e1-aa18-1ea0204f565d)

![Screenshot (24)](https://github.com/user-attachments/assets/852830d2-1893-494c-bd9a-2ea84c6e89af)

![Screenshot (25)](https://github.com/user-attachments/assets/4aa14c7c-331b-4040-aa27-ab7fcf81b07a)

![Screenshot (26)](https://github.com/user-attachments/assets/4dbe944c-4ff6-4dee-bfc3-11284774dfa6)

![Screenshot (27)](https://github.com/user-attachments/assets/164a2157-cdb3-4b7b-9b97-66627700980c)

![Screenshot (28)](https://github.com/user-attachments/assets/a08184d6-af79-47cb-991d-f0ac0fe50eed)

![Screenshot (29)](https://github.com/user-attachments/assets/143a0995-12ce-4f4b-8b8d-d4d4e461af10)



