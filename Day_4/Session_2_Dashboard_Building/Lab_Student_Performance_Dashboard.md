# Lab: Student Performance Dashboard

> **Objective:** Build a professional dashboard to help a school principal identify struggling students and top performers.

---

##  Requirements & Setup

1. **The Dataset**: Use `student_marks.csv` (generated in Day 2).
2. **Tools**: Power BI Desktop or Tableau Public.

---

##  Step-by-Step Instructions

### Step 1: Data Ingestion
- Open your BI tool.
- Click `Get Data` -> `Text/CSV`.
- Load your student dataset.
- **Transform**: Ensure 'Marks' is a Number and 'Date' is a Date.

### Step 2: Create KPI Cards
Place 3 KPI cards at the very top:
- **Total Students**: `Count of Student_ID`.
- **Average Marks**: `Average of Marks`.
- **Passing Rate**: (Calculated field: `Students with Marks > 40 / Total Students`).

### Step 3: Performance Distribution
- Create a **Histogram** (or Bar Chart) showing the number of students in different mark ranges (0-40, 41-70, 71-100).
- **Insight**: This shows at a glance if the class is doing well overall.

### Step 4: Add Interactivity (Slicers)
- Add a **Slicer** for `Subject`.
- Add a **Slicer** for `Grade/Class`.
- **Test**: Click 'Maths'  do the KPI cards and charts update?

### Step 5: The "Watchlist" Table
- At the bottom, add a **Table** showing: `Student Name`, `Marks`, and `Attendance`.
- Apply a **Conditional Formatting** rule: Color the 'Marks' cell RED if it is below 40.

---

##  Challenge Task
Add a **Trend Line** at the side which shows if the class average is going UP or DOWN across different test dates.

---

##  Submission
Save your dashboard as a `.pbix` or `.twbx` file and take a screenshot for your Capstone planning.

---

[Previous](02_Interactive_Reports.md) | [Home](../../../README.md) | [Next](../Session_3_Capstone_Initiation/01_Capstone_Overview.md)
