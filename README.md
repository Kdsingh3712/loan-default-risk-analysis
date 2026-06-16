# Loan Default Risk Analysis

## Project Overview
End-to-end data analysis project investigating loan default risk across 25,000+ borrower records. Built using SQL for data cleaning and analysis, and Power BI for interactive dashboards.

## Tools Used
- SQLite (via sqliteonline.com) — data cleaning and analysis
- Power BI — interactive dashboard
- Dataset: credit_risk_dataset.csv (Kaggle) — 32,581 raw records

## Dataset
- Raw records: 32,581
- After cleaning: 25,131
- Columns: person_age, person_income, loan_grade, loan_intent, loan_amnt, loan_int_rate, loan_status, person_emp_length

## Data Cleaning Steps
- Renamed 12 columns from default import names
- Removed fake header row imported with CSV
- Deleted 895 rows with missing employment length
- Deleted 3,116 rows with missing interest rate
- Removed 3,500+ duplicate rows using 5-column match
- Deleted 7 rows with impossible ages (over 80) and employment lengths (over 60 years)

## Analysis Queries
| Query | Key Finding |
|---|---|
| Overall Default Rate | 22.34% — 1 in 4 borrowers defaulted |
| By Loan Grade | Grade G defaults at 98% vs Grade A at 9.95% |
| By Income Bracket | Low income defaults at 46.59% vs Very High at 9.71% |
| By Loan Purpose | Debt Consolidation highest at 29.47% |
| By Employment Length | Less than 1 year highest at 29.17% |
| Top 10 Risk Segments | Grade E/F Debt Consolidation at 100% default rate |

## Power BI Dashboard
3-page interactive dashboard:
- Page 1:
