## Subject: Fetch Data Analysis – Findings & Key Insights  

**Hi Stakeholder,**  

I’ve completed an initial analysis of the Fetch dataset and wanted to share key findings, outstanding questions, and next steps. The full analysis is attached in the Jupyter notebook for further details.

---

## 🔹 Data Quality Issues Identified

- **Severe user-transaction mismatches:** The majority of transactions lack a corresponding user in the `USERS` table, and most users have no transactions. This suggests potential data pipeline issues, incomplete exports, or sample limitations.  
- **Duplicate and inconsistent data:**  
  - Transactions contained `'zero'` as a string instead of `0` in `FINAL_QUANTITY`, creating duplicate records that were removed.  
  - Some `FINAL_SALE` values were blank (`' '`), requiring removal.  
  - The `PRODUCTS` table had duplicate entries, some of which remain due to uncertainty about the correct version.  
- **Potential missing data:** Given the scale of inconsistencies, it’s unclear if this dataset is a full or representative sample.  

---

## 📊 Key Trend: Growth is Slowing, but User Base is Expanding

- Fetch’s **YoY growth percentage has declined**, but **total users continue to increase steadily**.  
- **2022 saw a massive influx of new users**, indicating a possible campaign, app update, or external factor worth investigating.  
- Further analysis into **churn and daily active users (DAU)** would help determine user retention health.  

---

## 📌 Next Steps & Requests for Action

- **Can we assess how closely related the transaction and user data are?**  
- **Are there known data pipeline issues affecting the user-transaction relationship?**  
- **What happened in 2022 that caused a surge in new users?** Understanding this could inform future acquisition strategies.  

Let me know if we should set up time to discuss these findings further. Looking forward to your thoughts!  

**Best,**  
Max 
