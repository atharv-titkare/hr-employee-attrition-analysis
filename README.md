# HR Employee Attrition Analysis

Analysis of 1,470 employee records to understand who leaves the company and why, using Python, MySQL and Power BI.

## Tools
Python (Pandas, Matplotlib, Seaborn) | MySQL (CTEs, window functions, views) | Power BI

## Key findings
- Overall attrition rate: **16.12%**
- Overtime is a major factor: **30.5%** attrition with overtime vs **10.4%** without
- Highest-risk groups: Sales Representatives (**39.8%**), single employees (**25.5%**), frequent travellers (**24.9%**)

## What I did
1. **EDA (Python):** distributions, outliers and attrition split by department, job role, overtime, marital status and travel
2. **SQL analysis (MySQL):** 24 queries incl. CTEs, `RANK`, `NTILE`, `PERCENT_RANK`, subqueries; attrition by department, tenure band and income decile
3. **Risk score:** rule-based attrition risk score (overtime, tenure, work-life balance) listing the top 50 high-risk employees
4. **SQL view:** `department_joblevel_summary` (employees, leavers, attrition rate, avg income)
5. **Dashboard (Power BI):** interactive dashboard of the results

## Dataset
IBM HR Analytics Employee Attrition dataset (`HR-Employee-Attrition.csv`). Place it in `data/` before running the notebook.

## Project structure
- `data/` dataset
- `notebooks/` Python EDA
- `sql/` MySQL queries
- `dashboard/` Power BI file (`.pbix`)
