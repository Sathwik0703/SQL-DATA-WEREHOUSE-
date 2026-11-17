[SQLDash.pdf](https://github.com/user-attachments/files/23689533/SQLDash.pdf)
<img width="1920" height="1080" alt="Screenshot (170)" src="https://github.com/user-attachments/assets/4a2bbe6b-ae09-463b-a31a-b0b3cd9f9451" />
# SQL-DATA-WHEREHOUSE-
Sales & Customer Analytics – SQL Server + Power BI (Medallion Architecture)
# SQL Data Analytics Project

## Overview
End-to-end analytics pipeline using Medallion Architecture (Bronze → Silver → Gold)
on the AdventureWorks sales dataset, with an interactive Power BI report.

## Dataset
- **Source:** AdventureWorks (AdventureWorksDW)
- **Period:** Dec 2010 – Jan 2014
- **Scale:** 27,659 orders | 60,423 units | 18,484 customers | 295 products | ~$29.4M revenue

## Architecture  
Raw CRM/ERP → Bronze (raw) → Silver (cleaned) → Gold (aggregated) → Power BI


## How to Run
1. Create a SQL Server / Postgres instance
2. Run scripts in order: `01_bronze` → `02_silver` → `03_gold` → `04_analysis`
3. Connect Power BI to Gold-layer tables
4. Open `powerbi/AdventureWorks_Report.pbix`

## Key Insights
- Top 5 products (Mountain-200) each generate ~$1.3M
- 56% of products (165/295) have zero sales
- VIP customers (small %) drive majority of revenue
- Clear seasonal peaks in monthly sales

## Tech Stack
- SQL (Window Functions, CTEs, Subqueries)
- Power BI (DAX, Data Modeling)
- Medallion Architecture

 
