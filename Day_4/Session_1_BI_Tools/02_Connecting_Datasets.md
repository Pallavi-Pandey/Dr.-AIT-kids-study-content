# Connecting Datasets in BI Tools

> **Learning Goal:** Learn how to bring your SQL and Python results into a BI environment reliably.

---

## Methods of Connection (How)

BI tools are useless without data. There are two main ways to connect:

### 1. Static Files (CSV / Excel)
- **Use**: For one-off projects or simple labs.
- **Process**: `Get Data` -> `Text/CSV` -> `Select File`.
- **Note**: You must manually "Refresh" if the file changes.

### 2. Live Database Connection (SQL)
- **Use**: Professional industry standard.
- **Process**: `Get Data` -> `SQL Server` / `SQLite`.
- **Why**: The dashboard updates automatically as new sales happen.

---

## Data Cleaning (Power Query / Tableau Prep)

Before building charts, you must ensure the data is "Healthly." Both tools have a built-in cleaning engine.

**Common Cleaning Tasks**:
- **Promote Headers**: Making the first row the column names.
- **Change Types**: Ensuring 'Date' isn't being read as 'Text'.
- **Filtering**: Removing unwanted years or categories to speed up the report.

---

## Industry Tip: The "Clean at Source" Rule

**Where to clean?**
- If you can fix a data issue using a **SQL Query** before it hits the BI tool, do it! 
- Pre-cleaning in SQL or Python makes your final dashboard run much faster.

---

## Practice Task

Imagine you have a CSV with a column `order_amount` that contains symbols like "$". 
1. How would you handle this in a BI tool? 
2. Why can't you build a Sum chart until it's fixed?

---

[Previous](01_Intro_to_BI_Tools.md) | [Home](../../../README.md) | [Next](03_Data_Modeling_Basics.md)
