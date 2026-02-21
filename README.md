# Credit-Union-Financial-Health-Analyzer



A Python + SQL project analyzing real U.S. credit union financial data from NCUA Call Reports. It profiles data, validates records, runs SQL queries for business insights, computes key ratios, visualizes trends, and exports stakeholder-ready Excel reports.

Built to demonstrate skills relevant to data analysis, reporting, and problem-solving roles in financial services.

## Overview

This tool:
- Loads and validates NCUA quarterly Call Report data
- Uses SQL (via pandasql) to identify top-performing and high-growth credit unions
- Calculates financial ratios (e.g., loan-to-asset, net worth ratio)
- Generates visualizations for stakeholder presentations
- Exports multi-sheet Excel reports

**Goal**: Help teams answer questions like  
*"Which credit unions are financially strong or showing high growth potential?"*

## Skills Demonstrated
- SQL queries for business analysis
- Python (pandas) for data cleaning, validation, and feature engineering
- Basic statistical techniques (summary stats, ratios)
- Data visualization (matplotlib/seaborn)
- Reporting & dashboards (Excel export)
- Documentation & transparency (handling real data limitations)

## Data Source
- Public NCUA Quarterly Call Report (example: Q3 2025)
- Main file: FS220.txt (balance sheet summary)
- Merged with FS220C.txt (loans detail) for richer analysis
- Link: https://ncua.gov/analysis/credit-union-corporate-call-report-data/quarterly-data

**Note**: In this public export, loan and net worth fields appear zeroed (likely privacy masking). Assets data is fully populated and analyzed. In production, full internal data would be used.

## Demo Outputs

### Asset Distribution ($ Millions)
![Asset Distribution](assets_distribution.png)

### Top 10 Credit Unions by Total Assets ($ Millions)
![Top 10 Assets](top_10_assets_bar.png)

### Loan-to-Asset Ratio vs Total Assets
![Loan-to-Asset Scatter](loan_to_asset_scatter.png)

### Sample Excel Report
[Download credit_union_analysis_report.xlsx](credit_union_analysis_report.xlsx)  
(Sheets: Raw_Data, Statistics, Top_Assets_SQL, High_Growth_SQL)

## How to Run
1. Clone the repo
2. Install dependencies:
   ```bash
   pip install pandas pandasql matplotlib seaborn openpyxl
