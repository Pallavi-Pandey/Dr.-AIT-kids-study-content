# Sales Trend Analysis

> **Learning Goal:** Learn how to spot patterns, seasonality, and growth in time-series retail data to make better predictions.

---

##  Why Time Series Analysis?

In retail, a single number (Total Sales) is a snapshot. **Trend Analysis** is the movie. It tells you where the business is heading.

---

## 1. Seasonality: The "Pulse" of Retail

**What**: Repeating patterns in sales data over a specific period.
**Why**: Helps in stock planning and staffing.

- **Weekly Seasonality**: Sales peak on Saturdays/Sundays (Friday is the "prep" day).
- **Monthly Seasonality**: Spikes around the 1st-5th (Salary day).
- **Annual Seasonality**: Huge spikes during Festivals (Diwali, New Year) or End-of-Season sales.

---

## 2. Moving Averages: Removing the "Noise"

**What**: Averaging data points over a sliding window (e.g., 7 days).
**Why**: Real data is "noisy" (zig-zags). Moving averages smooth the line to show the real trend.

**How it works**:
- Day 1-7 Average -> Point 1
- Day 2-8 Average -> Point 2
- Day 3-9 Average -> Point 3

```python
# Pandas Example
df['7day_rolling_avg'] = df['amount'].rolling(window=7).mean()
```

---

##  The Inventory Trap (Case Study)

**Where** trends go wrong:
Imagine you see a huge spike in 'Electronics' sales in October.
- **Wrong Conclusion**: "People suddenly love electronics more. Let's order 2x more stock for November."
- **Data Reality**: October was Diwali season. Sales will naturally drop in November.
- **Result of Wrong Conclusion**: Overstocking and lost money.

**Lesson**: Always compare this month's growth to **last year's same month** (Year-over-Year / YoY) instead of just last month.

---

##  Brainstorming Exercise

Look at a chart with a 15% dip in sales during the 15th-20th of every month.
1. **What is happening?** (Insight: People have less cash before next salary).
2. **How to fix it?** (Decision: Offer "Mid-month Budget Deals" or small EMI options).

---

##  Quick Check Questions

1. What is the difference between a "Trend" and "Seasonality"?
2. Why is a 7-day moving average better than a 2-day moving average for retail?
3. If sales were Rs. 10,000 in August and Rs. 12,000 in September, what is the Month-over-Month (MoM) growth percentage?

---

[Previous](01_KPI_Identification.md) | [Home](../../README.md) | [Next](03_Customer_Insights.md)