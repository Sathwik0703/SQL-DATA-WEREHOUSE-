[SQLDash.pdf](https://github.com/user-attachments/files/23689533/SQLDash.pdf)
<img width="1920" height="1080" alt="Screenshot (170)" src="https://github.com/user-attachments/assets/4a2bbe6b-ae09-463b-a31a-b0b3cd9f9451" />
# SQL-DATA-WHEREHOUSE-
Sales & Customer Analytics – SQL Server + Power BI (Medallion Architecture)
📊 Sales & Customer Analytics | End-to-End Data Pipeline

Tools: SQL Server, Power BI
Architecture: Medallion Architecture (Bronze–Silver–Gold), Star Schema

📌 Project Overview

This project is an end-to-end data analytics solution built to transform raw transactional data into actionable business insights. It integrates multiple customer, product, and sales data sources, applies industry-standard data warehousing practices, and delivers an interactive Power BI dashboard for sales and customer analysis.

The solution enables stakeholders to track KPIs, understand customer behavior, identify revenue drivers, and make data-driven decisions to improve profitability.

🎯 Business Objective

Consolidate data from multiple source systems into a single analytical platform

Ensure data quality, historical tracking, and scalability using proper warehouse design

Analyze sales performance, customer distribution, and product contribution

Identify opportunities for revenue growth, customer retention, and inventory optimization

🗂️ Data Sources

The project integrates 6 structured data sources:

Customer Master

Customer Demographics

Customer Geography

Product Master

Product Category

Sales Orders

🏗️ Data Architecture – Medallion Architecture
🔹 Bronze Layer (Raw Data)

Ingested raw data from all source systems into SQL Server

No transformations applied

Maintained full auditability and reprocessing capability

🔹 Silver Layer (Cleaned & Transformed Data)

Performed ETL operations including:

Data cleaning, trimming, and deduplication

Standardization of gender and marital status codes

Date format normalization

Integration of customer tables into a single customer dataset

Integration of product master and product category into a unified product dataset

Implemented Slowly Changing Dimension (SCD Type-2) to track historical product price changes

🔹 Gold Layer (Analytics-Ready Data)

Designed a Star Schema optimized for reporting

Created:

dim_customer

dim_product

dim_date

fact_sales

Used surrogate keys and enforced relationships

Optimized model for Power BI performance

📐 Data Modeling

Dimensional modeling with clearly defined grain at sales order level

Separation of descriptive attributes (dimensions) and measures (fact table)

Time-based analysis enabled using a comprehensive date dimension

📊 Power BI Dashboard Features
🔑 Key KPIs

Total Sales: 29M

Total Orders: 28K

Total Customers: 18K

Total Products: 295

Total Quantity Sold: 60K

Average Product Price: 486

📈 Visual Analysis

Customer segmentation by gender and country

Product distribution by category

Top customers by total sales

Top-selling products by revenue

Category-wise sales contribution

Interactive date slicer for time-based filtering

🔍 Key Insights

The business generated 29M in sales from 28K orders, indicating strong transaction volume

The United States is the primary revenue-generating market

Customer base is evenly split by gender (~50/50), indicating broad market reach

Bikes contribute ~98.8% of total revenue, making them the core business driver

A small group of top customers contributes ~8K+ sales per customer, highlighting high-value customers

💡 Business Recommendations

Revenue Diversification: Cross-sell accessories and components with bikes to increase average order value

Customer Retention: Introduce loyalty programs targeting high-value customers

Inventory Optimization: Prioritize stock planning for top-selling bike models

Market Expansion: Apply successful US sales strategies to other high-potential regions

Pricing Strategy: Use historical pricing data to optimize prices for high-demand products

✅ Outcome

This project demonstrates complete ownership of the data analytics lifecycle—from raw data ingestion and warehouse design to advanced analytics and visualization. It reflects real-world data engineering and analytics practices and showcases strong skills in SQL, ETL, dimensional modeling, and Power BI.

📌 Skills Demonstrated

SQL Server (ETL, Data Warehousing, Star Schema, SCD Type-2)

Medallion Architecture (Bronze, Silver, Gold)

Power BI (Data Modeling, DAX, Dashboard Design)

Business Analysis & Insight Generation
