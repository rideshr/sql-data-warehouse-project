# SQL Data Warehouse Project

This project demonstrates the implementation of **data warehouse data modeling using SQL**.  
It focuses on creating staging tables, transforming raw data, and building analytical tables using SQL queries.

The project showcases fundamental **data warehousing concepts such as staging layers, transformations, and dimensional modeling**.

---

## 📌 Project Overview

The goal of this project is to transform raw data into a structured format suitable for analytics by:

- Creating staging tables
- Cleaning and transforming data
- Implementing dimensional data models
- Building fact and dimension tables

---

## ⚙️ Technologies Used

- SQL
- SQL Server
- Git & GitHub

---

## 📂 Project Structure

```
sql-data-warehouse-project
│
├── datasets
│   ├── crm_data
│   └── erp_data
│
├── sql
│   ├── staging
│   ├── transformations
│   └── data_models
│
└── README.md
```

---

## 📊 Data Modeling

The project demonstrates **dimensional modeling techniques** using SQL.

Example tables:

**Fact Tables**
- fact_sales
- fact_orders

**Dimension Tables**
- dim_customer
- dim_product
- dim_date

---
## Example Query

```sql
SELECT
    c.customer_name,
    SUM(f.sales_amount) AS total_sales
FROM fact_sales f
JOIN dim_customer c
ON f.customer_id = c.customer_id
GROUP BY c.customer_name;
```

## 🎯 Key Learnings

- Data warehouse fundamentals
- Writing SQL for data transformations
- Implementing dimensional models
- Structuring analytical datasets
