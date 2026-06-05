# Procurement - Spend Analytics Project
## 🎯 Problem Statement
Axiom Strat Technologies is currently facing a **₱9.34M** overspend (13.6% variance). To bring operations back within a standard corporate threshold of 3% (**₱2.06M**), this analysis aims to bridge the gap by identifying the remaining **₱7.28M** in addressable savings across departments.
## 📈 Data
- **Source:** A 3-year (2023 to 2025) simulated corporate ERP procurement dataset generated using AI.
- **Volume:** 602 final transaction records (refined from an initial dataset of 1,285 raw rows).
- **Key Attributes:** Tracks transaction details across Fiscal Years, Departments, Vendors, and Amounts (PHP).
<img width="100%" alt="Cleaned Transactions (sample)" src="https://github.com/user-attachments/assets/5e470b6d-a866-4b3f-a900-4c3534d284ff" />
<br>
<div align="center">
<img width="45%" alt="Executive Summary" src="https://github.com/user-attachments/assets/541ffff1-331f-43b4-bf38-8841e24b5d0c" />
</div>

## 🛠️ Tools & Methodology 

 1️⃣ Data Preparation & Engineering (Python via Google Colab)
* Data Cleaning: Removed duplicate records and filtered out non-final transactions (*Pending* and *Rejected* files) to ensure the analysis focused only on realized expenses.
* Handling Missing Data: Standardized department and category names and flagged missing department entries as *Unassigned* to keep all data fully accountable.
* Date Standardization and Calculations: Uniformly formatted all transaction dates, extracted `Fiscal_Year`, and calculated a core metric `variance_php`.
  
 2️⃣ Data Analysis & Dashboard (Power BI)
* Executive-level dashboard design: Designed a clean, easy-to-navigate interface using intuitive visual hierarchies, uniform theme colors, and global interactive filters.


## 💡 Insights and Visualizations
- **Departmental overspend concentration:** A combined **₱8.69M** of the total budget overspend is concentrated in just two departments: *Marketing & Sales* and *Facilities & Ops*. Targeting optimization strategies in these two areas alone will successfully fulfill and surpass the targeted **₱7.28M** budget recovery goal.
<div align="center">
<img width="70%" alt="pbix-total budget overspend by department" src="https://github.com/user-attachments/assets/372fd6d5-ab13-4d7e-8ff6-5dbf25db2e1b" />
</div>

- **Hidden risks in under-spending:** *HR & Admin* is significantly under-spending their budget by nearly **₱3.49M**. While this appears as a saving, a large negative variance often indicates delayed projects, deferred hiring, or operational bottlenecks that require investigation.
  
- **Data governance gaps:** There is **₱2.96M** (3.8% of total spend) currently unassigned to any department. This represents an internal data tracking gap that compromises budget accountability.
  
- **The spending peak:** Budget performance was relatively stable in 2023, but spiked sharply in **2024**, which alone accounted for **₱5.57M** of the overspend before the company began pulling back and correcting course in 2025.
<div align="center">
<img width="70%" alt="image" src="https://github.com/user-attachments/assets/7f4b112b-3b5e-4858-a1ab-626cdd061378" />
</div>
  
- **Major cost categories:** *Hardware Procurement* and *Software Licenses* represent the highest overall expense categories of expenditure across the three-year period.
<div align="center">
<img width="70%" alt="pbix top expense categories by total spend" src="https://github.com/user-attachments/assets/96db11f4-0df7-4a4e-9fc9-0fffffb28766" />
</div>
  
## 🚀 Strategic Recommendations
- **Focus Cost Controls on High-Risk Departments:** Applying the 80/20 rule (Pareto principle), focus cost-saving efforts on **Marketing & Sales** and **Facilities & Ops**, instead of cutting budgets across the entire company. Since these two departments drive ₱8.69M of the overspend, targeting them directly will give the company the biggest impact with the least amount of disruption.
  
- **Investigate the Operational Delays in HR & Admin:** Look into why **HR & Admin** under-spent their budget by ₱3.49M. While under-spending looks like a saving on paper, a large negative gap often means important hiring was delayed or key operational projects were put on hold, which could hurt the company long-term.
  
- **Fix Data Tracking Gaps:** Make department codes a mandatory field for all financial transaction to eliminite the ₱2.96M in unmapped spend and ensure 100% data accountability in future reports.
  
- **Review the 2024 Spending Spike:** Run a review on what caused the massive ₱5.57M overspend peak in 2024. Identifying whether this was due to specific project approvals or unexpected vendor costs will help set up rules to prevent a similar spike from happening again.
  
- **Renegotiate Vendor Contracts for Top Expense Categories:** Target **Hardware Procurement** and **Software Licenses**—the two highest spending categories over the three-year period—for contract renegotiations. Consolidating software subscriptions or moving to long-term agreements will help permanently lower baseline costs.

## 📊 Dashboard
<img width="1412" height="819" alt="pbix-spend and budget analytics dashboard" src="https://github.com/user-attachments/assets/a0b9ca0e-647a-4cb6-8bc0-2363bd09867e" />

## 📂 Project Assets & Quick Links
- Raw dataset: 
- Cleaned dataset:
- Power BI visualization:
- Python (link to Google Colab)
