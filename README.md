# Databricks Delta Lake Practice – QuickCart Orders

This repository contains a hands-on **Databricks notebook** that demonstrates core **Delta Lake operations** using a realistic e-commerce scenario (QuickCart).

## Scenario

**QuickCart** is a small e-commerce company. Every day, order data arrives as CSV files. The data engineering team needs to:

- Store the data in Delta Lake
- Perform common Delta operations
- Explore table history, time travel, and optimization features

## What is Covered

| Part | Topic | Description |
|------|-------|-------------|
| 1 | Create Delta Table | Read CSV and create a Delta table |
| 2 | INSERT INTO | Append new records |
| 3 | INSERT OVERWRITE | Replace entire table content |
| 4 | UPDATE | Modify existing records |
| 5 | DELETE | Remove records |
| 6 | CTAS | Create table for high-value orders |
| 7 | CREATE OR REPLACE TABLE | Replace table definition/data |
| 8 | Temporary View | Create a temporary view on delivered orders |
| 9 | DESCRIBE EXTENDED / DETAIL | Inspect table metadata |
| 10 | DESCRIBE HISTORY | View table change history |
| 11 | Time Travel | Query data as of a specific version/timestamp |
| 12 | RESTORE TABLE | Restore table to a previous version |
| 13 | OPTIMIZE | Improve physical layout of the Delta table |
| 14 | VACUUM | Clean up old files based on retention |
| 15 | MERGE INTO | Upsert (update + insert) records |
| 16 | SQL UDF | Create a user-defined function for order category |

## Sample Data (`orders.csv`)

```csv
order_id,customer_id,order_date,shipping_city,payment_method,order_status,order_amount
1001,C101,2026-08-10,Ahmedabad,UPI,PLACED,850
1002,C102,2026-08-10,Mumbai,CARD,SHIPPED,1200
...
```

## Technologies Used

- Databricks
- Delta Lake
- Spark SQL

**Delta Lake Features:** Time Travel, OPTIMIZE, VACUUM, MERGE, History, RESTORE, etc.
