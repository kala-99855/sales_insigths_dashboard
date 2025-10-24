# Sales Insights Dashboard using Power BI
## Project Objectives

The main objective of this project is to analyze sales data stored in a SQL Server database and create an interactive Power BI dashboard that provides meaningful business insights.

Key objectives:

•	To visualize overall sales, profit, and quantity trends over time.

•	To identify top-performing products, customers, and regions.

•	To compare sales performance across different periods and locations.

•	To help management make data-driven decisions through interactive visuals.

•	To integrate Power BI with SQL Server for automated data refresh and live analysis.

## Dataset Used

Data Source: Microsoft SQL Server

Database Name: Sales Insights

Tables Imported:

1.	Customers – Customer ID, Name, Location, Segment, Region
2.	Transactions – Transaction ID, Date, Product ID, Customer ID, Quantity, Amount
3.	Products – Product ID, Product Name, Category, Sub-Category, Unit Price
4.	Regions – Region Name, State, Country
5.	Sales Targets (optional) – Target Amount per Region/Month
The data was extracted using SQL queries and imported into Power BI through a Direct Query or Import mode connection.

## KPIs / Dashboard Questions

These Key Performance Indicators (KPIs) and business questions guide the dashboard’s visual design:
Key KPIs:

•	✅ Total Sales
•	✅ Total Profit
•	✅ Total Quantity Sold
•	✅ Average Sales per Transaction
•	✅ Profit Margin (%)
•	✅ Sales Growth Rate (%)

Business Questions Answered:

1.	What is the total revenue and profit generated this year?
2.	Which region or city contributes the most to total sales?
3.	Who are the top 10 customers by purchase value?
4.	Which products or categories are most profitable?
5.	How do sales vary month-over-month or year-over-year?
6.	What is the sales trend across regions and time periods?
7.	Which regions underperform and need attention?
8.	How does the actual sales compare with targets?

<a href ="https://github.com/kala-99855/sales_insigths_dashboard/blob/main/Screenshot%202025-10-24%20100013.png"> dashboard<a>
## Project Process (Workflow)

Step 1: Data Extraction

•	Connected Power BI to SQL Server database using SQL queries.

•	Imported tables like Customers, Products, Transactions, Regions.

Step 2: Data Cleaning & Transformation


•	Removed duplicates and null values

•	Standardized column names and data types.

•	Created calculated columns (e.g., Total_Sales = Quantity * Unit Price).

Step 3: Data Modeling

•	Built relationships between tables using primary and foreign keys.

o	Example: Customers[Customer_ID] ↔ Transactions[Customer_ID]

•	Used a Star Schema for efficiency.

Step 4: DAX Calculations

•	Created measures for key KPIs using DAX formulas:

o	Total Sales = SUM(Transactions[Sales Amount])

o	Profit Margin = DIVIDE(SUM(Profit), SUM(Sales Amount))

o	Sales Growth = (Current Year Sales - Previous Year Sales) / Previous Year Sales

Step 5: Visualization Design

•	Added charts, maps, and KPI cards for interactive analysis.

•	Applied slicers for filters (Year, Region, Product Category).

Step 6: Dashboard Creation

•	Created multiple pages:

o	Sales Overview Dashboard

o	Regional Performance Dashboard

o	Product Analysis Dashboard

o	Customer Insights Dashboard

## Final Conclusion

The Sales Insights Power BI Dashboard successfully transformed raw SQL Server data into actionable business intelligence.
It provides:

•	A comprehensive view of sales, profit, and customer performance.

•	Identification of high-performing products and regions.

•	Strategic insights to improve marketing and inventory planning.

•	A dynamic and user-friendly interface for decision-makers to explore data visually.

This project demonstrates the integration of SQL-based data analytics and Power BI visualization for real-world business decision-making.

________________________________________

________________________________________

