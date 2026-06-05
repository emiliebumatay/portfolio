# Procurement - Spend Analytics Project
## Problem Statement
Axiom Strat Technologies is currently facing a 9.34 million pesos overspend (13.6% variance). To bring operations back within a standard corporate threshold of 3% (2.06 million pesos), this analysis aims to bridge the gap by identifying the remaining 7.28 million pesos in addressable savings across departments.
## Dataset
- **Source:** A 3-year synthetic corporate ERP procurement dump (2023–2025) generated using AI.
- **Volume:** 1,265 raw records optimized down to 618 fully processed, *APPROVED* transaction rows.
- **Key Attributes:** Tracks transaction details across Fiscal Years, Departments, Vendors, and Amounts (PHP).
<img width="100%" alt="Cleaned Transactions (sample)" src="https://github.com/user-attachments/assets/99929a48-b96d-43af-8569-1315558dc0fa" />
<br><br>
<img width="35%" alt="Executive Summary" src="https://github.com/user-attachments/assets/312baef9-0762-4906-85fe-705f387df2f0" />

## 🛠️ Tools & Methodology 
### 1️⃣ Data Preparation & Engineering (Python via Google Colab)
* Data Cleaning: Removed duplicate records and filtered out non-final transactions (*Pending* and *Rejected* files) to ensure the analysis focused only on realized expenses.
* Handling Missing Data: Standardized department and category names and flagged missing department entries as *Unassigned* to keep all data fully accountable.
* Date Standardization and Calculations: Uniformly formatted all transaction dates, extracted `Fiscal_Year`, and calculated the core metrics `variance_php` and `variance_percentage`.
  
### 2️⃣ Data Analysis & Dashboard (Power BI)
* Executive-level dashboard design: Designed a clean, easy-to-navigate interface using intuitive visual hierarchies, uniform theme colors, and global interactive filters.

## Insights and Visualizations
- **Departmental overspend concentration:** Applying the 80/20 rule (Pareto principle), just two departments—*Marketing & Sales* and *Facilities & Ops*—are the primary risk areas driving a combined **₱8.69M** of the total budget overspend. Focusing cost-saving efforts on just these two areas allows the company to maximize its impact and easily hit the target.
<div align="center">
<img width="70%" alt="pbix-total budget overspend by department" src="https://github.com/user-attachments/assets/372fd6d5-ab13-4d7e-8ff6-5dbf25db2e1b" />
</div>

- **The spending peak:** Budget performance was relatively stable in 2023, but spiked sharply in **2024**, which alone accounted for **₱5.57M** of the overspend before the company began pulling back and correcting course in 2025.
<div align="center">
<img width="70%" alt="image" src="https://github.com/user-attachments/assets/7f4b112b-3b5e-4858-a1ab-626cdd061378" />
</div>
  
- **Major cost categories:** *Hardware Procurement* and *Software Licenses* represent the highest overall categories of expenditure across the three-year period, making them the primary targets for long-term contract renegotiations.
<div align="center">
<img width="70%" alt="pbix top expense categories by total spend" src="https://github.com/user-attachments/assets/96db11f4-0df7-4a4e-9fc9-0fffffb28766" />
</div>
  
- **Hidden risks in under-spending:** *HR & Admin* presents the opposite problem, significantly under-spending their budget by nearly **₱3.49M**. While this appears as a saving, a large negative variance often indicates delayed projects, deferred hiring, or operational bottlenecks that require investigation.
- **Data governance gaps:** There is **₱2.96M** (3.8% of total spend) currently unassigned to any department. This represents an internal data tracking gap the compromises budget accountability.
## 🚀 Strategic Recommendations
* **Focus Cost Controls on High-Risk Departments:** Instead of cutting budgets across the entire company, focus cost-saving efforts strictly on **Marketing & Sales** and **Facilities & Ops**. Because these two departments drive ₱8.69M of the overspend, targeting them directly will give the company the biggest impact with the least amount of disruption.
* **Review the 2024 Spending Spike:** Run a review on what caused the massive ₱5.57M overspend peak in 2024. Identifying whether this was due to specific project approvals or unexpected vendor costs will help set up rules to prevent a similar spike from happening again.
* **Renegotiate Vendor Contracts for Top Expense Categories:** Target **Hardware Procurement** and **Software Licenses**—the two highest spending categories over the three-year period—for contract renegotiations. Consolidating software subscriptions or moving to long-term agreements will help permanently lower baseline costs.
* **Investigate the Operational Delays in HR & Admin:** Look into why **HR & Admin** under-spent their budget by ₱3.49M. While under-spending looks like a saving on paper, a large negative gap often means important hiring was delayed or key operational projects were put on hold, which could hurt the company long-term.
* **Fix Data Tracking Gaps:** Eliminate the ₱2.96M visibility gap by making department codes a mandatory field for all financial transactions. Cleaning up these "Unassigned" records will ensure 100% budget accountability and prevent messy data from reaching executive reports in the future.
## Project Assets
- Raw dataset: 
- Cleaned dataset:
- Power BI visualization:
- Python (link to Google Colab)
