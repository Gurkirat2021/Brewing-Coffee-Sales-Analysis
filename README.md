🌟 Why I Built This
I didn’t just want to "use" Excel; I wanted to master the story behind the data. This project started as a self-motivated challenge to push myself beyond basic spreadsheets.
I wanted to prove to myself that I could take messy, raw CSV files and transform them into a sleek, professional dashboard. This was my hands-on laboratory for learning how to clean, transform, and visualize data from scratch.
Excel Coffee Sales Dashboard Project
This repository contains the files for an end-to-end Excel project designed to create a dynamic and interactive coffee sales dashboard. This project is ideal for data professionals and job seekers looking to build a robust data portfolio, demonstrating skills in data gathering, transformation, analysis, and visualization using Microsoft Excel.
📊 Project Overview
The project walks through the entire process transforming raw sales data into an interactive, data-driven dashboard. It focuses on solving business problems using data, turning complex information into actionable insights.
🔍 Objectives
The core objective was to move beyond basic data entry and master the art of automated financial analysis, using modern Excel logics to track profitability, customer loyalty, and regional growth I real time.
✨ Features
Dynamic Coffee Sales Dashboard: An interactive dashboard to visualize key sales metrics.
•	Visualization and Aggregation
Total Sales Over Time: Line chart displaying sales trends across different coffee types (Arabica, Excelsa, Libreca, Robusta) and trends across months and years
Sales by Country: Bar chart breaking down sales by geographical region (U.S., Ireland, UK), identifying the primary markets
Top 5 Customers: Bar chart showcasing most valuable individual buyers.
Profitability Analysis: The breakdown of sales between Arabica, Robusta, Libreca, Excelsa. To understand the product preferences.
•	Interactive Controls:
Timeline: Filter data by specific time periods (e.g., years, months).
Slicers: Filter data by 
•	Roast Type (Dark, Light, Medium), 
•	Size (e.g., 0.2kg, 0.5kg), 
•	Loyalty Card status (Yes/No)
📂Dataset Source 
coffeeordersdata.xlsx (via GitHub) Data Format: xlsx imported into Excel worksheet with 3 different sheets in it. Key Columns in each worksheet 
Orders:       • Order ID • Order Date • Customer ID • Product ID • Quantity
Customers • Customer ID • Customer Name • Email • Phone Number • Address Line 1	          •City •Country •Postcode •Loyalty Card
Products    •Product ID •Coffee Type •Roast Type •Size •Unit Price •Price per 100g 
                    •Profit
🛠️ Technologies & Techniques
Microsoft Excel: The primary tool for the entire project.
Data Gathering: 
XLOOKUP/VLOOKUP function used for efficiently retrieving customer information and INDEX MATCH function applied for dynamic lookup of product data.
Data Transformation & Cleaning:
Multiplication formula for Sales calculation., Multiple IF functions for data categorization (e.g., full coffee type names). Date Formatting and Number Formatting for enhanced readability and Duplicate Value Check 
Data Structuring:
Converting Range to Table to ensures dynamic data sources for pivot tables.
Data Analysis & Visualization:
Pivot Tables used to summarize and analyse data. Pivot Charts (Line and Bar charts) for visual representation and inserting Timelines and Slicers for interactive filtering.
🧮 Calculation Logic & Data Modeling
1.	The ‘LOOKUP’ Logic
To maintain a clean and efficient dataset, many attributes in the Orders sheet were pulled dynamically from the Products and Customers tables using VLOOKUP and XLOOKUP.
Name, Email, and Country, Loyalty, Profit were retrieved from the customers and product sheet using Customer_ID and Product_ID.

2.	‘Index Match’ Logic
To dynamically retrieve coffee type, roast type, size, and unit price from the Products table. This formula is "dynamic" because it can be dragged horizontally and vertically to populate multiple columns without modification due to the careful use of absolute and mixed references.

3.	Nested IF Functions:
These are used for Coffee Type Name and Roast Type Name

4.	 Financial Formulas:
Sales Calculation is the total revenue for each order line. 
Sales = Quantity* Unit_Price 
Purchase Price is the cost to the business for the coffee sold.
Purchase Price = Sales – Profit
📂 Project Structure
•	Data/- raw dataset and transformed version.
•	Excel/- Excel Formulas for calculations and Data Modeling
•	Visualizations/- Excel Dashboard screenshots and files.
•	Readme/- Project Documentation

🖥️ Defining the Dashboard
The dashboard was designed to provide a 360-degree view of the business performance using interactive elements. It is divided into three primary functional areas:
1.	Navigation & Interactivity
•	Timeline Slicer: Allows users to filter the entire dashboard by Year and Month to visualize growth patterns.
•	Slicers (Coffee Type, Roast, Size, Loyalty): Enables deep dives into specific product categories.

2.	Visual Components: 
Line Charts, Bar Charts and Horizontal Bar Charts display Total sales over time, sales by country, top 5 customers and profitability analysis. 

3.	 Dynamic Metrics
Used Pivot Tables to summarize over 1,000 rows of order data into clear, digestible totals for Sales and Profit.

💡 Key Insights
After analyzing the data through the dashboard, several business-critical trends emerged:

Market Dominance: The United States is our largest market by a significant margin, contributing over 75% of total revenue. However, Ireland shows a higher percentage of "Loyalty" customers per capita, suggesting a very dedicated niche.

Size Matters: The 2.5kg bags are the most profitable per transaction. While 0.2kg bags have a higher sales volume, the operational efficiency of larger packaging drives the majority of the net profit.

Roast Preferences: Medium Roast is the "crowd-pleaser," performing consistently across all three countries. Conversely, Dark Roast sales are highly concentrated in the UK market.

Loyalty Impact: Customers with Loyalty Cards spend on average 15% more per order than non-members, proving the value of the current rewards program.

🚀 Future Enhancements
This project is a foundation. If I were to take this to "Version 2.0," here is the roadmap:

Power BI Integration: Transition the data model from Excel to Power BI to handle larger datasets and create more advanced DAX measures for Year-Over-Year (YOY) growth.

Customer Churn Analysis: Add a "Last Purchase Date" metric to identify customers who haven't ordered in 6 months and flag them for re-engagement campaigns.

Automated Data Refresh: Set up a Power Query connection to a live folder or API so the dashboard updates automatically when a new month of sales data is added.
