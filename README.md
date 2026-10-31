# Week 1 Assignment: E-Commerce Data Cleaning and Sales Analysis

## Project Title
E-Commerce Data Cleaning and Sales Analysis

## Objective
Clean an e-commerce dataset, calculate core sales KPIs, analyse sales trends and customer behaviour, and present the findings with clear visuals and a report.

## Dataset
Olist Brazilian E-Commerce Public Dataset (Kaggle). Five tables were used: orders, order items, products, customers and payments. Amounts are in Brazilian Real (BRL).

## Tools and Libraries
Python, pandas, numpy, matplotlib, seaborn, Jupyter Notebook (VS Code).

## Key Steps
1. **Data cleaning:** inspected the raw tables, reported missing values, checked duplicates, validated prices, dates and statuses, and saved cleaned files separately.
2. **Sales analysis:** calculated KPIs on delivered orders, analysed monthly trends, regions and customer behaviour.
3. **Visualization:** created a bar chart, a line chart, a pie chart and a dashboard mockup.
4. **Report:** summarised the work in `reports/final_report.pdf`.
5. **Power BI dashboard:** a second version of the dashboard, built from `data/cleaned/sales_cleaned_merged.csv`, is in `outputs/dashboard/` (`olist_dashboard.pdf`).

## Major Findings
- Delivered orders generated 13,221,498.11 BRL from 96,478 orders (average order value 137.04 BRL).
- Revenue peaked in November 2017 (987,765.37 BRL), then levelled off in 2018.
- SP, RJ and MG generated 63.38% of revenue.
- Only 3.0% of customers ordered more than once, so retention is low.
- Credit cards made up 78.5% of payment value.

## Assumptions
- Revenue counts delivered orders only and excludes freight.
- The dataset has no quantity column, so each order-item row is counted as one unit.
- Product IDs are used because product names are not available.

## Folder Structure
```
data-science-week1-assignment/
├── data/
│   ├── raw/
│   └── cleaned/
├── notebooks/
│   └── week1_analysis.ipynb
├── outputs/
│   ├── charts/
│   └── dashboard/
├── reports/
│   └── final_report.pdf
├── screenshots/
├── README.md
└── requirements.txt
```

## Execution Instructions (How to Run)
1. Install the packages: `pip install -r requirements.txt`
2. Open `notebooks/week1_analysis.ipynb` in VS Code or Jupyter.
3. Select **Restart**, then **Run All**. The notebook reads from `data/raw/` and writes to `data/cleaned/` and `outputs/`.

## Author Details
**Author:** Snehal Subhash Mali

**Programme:** WeIntern Data Science Internship, Week 1