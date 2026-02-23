# Credit-Risk-Analysis-DTI
Credit risk analysis and DTI calculation using SQL (SQLite) and Python (Pandas, Matplotlib).

## Project Overview
This project demonstrates a data engineering and analysis pipeline for credit risk assessment. It processes historical loan data to evaluate the relationship between the **Debt-to-Income (DTI)** ratio and the probability of default.

### Key Features
* **Data Integration:** Migrating raw CSV data from Kaggle into a structured SQLite database for SQL-based querying.
* **Data Cleaning & Filtering:** Handling anomalies (e.g., unrealistic age or zero-income records).
* **Feature Engineering:** Calculating DTI ratios using SQL logic.
* **Financial Visualization:** Comparing distribution densities of repaid vs. defaulted loans.

## The Technical Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, Matplotlib, SQLite3
* **Database:** SQL (for relational data management)

## Methodology
1. **ETL Process:** Data is loaded from `credit_data_clean.csv`, validated, and pushed to a local SQLite instance (`credit_risk.db`).
2. **SQL Analysis:** A custom query calculates the DTI for each applicant while filtering out outliers (age > 100).
3. **Visualization:** A density-normalized histogram is generated to compare behaviors of different borrower groups.

## Insights
The generated analysis (see below) shows how DTI distribution shifts for 'Default' cases compared to 'Repaid' loans, providing a visual threshold for risk appetite.

![DTI Distribution EN](visualizations/DTI_PLOT_EN.png)

<details>
  <summary> Kliknij tutaj, aby zobaczyć wykres po polsku</summary>
  <br>
  
  ![DTI Distribution PL](visualizations/DTI_PLOT_PL.png)
</details>
