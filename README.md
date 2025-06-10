# 06_sales-trend-analysis
Sales trend analysis using SQL and SQLite
# 📊 Sales Trend Analysis Using SQL

This project focuses on analyzing monthly sales trends from a simulated online sales dataset using SQL in SQLite.

## 📁 Dataset Overview

The dataset consists of a single table:

### `orders`
| Column Name  | Data Type | Description                          |
|--------------|-----------|--------------------------------------|
| order_id     | INTEGER   | Unique identifier for each order     |
| order_date   | TEXT      | Date the order was placed (YYYY-MM-DD) |
| amount       | INTEGER   | Total amount for the order           |
| product_id   | INTEGER   | ID of the product ordered            |

---
## 🎯 Objective

To analyze sales performance over time by calculating:

- ✅ Monthly total revenue
- ✅ Monthly number of orders
- ✅ Average order value per month

---
## 🛠 Tools & Techniques

- **SQLite** (via SQLiteOnline)
- SQL functions: `SUM()`, `COUNT()`, `ROUND()`, `strftime()`
- Data grouping by month using `strftime('%Y-%m', order_date)`
- Exported result as `.csv`

---
## 📜 SQL Script

The SQL file includes:

- Table creation
- Sample data insertion
- Aggregation query for sales trend

👉 View the full script: [sales_trend_analysis.sql](./sales_trend_analysis.sql)

---

## 📈 Result Table

👉 View the output: [monthly_sales_trend.csv](./monthly_sales_trend.csv)

The table includes:

| Month     | Total Revenue | Total Orders | Average Order Value |
|-----------|----------------|---------------|-----------------------|
| 2023-01   | 1250           | 2             | 625.00                |
| 2023-02   | 1530           | 2             | 765.00                |
| ...       | ...            | ...           | ...                   |

---

## 💡 Key Insights

- 📈 Sales peaked in **October** and **December**, indicating strong Q4 performance.
- 📉 A slight dip in **April** may suggest a seasonal trend.
- 💰 Average order value remained stable, showing consistent pricing or order behavior.

---
## 📌 Conclusion

This SQL-based analysis demonstrates how simple aggregation and grouping functions can help businesses:

- Understand trends over time
- Plan inventory and marketing strategies
- Make data-driven decisions


