# Visual Components: Filters, Slicers & KPIs

> **Learning Goal:** Learn how to build the "Interactive" parts of a dashboard that allow users to explore data themselves.

---

## 1. Slicers: The User's Remote Control

**What**: A slicer is a visual filter on the canvas (e.g., a dropdown list of Cities or a Date slider).
**Why**: It empowers the user to answer their own questions. Instead of building 10 charts for 10 cities, you build ONE chart and add a City Slicer.
**Best Practice**: Keep slicers at the **Top** or **Left** of the page so they are easy to find.

---

## 2. KPI Cards: The Big Numbers

**What**: Large, single-value displays (e.g., "Total Profit: $5M").
**Why**: These are the first things an executive looks at. They provide an instant "Health Check" of the business.
**How**: Drag a numeric field (like `Revenue`) into a 'Card' visual and set it to `Sum`.

---

## 3. Filters: Behind the Scenes

Unlike Slicers, Filters are often hidden from the user.

- **Page-Level Filters**: Filters every chart on the page (e.g., "Only show data for 2023").
- **Visual-Level Filters**: Filters ONLY that specific chart (e.g., A bar chart showing "Top 5 products only").

---

##  The "Drill-Down" Concept

**What**: The ability to click a visual and see more detail.
- **Example**: Click on "Category: Clothing" -> The chart changes to show "Jeans, T-shirts, Jackets."
**Why**: Prevents overwhelming the user with too much data at once.

---

##  Quick Check Questions

1. What is the main difference between a Slicer and a Page Filter?
2. Why should a KPI card be big and bold?
3. How does a "Drill-Down" help in following the "Storytelling" rules we learned on Day 3?

---

[Previous](../Session_1_BI_Tools/03_Data_Modeling_Basics.md) | [Home](../../../README.md) | [Next](02_Interactive_Reports.md)
