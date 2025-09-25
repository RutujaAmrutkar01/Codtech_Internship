# Codtech_Internship
Internship Task-1 : Sales Dashboard
📌 Project Overview
This project is part of the CodTech Internship Program.
The task was to develop a Power BI Sales Dashboard to visualize sales performance using sample data.

📊 Dataset
The dataset contains the following columns:
Date
Region
Product
Sales

🎯 Objectives
Show sales trends over time
Identify top products by sales
Compare regional sales performance
Provide interactive slicers for filtering

🛠️ Tools Used
Power BI Desktop

📁 Deliverables
Power BI file: Sales_Dashboard.pbix
Interactive dashboard visuals with slicers

🚀 How to Use
Open the .pbix file in Power BI Desktop
Explore dashboard visuals (trends, top products, regional performance)
Use slicers for filtering by Date, Region, and Product

🏆 Outcome
The dashboard provides insights into sales performance, helping to understand product trends and regional growth.# Codtech_Internship# Codtech_Internship



# Task 2: Sales and Customer Analysis
This project analyzes sales and customer data. 
You can perform region-wise sales, product-wise sales, and customer-age analysis.

## Tables
 Sales Table
| Column | Description |
|--------|------------|
| Date   | Date of the sale |
| Region | Region where the sale happened |
| Product | Product sold |
| Sales  | Amount of sales |

Customer Table
| Column | Description |
|--------|------------|
| CustomerID | Unique ID of the customer |
| CustomerName | Name of the customer |
| Age | Age of the customer |
| Region | Region of the customer |

## Example SQL Queries
1. Total Sales by Region
sql
SELECT Region, SUM(Sales) AS TotalSales
FROM Sales
GROUP BY Region;

2. Customer Details with Sales
sql
SELECT c.CustomerID, c.CustomerName, c.Age, c.Region, s.Product, s.Sales, s.Date
FROM Customer c
JOIN Sales s ON c.Region = s.Region;

3. Average Sales by Customer Age
sql
SELECT c.Age, AVG(s.Sales) AS AvgSales
FROM Customer c
JOIN Sales s ON c.Region = s.Region
GROUP BY c.Age;

Usage
Create tables in SQL database.
Insert the data.
Use the SQL queries above to perform analysis.

