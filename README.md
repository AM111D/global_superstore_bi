#  Global Superstore BI Project

End-to-end Business Intelligence project based on the **Global Superstore** dataset.

This project demonstrates a full BI pipeline:
- raw data ingestion
- SQL transformations
- star schema modeling
- KPI views
- Power BI dashboarding

Built as a **portfolio project** to showcase **SQL + Power BI** skills.

---

##  Architecture

### Data Layer (MySQL)

**Database:** `global_superstore_bi`

### Tables
- `stg_orders` — raw staging table  
- `dim_customer`  
- `dim_product`  
- `dim_geo`  
- `dim_shipmode`  
- `fact_sales`  

### Views
- `vw_sales` — base analytical view  
- `vw_sales_month` — monthly aggregation  
- `vw_sales_month_total` — monthly totals  
- `vw_kpi` — main KPI view (single-row KPIs)  
- `vw_kpi_pretty` — formatted KPIs for Power BI  

---

## KPIs Implemented

- Total Sales  
- Total Profit  
- Profit Margin  
- Orders Count  
- Average Discount  
- Average Delivery Days  
- Min Order Date  
- Max Order Date  

---

## Calendar Table (Power BI – DAX)

A custom DAX calendar table was created in Power BI:
- Date  
- Year  
- Month Number  
- Month Name  
- YearMonth  
- Sort Column  

Used for proper time intelligence and clean visuals.

---

## Tools Used

- MySQL 8.0  
- MySQL Workbench  
- Power BI Desktop  
- Git & GitHub  

---

## Repository Structure

```
global_superstore_bi/
│
├── sql/
│   └── global_superstore_bi.sql
│
├── powerbi/
│   └── global_superstore.pbix
│
└── README.md
```

---

## How to Run

### 1. Restore database

Using MySQL Workbench:
```
File → Run SQL Script → global_superstore_bi.sql
```

Or via terminal:
```
mysql -u root -p < global_superstore_bi.sql
```

---

### 2. Open Power BI

Open `global_superstore.pbix`  
Update MySQL connection settings if required.

---

## Project Purpose

This project was built as a **learning and portfolio project** to practice:
- SQL data modeling  
- BI architecture  
- KPI logic  
- Power BI visualization  
- Git version control  

---

## Author

**Dmytro Kalaida**  
Junior Data / BI Analyst  

GitHub: https://github.com/AM111D
