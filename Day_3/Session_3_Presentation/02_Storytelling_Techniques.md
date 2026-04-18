# Visual Narrative Techniques

> **Learning Goal:** Learn how to design visualizations that communicate clearly and avoid common traps that confuse the audience.

---

##  Rule 1: Increase the Data-Ink Ratio

Edward Tufte proposed this rule: **Remove everything that isn't necessary.**

- **What**: Gridlines, background colors, 3D effects, and excessive decimal points.
- **Why**: These "distract" the brain from seeing the actual data points.
- **How**: Remove the default grid in Matplotlib using `plt.grid(False)`.

---

##  Rule 2: Color is a Tool, Not a Decoration

- **What**: Color should be used to highlight, not just look "pretty."
- **Why**: Our eyes seek out contrast. If everything is colorful, nothing stands out.
- **The "Grey-to-Color" Strategy**: Make all bars grey, and color ONLY the one you want the audience to focus on (e.g., "Our Store").

---

##  Rule 3: Choosing the Right Chart

| Use Case | Best Chart | Why? |
|----------|------------|------|
| **Trends over time** | Line Chart | Shows directionality clearly. |
| **Comparing categories** | Bar Chart | Easiest for the brain to compare heights. |
| **Distribution** | Histogram / KDE | Shows where most data "clumps." |
| **Part-to-Whole** | Treemap / Stacked Bar | Better than Pies for comparing small slices. |

---

##  Common Visualization Traps

1. **The Truncated Y-Axis**: Starting your axis at 80 instead of 0 to make a 2% change look like 50%. **Always start at 0** for bar charts.
2. **Dual Axes**: Putting Sales (Rs.) and Satisfaction (1-5) on the same chart. Its almost always confusing. Try two charts side-by-side.

---

##  The Visual Audit Checklist

Before you put a chart in a presentation, ask:
- [ ] Can an 8-year-old understand what this chart is saying in 5 seconds?
- [ ] Did I use the color Red for a good thing (bad) or Green for a bad thing (confusing)?
- [ ] Is my title an "Insight" (e.g., "Sales Up 10%") or just a label (e.g., "Monthly Sales")?

---

##  Quick Check Questions

1. When is a Pie Chart better than a Bar Chart? (Hint: Almost never, but think about very few categories).
2. What does "Data-Ink Ratio" mean in simple terms?
3. Why shouldn't you use 3D effects on your bar charts?

---

*End of Day 3  Congratulations! You have mastered the chain of Data -> Cleaning -> Analysis -> Visualization -> SQL -> Storytelling.*

---

[Previous](01_Insights_to_Decisions.md) | [Home](../../README.md)