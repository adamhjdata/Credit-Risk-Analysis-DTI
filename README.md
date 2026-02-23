# Credit Risk Analysis & Data Pipeline (Python & SQL)

## 📌 Project Overview
This project demonstrates an end-to-end data engineering and risk analytics pipeline focused on credit risk assessment. The primary objective was to integrate raw financial data into a relational database, perform SQL-based feature engineering, and analyze the distribution of **Debt-to-Income (DTI)** ratios as a key predictor of loan defaults.

## 🛠️ Tools & Technologies
* **Python:** Data processing (Pandas), Visualization (Matplotlib), Database Connectivity (Sqlite3).
* **SQL:** Relational data modeling, Data cleaning, and Feature Engineering (DTI calculation).
* **SQLite:** Local database engine for structured data storage and querying.

## 📊 Key Features & Methodology

### 1. ETL Pipeline & Data Integration
* Developed a Python-based **ETL (Extract, Transform, Load)** process to migrate raw `CSV` data into a structured `SQLite` database.
* Implemented data validation logic during the ingestion phase to handle missing values and ensure data integrity for downstream analysis.

### 2. SQL-Driven Feature Engineering
* Leveraged SQL queries to perform on-the-fly transformations, calculating the **DTI (Debt-to-Income)** ratio: $DTI = \frac{Loan\ Amount}{Annual\ Income}$.
* Applied rigorous data filtering to remove anomalies, such as unrealistic demographic data (age > 100) or zero-income records, ensuring statistical robustness.

### 3. Credit Risk Visualization & Insights
* Conducted a density-normalized distribution analysis to compare the DTI profiles of "Repaid" vs. "Defaulted" loans.
* Utilized **Matplotlib**'s `ggplot` styling to generate high-fidelity histograms for risk threshold identification.
* **Key Insight:** Visualized the shift in DTI density, providing a clear visual indicator for credit risk appetites in portfolio management.

## 🖼️ Project Gallery

![DTI Distribution EN](visualizations/DTI_PLOT_EN.png)

<details>
  <summary>▼ Click here to see the Polish version of the analysis</summary>
  <br>
  
  ![DTI Distribution PL](visualizations/DTI_PLOT_PL.png)
</details>

---
