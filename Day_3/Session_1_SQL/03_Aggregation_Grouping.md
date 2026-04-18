# Aggregation & Grouping in SQL

> **Learning Goal:** Learn how to summarize millions of rows into meaningful business insights using aggregate functions and the GROUP BY clause.

---

## 1. Aggregate Functions

**What**: Functions that perform a calculation on a group of values and return a single result.

| Function | What it calculates | Business Question |
|----------|-------------------|-------------------|
| `SUM()` | Total of a column | What is our total revenue? |
| `AVG()` | Average of a column | What is the average order value (AOV)? |
| `COUNT()` | Number of rows | How many orders did we get today? |
| `MAX()` / `MIN()` | High / Low | What was our most expensive sale? |

---

## 2. GROUP BY: The Secret Sauce

**What**: It groups rows that have the same values into summary rows (like "total revenue by City").
**Why**: This is how you transition from "Row-level data" to "Executive-level insights."

```sql
-- Revenue by Store
SELECT store, SUM(amount) AS store_revenue
FROM transactions
GROUP BY store
ORDER BY store_revenue DESC;
```

---

## 3. HAVING: Filtering the Groups

**What**: Like a `WHERE` clause, but it works on the **grouped result**.
**Why**: Use it to find "Outlier categories" (e.g., "Find cities with more than 1,000 orders").

```sql
SELECT category, COUNT(*) as order_count
FROM transactions
GROUP BY category
HAVING order_count > 500;
```

---

##  Case Study: Identifying Seasonal Dip

**Business Problem**: You suspect sales are dropping. You want to see total revenue per month to confirm.

```sql
SELECT month, SUM(amount) as monthly_total
FROM transactions
GROUP BY month
ORDER BY monthly_total ASC; -- Lowest sales months first
```

---

##  Quick Check Questions

1. What is the difference between `COUNT(*)` and `COUNT(discount_code)`? (Hint: Think about NULLs).
2. Write a query to find the average `items_count` per `payment_method`.
3. When do you use `HAVING` instead of `WHERE`?

---

[Previous](02_Basic_Queries.md) | [Home](../../README.md) | [Next](04_SQL_Joins.md)