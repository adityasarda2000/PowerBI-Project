Sales Insights Dashboard - Power BI Project
1. Project Overview
This project analyzes and visualizes company sales performance using Power BI. The dashboard provides insights into revenue trends, sales quantities, top-performing products, key customers, and regional sales distribution.

Key Business Questions Addressed:
What are the sales trends over time?
Who are the top-performing customers?
Which products generate the most revenue?
How does revenue vary across different markets?
What is the total sales revenue and quantity?
2. Data Extraction & Sources
Data Pipeline Overview
Data Source: The dataset originates from a MySQL database, serving as the central repository for all sales-related data.
Data Transformation: All Power Queries were executed directly in MySQL and within PowerBi using SQL queries for data cleaning, aggregation, and transformation.
Export to Power BI: The processed data was exported from MySQL as structured tables and imported into Power BI for visualization.
Datasets Used
Dataset Name	Columns	Rows	Description
Revenue_YOY	Revenue, cy_date	33	Revenue trends over time
Top_5_Products	Revenue, product_code	5	Top 5 revenue-generating products
Top_5_Customers	custmer_name, Revenue	5	Top 5 revenue-generating customers
Dates	cy_date	37	Reference table for dates
Years	year	4	Distinct years in the dataset
Revenue	Revenue	1	Total revenue summary
SalesQty	Sales Qty	1	Total sales quantity summary
Revenue_by_Markets	Revenue, markets_name	14	Revenue distribution across markets
Sales_Qty_by_Markets	Sales Qty, markets_name	14	Sales quantity distribution across markets
3. Tools & Technologies Used
Power BI – Interactive dashboard visualization.
MySQL Database – Primary data storage and transformation platform.
SQL Queries & Power Queries – Data extraction, cleaning, and transformation within MySQL.
DAX (Data Analysis Expressions) – Custom calculations and measures in Power BI.
Power Query (within MySQL) – Pre-processing and structuring of data before export to Power BI.
4. Data Model & Relationships
The data follows a dimensional model, optimized for efficient analysis:

Fact Tables:
Revenue_YOY, Revenue_by_Markets, Sales_Qty_by_Markets
Dimension Tables:
Top_5_Customers, Top_5_Products, Dates, Years
Key Relationships:
Dates Table ↔ Revenue Tables (using cy_date)
Markets Table ↔ Revenue & Sales Tables (using markets_name)
Customers & Products ↔ Revenue Tables (using customer_name, product_code)
5. Key Insights from the Dashboard
1️⃣ Year-over-Year Revenue Trends
Revenue trends fluctuate over time, showing seasonal patterns.
The highest revenue months correspond to major sales cycles.
2️⃣ Top 5 Products by Revenue
The top-performing products generate a significant portion of total revenue.
A few key products dominate sales, emphasizing product concentration.
3️⃣ Top 5 Customers
A small number of customers contribute heavily to overall revenue.
The dataset shows a mix of high-volume bulk buyers and frequent customers.
4️⃣ Market-Wise Revenue & Sales Distribution
Revenue varies significantly across markets, with some outperforming others.
Some regions consistently lead in both revenue and sales volume.
6. How to Use the Dashboard
Navigation: Use filters (date, product, customer, and market) for focused insights.
Interactivity: Hover over graphs for detailed tooltips and click to drill down.

