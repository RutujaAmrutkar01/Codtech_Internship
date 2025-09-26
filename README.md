# Codtech_Internship
# Task 1: Sales Dashboard
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



#  Task 3 :Real-Time Dashboard
📌 Task Objective
Set up a *real-time dashboard* using streaming data (e.g., from Azure or a simulated API feed).  
Deliverable: A *live Power BI dashboard* that updates in real time.  
 
📊 Features
- Real-time data visualization in *Power BI*  
- Data fields included:
  - ⏰ *Time*  
  - 🌡️ *Temperature*  
  - 👥 *Visitors*  
  - 💰 *Sales*  
  - 📦 *API JSON Data (with related date)*  
- Auto-refreshing dashboard using streaming API  

🔗 Data Source
The dashboard uses:
- *Simulated JSON API feed* (can be replaced with Azure Streaming Data).  

*Sample JSON structure:*
```json
{
  "time": "2025-09-26T10:30:00Z",
  "temperature": 28.5,
  "visitors": 120,
  "sales": 45,
  "date": "2025-09-26"
}
connect the dgfdyfvmm
⚙️ Setup Instructions
Connect Power BI to the JSON streaming API.
Import the data model with the above fields.
Enable real-time streaming for the dataset.
Design dashboard visuals (line chart for temperature, bar chart for sales, card for visitors, etc.).
Enable auto-refresh to keep the dashboard live.

📌 Deliverable
A Power BI real-time dashboard that displays and auto-updates with:
Time
Temperature
Visitors
Sales
API JSON Data

✅ Completion
This fulfills Task-3 of the CODTECH Internship program.





