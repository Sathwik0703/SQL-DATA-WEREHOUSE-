[SQLDash.pdf](https://github.com/user-attachments/files/23689533/SQLDash.pdf)
<img width="1920" height="1080" alt="Screenshot (170)" src="https://github.com/user-attachments/assets/4a2bbe6b-ae09-463b-a31a-b0b3cd9f9451" />
# SQL-DATA-WHEREHOUSE-
Sales & Customer Analytics – SQL Server + Power BI (Medallion Architecture)

This project takes six CSV files containing customer, product, and sales data and builds a complete analytics pipeline using SQL Server for data engineering and Power BI for visualization.

The goal was to simulate a real-world warehouse setup using the Medallion Architecture (Bronze → Silver → Gold) and create a dashboard that delivers actionable business insights.

📂 Data Sources

Total Files: 6 CSVs

Customer Data (2 files)

Customer details

Customer ID for joining

Product Data (2 files)

Product details

Product ID for joining

Sales Data (2 files)

Transaction-level data

Contains Customer ID and Product ID references

The files together form a relational dataset.

🏗️ Data Pipeline (Medallion Architecture)
1️⃣ Bronze Layer – Raw Data

All CSVs loaded into SQL Server as-is

No transformations

Acts as the raw landing zone

2️⃣ Silver Layer – Cleaned & Standardized Data

Data cleaning performed in SQL:

Handling missing/invalid values

Formatting standardization

Data normalization

Derived columns

Lookup joins using shared keys

Enrichment logic

3️⃣ Gold Layer – Business-Ready Models

Final reporting layer structured as:

Fact Table: Sales

Dimensions: Customers, Products

Implemented using SQL Views

Optimized for downstream analytics and BI tools

🔍 Exploratory Data Analysis (SQL)

EDA and advanced SQL analysis were performed before Power BI import, including:

Trend analysis

Sales breakdowns

Customer segmentation

Product performance

Outlier checks

📊 Power BI Dashboard

The Gold layer was used to build an interactive dashboard showing:

Total Sales

Total Orders

Customer Count

Sales by product, category, and geography

Top products and customers

Gender and country breakdowns

Filters allow drilldowns and exploration from multiple angles.

🗂️ Repository Contents

/data – All 6 original CSV files

/sql – Scripts for:

Bronze Load

Silver Transformations

Gold Views

EDA queries

/powerbi – Power BI dashboard (.pbix)

/images – Architecture diagram & dashboard screenshots

🚀 Tech Stack

SQL Server – Data storage, cleaning, modeling

Power BI – Visualization and reporting

CSV Files – Raw data source

📌 Project Highlights

Real relational dataset with connected keys

Fully implemented Medallion Architecture

SQL-based cleaning, transformation, and modeling

Professional dashboard built from structured warehouse data

End-to-end pipeline similar to real enterprise data workflows
