# 📊 Financial KPI Dashboard (Power BI)

## 📌 Project Overview

This project presents an **interactive Financial KPI Dashboard** built using **Microsoft Power BI** based on the **Budget vs Actual Financial Dataset**. The dashboard helps management monitor budget performance, analyze spending patterns, track budget utilization, and identify financial variances across departments, categories, regions, and payment methods.

This project was developed as part of the **Data Analytics for Business - Experiment 7** at **Alliance University**.

---

## 🎯 Objective

The objective of this dashboard is to:

* Monitor budget and actual spending
* Track budget variance and utilization
* Analyze department-wise financial performance
* Identify overspending and underspending areas
* Support data-driven financial planning and cost-control decisions

---

## 🛠️ Tools & Technologies

* Microsoft Power BI Desktop
* Microsoft Excel / CSV
* Power Query
* DAX (Data Analysis Expressions)

---

## 📂 Dataset

**Dataset Name:** Budget vs Actual Financial Dataset

**Source:** Academic Dataset for Financial KPI Analysis

---

## 📈 Dashboard Features

### KPI Cards

* Total Budget
* Total Actual
* Budget Variance
* Budget Variance %
* Budget Utilization %

### Interactive Filters

* Date
* Department
* Category
* Region
* Payment Method

### Visualizations

* Actual Spending by Payment Method (Donut Chart)
* Budget vs Actual by Department (Bar Chart)
* Budget Utilization % (Gauge)
* Variance % by Region (Column Chart)
* Budget Utilization % by Category (Column Chart)
* Detailed Budget vs Actual Table

---

## 📊 Key Insights

* Total Budget: **₹795.36M**
* Total Actual Spending: **₹890.03M**
* Budget Variance: **-₹95M**
* Budget Variance %: **-11.89%**
* Budget Utilization: **111.90%**

### Major Findings

* The organization exceeded its allocated budget, resulting in overall overspending.
* Marketing and Sales departments showed comparatively higher actual spending.
* Marketing–Training–East region recorded the highest negative variance.
* Spending distribution across payment methods remains relatively balanced.
* Department-level analysis reveals significant differences in budget utilization and spending efficiency.

---

## 📁 Repository Structure

```text
Financial-KPI-Dashboard/
│
├── Dataset/
│   └── Budget_vs_Actual_Data.xlsx
│
├── Dashboard/
│   └── Financial KPI Dashboard.pbix
│
├── Report/
│   └── Experiment_7_Report.pdf
│
└── README.md
```

---

## 📌 Business Benefits

* Improves budget monitoring and financial transparency
* Helps identify overspending departments and categories
* Supports cost-control initiatives
* Enables faster financial decision-making
* Provides interactive financial performance analysis

---

## 📚 Learning Outcomes

* Data Cleaning using Power Query
* Data Modeling in Power BI
* Creating DAX Measures
* KPI Development
* Financial Analytics Reporting
* Interactive Dashboard Design

---

## 📐 DAX Measures Used

```DAX
Total Budget =
SUM('Budget vs Actual'[Budget Amount])

Total Actual =
SUM('Budget vs Actual'[Actual Amount])

Budget Variance =
[Total Budget] - [Total Actual]

Budget Variance % =
DIVIDE([Budget Variance], [Total Budget], 0)

Budget Utilization % =
DIVIDE([Total Actual], [Total Budget], 0)
```

---

## 👨‍💻 Author

**Priyansh Nolkha**
Master of Computer Applications (MCA)
Alliance University

---
