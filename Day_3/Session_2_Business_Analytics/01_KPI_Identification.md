# KPI Identification in Retail

> **Learning Goal:** Learn how to translate raw data into "Key Performance Indicators" (KPIs) that business leaders use to steer a company.

---

##  What is a KPI?

A **Key Performance Indicator (KPI)** is a measurable value that demonstrates how effectively a company is achieving key business objectives. 

Think of a KPI like a **car's dashboard**:
- **Data**: The amount of fuel left (e.g., 5 Liters).
- **KPI**: "Distance to Empty" (e.g., 50km)  this is what tells you when to stop and refuel.

---

##  Top Retail KPIs

### 1. Total Revenue (The North Star)
- **What**: The total money brought in by sales.
- **Why**: It tells you the size of your business and overall growth.
- **Formula**: `total_revenue = df['amount'].sum()`

### 2. Average Order Value (AOV)
- **What**: The average amount spent by a customer per transaction.
- **Why**: Increasing AOV is often easier than finding new customers.
- **How**: `aov = total_revenue / total_transactions`
- **Where**: Use this to decide if you should bundle products (e.g., "Buy 2 Get 1").

### 3. Conversion Rate
- **What**: The % of visitors who actually made a purchase.
- **Why**: High traffic with low conversion means your website/store layout is confusing or prices are too high.
- **How**: `(Purchases / Total Visitors) * 100`

### 4. Churn Rate (Customer Loss)
- **What**: The percentage of customers who stop buying from you.
- **Why**: Its 5x more expensive to acquire a new customer than to keep an old one.
- **Where**: High churn in a specific city might mean a competitor has opened there.

---

##  Actionable vs. Vanity Metrics

| Metric Type | Example | Why it matters |
|-------------|---------|----------------|
| **Vanity** | Total App Downloads | Looks good on paper, but doesn't guarantee profit. |
| **Actionable** | Active Users per Day | Tells you if people are actually getting value. |

---

##  Practice Scenarios (The "So What?" Test)

Try to identify the problem and a possible solution for these scenarios:

1. **Scenario**: Your Revenue is UP, but your AOV is DOWN.
   - **Insight**: Many people are buying, but they are only buying cheap items.
   - **Action**: Launch a "Free Shipping over Rs. 1000" offer to push them to spend more.

2. **Scenario**: Your Traffic is UP, but your Conversion Rate is DOWN.
   - **Insight**: People are looking at your products but not buying.
   - **Action**: Check if your competitors have lower prices or if your checkout page is broken.

---

##  Quick Check Questions

1. If you have Rs. 50,000 revenue from 200 orders, what is your AOV?
2. Why is "Total Visits" considered a Vanity Metric if not compared with Conversion?
3. How would you use SQL to calculate the Average Order Value per City?

---

[Previous](../../Day_2/Session_3_Advanced_Visualization/03_Interactive_Visual_Insights.md) | [Home](../../README.md) | [Next](02_Sales_Trend_Analysis.md)