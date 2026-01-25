# Global Superstore BI Project

End-to-end Business Intelligence project based on the Global Superstore dataset.

This project demonstrates a full BI pipeline:

- raw data ingestion  
- SQL transformations  
- star schema modeling  
- KPI views  
- Power BI dashboarding  

Built as a portfolio project to showcase SQL + Power BI skills.

---

# Architecture

# Data Layer (MySQL)

Database: `global_superstore_bi`

# Tables:

- stg_orders — raw staging table  
- dim_customer  
- dim_product  
- dim_geo  
- dim_shipmode  
- fact_sales  

# Views:

- vw_sales — base analytical view  
- vw_sales_month — monthly aggregation  
- vw_sales_month_total — monthly totals  
- vw_kpi — main KPI view (single row KPIs)  
- vw_kpi_pretty — formatted KPIs for Power BI  


# KPIs Implemented

- Total Sales  
- Total Profit  
- Profit Margin  
- Orders Count  
- Average Discount  
- Average Delivery Days  
- Min / Max Order Date  


# Calendar Table (Power BI DAX)

Custom DAX calendar created in Power BI:

- Date  
- Year  
- Month Number  
- Month Name  
- YearMonth  
- Sort Column  

Used for proper time intelligence and visuals.


# Tools Used

- MySQL 8.0  
- MySQL Workbench  
- Power BI Desktop  
- GitHub  


# Repository Content

/sql  
  global_superstore_bi.sql  

/powerbi  
  global_superstore.pbix  

README.md  


# How to Run

# 1. Restore database

File → Run SQL Script → global_superstore_bi.sql

or

mysql -u root -p < global_superstore_bi.sql

# 2. Open Power BI

Open global_superstore.pbix  
Update MySQL connection if needed.

# Purpose

This project was built as a learning + portfolio project to practice:

- SQL modeling  
- BI architecture  
- KPI logic  
- Power BI visualization  
- Git version control  

# Author

Dmytro Kalaida  
Junior Data / BI Analyst  

GitHub: https://github.com/AM111D
