# Procurement Spend and Budget Variance Analysis
## 🎯 Problem Statement
Axiom Strat Technologies is currently facing a **₱9.34M** overspend (13.6% variance over the budget). To bring operations back within an acceptable corporate variance threshold of 3% (**₱2.06M**), this analysis aims to bridge the gap by identifying the remaining **₱7.28M** in addressable savings across departments.
<div align="center">
<img width="50%" alt="pbix-ProblemStatement" src="https://github.com/user-attachments/assets/b57f7613-c82a-4b76-9513-ad2ed0073c16" />
</div>

## 📈 Data
- **Source:** A 3-year (2023 to 2025) simulated corporate ERP procurement dataset generated using AI.
- **Transaction Records:** 602 final transaction records with key variables `FISCAL_YEAR`, `DEPARTMENT_NAME`, `EXPENSE_CATEGORY`, `RAW_AMOUNT` in PHP
- **Executive Summary of Budget and Spend per Department:** including a calculated metric `variance_php`
<img width="100%" alt="Cleaned Transactions (sample)" src="https://github.com/user-attachments/assets/5e470b6d-a866-4b3f-a900-4c3534d284ff" />
<br>
<div align="center">
<img width="45%" alt="Executive Summary" src="https://github.com/user-attachments/assets/541ffff1-331f-43b4-bf38-8841e24b5d0c" />
</div>

## 🛠️ Tools & Methodology 

 1️⃣ **Python via Google Colab** - Data Cleaning & Engineering
* **Data Cleaning:** Removed duplicate records, filtered out non-final transactions (*Pending* and *Rejected*) to ensure the analysis focused only on realized expenses
* **Standardization:** Uniformly formatted transaction dates, departments, and expense categories
* **Handling Missing Data:** Flagged missing department entries as *Unassigned* to keep all data fully accountable
* **Calculations:** Extracted `Fiscal_Year` from the transaction dates, calculated a core metric `variance_php`.
  
 2️⃣ **Power BI** - Data Analysis & Dashboard
* **Executive-level dashboard design:** clean, easy-to-navigate interface, uses intuitive visual hierarchies, uniform theme colors, with global interactive filters
<div align="center">
<img width="100%" alt="pbix-procurement spend and budget variance analysis" src="https://github.com/user-attachments/assets/b7acbc46-9364-460f-8af4-ce88ecc29728" />
</div>

## 💡 Insights
- **Departmental overspend concentration:**
  - A combined **₱8.69M** of the total budget overspend is concentrated in just two departments: **Marketing & Sales** and **Facilities & Ops**
  - [Pareto principle] Targeting optimization strategies in these two areas alone will successfully fulfill and surpass the targeted **₱7.28M** budget recovery goal.
<div align="center">
<img width="70%" alt="pbix-total budget overspend by department" src="https://github.com/user-attachments/assets/372fd6d5-ab13-4d7e-8ff6-5dbf25db2e1b" />
</div>

- **Data tracking gap:**
  - **₱2.96M** was unassigned to any department
  - Represents an internal data tracking gap that compromises budget accountability

- **The spending peak:**
  - The overspend spike in **2024** alone drove **₱5.57M** of the total variance
  - Budget overspend is not a gradual, systemic issue, but was concentrated within a single fiscal year
<div align="center">
<img width="70%" alt="image" src="https://github.com/user-attachments/assets/7f4b112b-3b5e-4858-a1ab-626cdd061378" />
</div>
<div align="center">
<img width="70%" alt="pbix-2024 total budget overspend by department" src="https://github.com/user-attachments/assets/2d4b945c-e312-4888-8a0b-54245b1e1c5d" />
</div>

<details>
 <summary> 🔍 Click to view more insights</summary>
 
- **Hidden risks in under-spending:** *HR & Admin* is significantly under-spending by **₱3.49M**. While this appears as a saving, a large negative variance often indicates delayed projects, deferred hiring, or operational bottlenecks that require investigation.
  
- **Major cost categories:** *Hardware Procurement* and *Software Licenses* represent the highest overall expense categories of expenditure across the three-year period.
<div align="center">
<img width="70%" alt="pbix top expense categories by total spend" src="https://github.com/user-attachments/assets/96db11f4-0df7-4a4e-9fc9-0fffffb28766" />
</div>
</details>

## 🚀 Strategic Recommendations
- **Focus Cost Controls on High-Risk Departments:**
  - Focus cost-saving efforts on **Marketing & Sales** and **Facilities & Ops**, instead of cutting budgets across the entire company
  - Since these two departments drive **₱8.69M** of the overspend, targeting them directly will give the company the biggest impact with the least amount of disruption.
 
- **Fix Data Tracking Gaps:**
  - Make department codes a mandatory field for all financial transactions
  - This will eliminate the **₱2.96M** in unmapped spend and ensure 100% data accountability in future reports

- **Review the 2024 Spending Spike:**
  - Run a review on what caused the massive **₱5.57M** overspend peak in 2024
  - Identifying whether this was due to specific project approvals or unexpected vendor costs will help set up rules to prevent a similar spike from happening again

<details>
  <summary> 🔍 Click to view more strategic recommendations</summary>
 
- **Investigate the Operational Delays in HR & Admin:** Look into why **HR & Admin** under-spent their budget by ₱3.49M. While under-spending looks like a saving on paper, a large negative gap often means important hiring was delayed or key operational projects were put on hold, which could hurt the company long-term.
  
- **Renegotiate Vendor Contracts for Top Expense Categories:** Target **Hardware Procurement** and **Software Licenses**—the two highest spending categories over the three-year period—for contract renegotiations. Consolidating software subscriptions or moving to long-term agreements will help permanently lower baseline costs.
</details>
