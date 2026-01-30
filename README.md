# Alteryx-Loan-Automation
# Automated Loan Approval Pipeline

## 📌 Project Overview
This project demonstrates an end-to-end automated data pipeline designed to streamline the loan application process. Using **Alteryx Designer**, I built a workflow that cleans raw applicant data, calculates key financial metrics, and segments applications based on credit risk thresholds. 

The final results are presented and visualized in a **Jupyter Notebook (Google Colab)** to provide actionable insights for stakeholders.

## 🛠️ Tools Used
* **Alteryx Designer:** Data ETL (Extract, Transform, Load) and Business Logic automation.
* **Python (Pandas/Matplotlib):** Data visualization and presentation.
* **Jupyter Notebook:** Project documentation and reporting.

## ⚙️ The Alteryx Workflow
The automated engine performs the following steps:
1.  **Data Cleaning:** Standardizing data types and handling null values from the raw Kaggle dataset.
2.  **Financial Engineering:** * Calculated **Total Household Income** (Applicant + Co-applicant).
    * Calculated **Loan-to-Income (LTI) Ratio**.
3.  **Risk Segmentation:** Applied a filter logic where applications are **Approved** only if:
    * `Credit_History` is 1.0 (Good standing).
    * `LTI Ratio` is less than 0.35 (Loan is <35% of income).
4.  **Output Generation:** Exported separate datasets for "Automated Approval" and "Manual Review Required."

## 📊 Key Visualizations
Included in the Jupyter Notebook is a **Risk Segmentation Scatter Plot** which visually validates the 0.35 threshold. This chart proves that the automation successfully separates high-risk, high-debt applicants from safe, low-risk borrowers.

## 🚀 Business Impact
* **Efficiency:** Reduces manual underwriting workload by automating low-risk approvals.
* **Consistency:** Eliminates human bias in initial data filtering.
* **Transparency:** Provides a clear audit trail of why a loan was approved or flagged for review.

---
