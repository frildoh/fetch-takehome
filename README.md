# Fetch Take-Home Assessment

## 📂 Project Overview
This repository contains my analysis for the Fetch Senior Data Analyst take-home assessment. The goal was to analyze transaction and user data, identify key insights, and communicate findings to stakeholders.

## 📜 Files & Structure
- `fetch_analysis.ipynb` - The full Jupyter Notebook containing data cleaning, SQL queries, analysis, and visualizations.
- `stakeholder_summary.md` - A stakeholder-friendly summary of key findings, data quality issues, and next steps.
- `data/` - Folder containing raw datasets:
  - `PRODUCTS_TAKEHOME.csv` - Product data.
  - `TRANSACTION_TAKEHOME.csv` - Transaction data.
  - `USER_TAKEHOME.csv` - User data.
- `requirements.txt` - List of required dependencies for running the analysis.

## 📊 Key Findings
- **Data Quality Issues:** Severe mismatches between the `USERS` and `TRANSACTIONS` tables, duplicate product data, and missing values in key columns.
- **Insights:**
  - **Health & Wellness:** Baby Boomers contribute the highest percentage of purchases.
  - **Dips & Salsa:** Tostitos is the top brand.
  - **User Growth:** While YoY % growth has slowed, total users continue to increase, with 2022 seeing a major spike.

For a deeper dive, please see the `fetch_analysis.ipynb` notebook.

## 📌 Next Steps
- Investigate why most transactions do not match any user.
- Assess how closely related the transaction and user data are and whether they can be reliably joined for meaningful analysis.
- Analyze churn and daily active users (DAU) to complement the YoY growth analysis.

## 💡 How to Run the Analysis

1. **Clone the Repository**
   ```sh
   git clone https://github.com/frildoh/fetch-takehome.git
   cd fetch-takehome
   ```

2. **Create and Activate a Virtual Environment** (Recommended)
   ```sh
   python -m venv venv
   source venv/bin/activate  # Mac/Linux
   venv\Scripts\activate  # Windows
   ```

3. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```

4. **Run Jupyter Notebook**
   ```sh
   jupyter notebook
   ```
   Then, open `fetch_analysis.ipynb` and run the cells.
