# Readme.md
<img width="1704" height="982" alt="Screenshot 2026-05-26 at 10 18 13 AM" src="https://github.com/user-attachments/assets/a06e605c-d455-47f9-b44c-1dd3cf3df8f2" />



Power BI DashBoard Project


# Overview
This project showcases an interactive and visually
appealing dashboard built using Power BI. 
The dashboard is designed to provide meaningful 
insights through data 
visualization, helping users make data-driven decisions efficiently.

# Features
Interactive and user-friendly dashboard.

Clean and attractive design.

Dynamic filtering and slicing options.

Key performance indicators (KPIs).

Data visualization using charts, graphs, and tables.

Drill-down and drill-through capabilities.

# Tools and Technologies
Power BI Desktop.

Data Modeling.

DAX (Data Analysis Expressions).

Data Visualization Techniques.
 

# Insights Provided
Overview of key metrics.

Trend analysis.

Comparative analysis.

Performance tracking.

# Purpose
The purpose of this project is to demonstrate data 
visualization skills and the ability to transform raw 
data into actionable insights using Power BI.

# Future Improvements
Add more advanced analytics.

Integrate real-time data sources.

Enhance dashboard performance.

# Modeling 
<img width="1686" height="1008" alt="Screenshot 2026-05-26 at 10 19 43 AM" src="https://github.com/user-attachments/assets/d3aaa15b-d1b8-4c30-b89b-f6d0812a491a" />
Power Bi Sales Dashboard

# Overview

This project presents an interactive Power BI dashboard built using a structured data model consisting of fact and dimension tables. The dashboard provides insights into sales performance, product trends, customer behavior, and returns analysis.

The data model follows a star schema design to ensure efficient querying and better performance.

# Data Model

The project is designed using the following tables:

# Fact Tables

1.Sales_Fact
--
 .Contains transactional sales data

 .Includes metrics like Cost, Profit, Quantity

 .Linked with Product, Customer, Region, and Date dimensions

2.Returns_Fact
   --  
 .Contains product return data

 .Tracks returned quantities and related details
 
 .Connected with Product, Region, and Date
 
# Dimension Tables
1.Product_Dim
   -
  .Product details such as ProductID, ProductName, Category, and Cost

2.Customer_Dim
   -
 .Customer information including CustomerID, FullName

3.Region_Dim
   -
 .Regional information including RegionID
and RegionName

4.Date_Dim
-
.Date-related attributes such as Year, 

.Quarter, Month, Day, Weekday

# Relationships

.One-to-many relationships between dimension tables and fact tables

.Centralized fact table (Sales_Fact) connected to all dimensions

.Returns_Fact shares relationships with Product, Region, and Date

.Proper key-based joins using IDs (ProductID, CustomerID, RegionID, Date)

Dax Formulas  
---
<img width="360" height="871" alt="Screenshot 2026-05-26 at 10 16 49 AM" src="https://github.com/user-attachments/assets/2d1e7d5f-a02b-43eb-8138-b340c589c7ef" />
<img width="323" height="783" alt="Screenshot 2026-05-26 at 10 17 22 AM" src="https://github.com/user-attachments/assets/df750c79-ae7e-4b3d-a864-745d57ac9785" />

# Power BI DAX Measures and Calculations

# Overview

This file 
contains DAX measures a
nd calculated columns 
used in the Power BI d
ashboard to analyze sales, 
customers, and returns data.

# Measures Included

# 1.Total Sales:-
Sum of sales amount

# Average Sale:-
Average sales per transaction

# Total Transactions:-
Count of unique sales

# Total Profit & Cost:-
Overall profit and cost calculation

# Quantity:-
Total items sold

# Return Rate:- 
Ratio of returned orders to total sales

# High Sales Metrics:-
Filtered calculations for high-value sales

# Time Intelligence:-
Last Year Sales
Last 3 Months Sales

# Sales Comparison:-
Sales (All Regions)
Sales Difference

# Sales Category:-
Classification (Low, Medium, High)

# Calculated Columns
# Total Revenue: 
SalesAmount × Quantity

# Sales Category: 
Based on revenue thresholds

# Return Flag: 
Returned / Not Returned

# Region Name & Product Category: 
Using relationships

# Customer Transformations:
Full Name

# Functions Used
CALCULATE, SUM, COUNT, DISTINCTCOUNT

FILTER, COUNTROWS, MAX

DIVIDE, SWITCH, IF

RELATED, VALUES

Time Intelligence (TOTALYTD, SAMEPERIODLASTYEAR, DATESINPERIOD)

# Data Transformation
<img width="1710" height="965" alt="Screenshot 2026-05-26 at 10 18 49 AM" src="https://github.com/user-attachments/assets/a5fb2987-d16e-4512-a015-943772ff8c2e" />
<img width="1699" height="1005" alt="Screenshot 2026-05-26 at 10 20 51 AM" src="https://github.com/user-attachments/assets/4bf1d38b-4252-465f-8797-c83066751721" />
<img width="1710" height="1007" alt="Screenshot 2026-05-26 at 10 21 17 AM" src="https://github.com/user-attachments/assets/0c016289-798d-441c-b7c6-90b6d7a9e9aa" />
<img width="1691" height="1011" alt="Screenshot 2026-05-26 at 10 21 50 AM" src="https://github.com/user-attachments/assets/22408202-9eb7-4d04-8a1e-0cba65221427" />
<img width="1679" height="999" alt="Screenshot 2026-05-26 at 10 22 25 AM" src="https://github.com/user-attachments/assets/35ca0786-8995-440a-aac8-5dd64dd013f6" />
<img width="1710" height="1107" alt="Screenshot 2026-05-26 at 10 23 26 AM" src="https://github.com/user-attachments/assets/e48aa5c9-c886-404b-87eb-5feeb75376fd" />
<img width="1710" height="1107" alt="Screenshot 2026-05-26 at 10 23 35 AM" src="https://github.com/user-attachments/assets/46e3effc-71bf-455b-b6af-1dd5e3987427" />

# Power BI Data Transformation (Power Query)

# Overview

This project includes data cleaning and transformation steps performed in Power Query to prepare raw data for analysis in Power BI.

# Tables Processed

Sales_Fact
Returns_Fact
Customer_Dim
Product_Dim
Region_Dim
Date_Dim
Key Transformations

# Data Cleaning

Removed null values from key columns (CustomerID, ProductID, RegionID)
Removed unnecessary columns (DateKey, extra text columns)
Ensured all columns have correct data types
Data Transformation

Renamed columns for better readability
Added custom columns where required
Filtered rows to maintain valid data
Created proper date format (New_Date)
Data Structuring

# Maintained star schema structure
Ensured consistency between fact and dimension tables
Applied indexing where needed
Tools Used

# Power BI Power Query Editor
M Language (Power Query Formula Language)
Purpose

# These transformations ensure:

Clean and reliable dataset
Improved performance of dashboard
Accurate reporting and analysis
Usage

All transformations are applied in Power Query before loading data into the Power BI model.








