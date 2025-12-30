# Pizza Sales Analysis (SQL)

## 1. Project Overview

This project analyzes sales data for a fictional pizza restaurant using SQL.

The goal is to answer practical business questions such as:

- How much revenue are we making?
- How many pizzas do we sell per order?
- Which days and months are busiest?
- Which pizza categories, sizes and individual pizzas perform best or worst?

All analysis is done in SQL on a single table: `pizza_sales`.

---

## 2. Dataset

All queries use the table `pizza_sales`, which includes at least the following columns:

- `order_id` – unique ID for each order  
- `order_date` – date of the order  
- `pizza_name` – name of the pizza  
- `pizza_category` – category (e.g. Classic, Supreme, Veggie, etc.)  
- `pizza_size` – size (e.g. S, M, L, XL)  
- `quantity` – number of pizzas in each order line  
- `total_price` – total price for that order line  

---

## 3. Key Performance Indicators (KPIs)

### 3.1 Total Revenue

Total revenue generated from all pizza sales:

```sql
SELECT SUM(total_price) AS Total_Revenue
FROM pizza_sales;


