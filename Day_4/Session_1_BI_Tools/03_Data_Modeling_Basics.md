# Data Modeling Basics

> **Learning Goal:** Understand how multiple tables talk to each other inside a BI tool to create a "Single Source of Truth."

---

## What is a Data Model? (What & Why)

**What**: A data model is a map of how different tables (Sales, Products, Stores) are connected using shared IDs.
**Why**: Without a model, you can't see "Total Sales" filtered by "Store Manager" if those two bits of data live in different tables.

---

## The Star Schema (The Industry Standard)

Imagine a star. The **Fact Table** is in the center, and **Dimension Tables** are the points.

1. **Fact Table (The "Verb")**: Stores events. (e.g., `Sales_Table`  million rows of transactions).
2. **Dimension Tables (The "Nouns")**: Stores details. (e.g., `Product_Table`, `Location_Table`).

---

##  How it looks in your project

- **Fact**: `transactions.csv` (contains amount, txn_id, store_id).
- **Dimension**: `stores_lookup.csv` (contains store_id, manager_name, city).

**The Relationship**: You link them on `store_id`. This is called a **One-to-Many** relationship (One store has many transactions).

---

## Logic in BI Tools (DAX & LOD)

Sometimes, you need to calculate new data that isn't in your table.
- **Power BI uses DAX**: `Revenue Growth = [Total Sales] - [Sales Last Year]`
- **Tableau uses Calculated Fields**: `IF [Profit] > 0 THEN 'Gain' ELSE 'Loss' END`

---

##  Quick Check Questions

1. What is the difference between a "Fact" and a "Dimension"?
2. Why is the "Star Schema" preferred over one giant single table?
3. In a school database, would 'Student Names' be a Fact or a Dimension?

---

[Previous](02_Connecting_Datasets.md) | [Home](../../../README.md) | [Next](../Session_2_Dashboard_Building/01_Visual_Components.md)
