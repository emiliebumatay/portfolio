# Procurement - Spend Analytics Project
## Problem Statement
Axiom Strat Technologies is currently facing a 9.34 million pesos overspend (13.6% variance). To bring operations back within a standard corporate threshold of 3% (2.06 million pesos), this analysis aims to bridge the gap by identifying the remaining 7.28 million pesos in addressable savings across departments.
## Dataset
- **Source:** A 3-year synthetic corporate ERP procurement dump (2023–2025) generated using AI.
- **Volume:** 1,265 raw records optimized down to 618 fully processed, "APPROVED" transaction rows.
- **Key Attributes:** Tracks transaction details across Fiscal Years, Departments, Vendors, and Amounts (PHP).
<img width="100%" alt="Cleaned Transactions (sample)" src="https://github.com/user-attachments/assets/99929a48-b96d-43af-8569-1315558dc0fa" />
<br><br>
<img width="35%" alt="Executive Summary" src="https://github.com/user-attachments/assets/312baef9-0762-4906-85fe-705f387df2f0" />

## Tools
- **Python (Pandas, NumPy):** Used within **Google Colab** for data cleaning and transformation.
- **Power BI:** Used for analysis and visualizations.
## Methodology
### Data Cleaning
Excel was used to handle initial data cleaning. I removed duplicate rows and filtered the dataset to include only 'Approved' transactions, dropping any pending or rejected requests. I also standardized the spend amounts into a consistent numeric format.
(used Pandas)
(you can also create visualizations using Python -- matplotlib, seaborn -- pip install matplotlib)

To fix inconsistent date formats, I moved the data into Google Colab and used Python to clean the dates efficiently. While in Python, I also standardized the department and vendor names to ensure consistent spelling and capitalization across the board.
### Data Analysis and Visualization
I used Excel pivot tables to perform a quick validation of the over-budget areas, before loading the clean dataset into Power BI to build the relational data model, write my KPI measures, and design the final dashboard.
## Insights
- **Departmental overspend concentration:** Applying the 80/20 rule (Pareto principle), just two departments—*Marketing & Sales* and *Facilities & Ops*—are the primary risk areas driving a combined **₱8.69M** of the total budget overspend. Focusing cost-saving efforts on just these two areas allows the company to maximize its impact and easily hit the target.
<div align="center">
<img width="931" height="462" alt="pbix-total budget overspend by department" src="https://github.com/user-attachments/assets/8d49e66f-7b3d-413b-9654-a2be237ee885" />
</div>
- **The spending peak:** Budget performance was relatively stable in 2023, but spiked sharply in **2024**, which alone accounted for **₱5.57M** of the overspend before the company began pulling back and correcting course in 2025.
- **Major cost categories:** *Hardware Procurement* and *Software Licenses* represent the highest overall categories of expenditure across the three-year period, making them the primary targets for long-term contract renegotiations.
- **Hidden risks in under-spending:** *HR & Admin* presents the opposite problem, significantly under-spending their budget by nearly **₱3.49M**. While this appears as a saving, a large negative variance often indicates delayed projects, deferred hiring, or operational bottlenecks that require investigation.
- **Data governance gaps:** There is **₱2.96M** (3.8% of total spend) currently unassigned to any department. This represents an internal data tracking gap the cmompromises budget accountability.
## Visualizations
[Power BI visualizations here]
## Recommendations
- Implement Monthly Budget Tracking: Instead of reviewing spending at the end of the year when it's too late, we should track budget vs actual spend monthly. This will let management catch overspending early and enforce discipline before it gets out of hand.
- Audit Hardware Procurement and Software Licenses: We need to audit these two categories to see if purchases are being misclassified, and enforce stricter spending limits.
- Budget reallocation: Since HR & Admin is under budget, a portion of HR & Admin's unused 3.49 million can be reallocated to cover the operational needs of Marketing & Sales and Facilities & Ops next year.
- Strengthen Data Governance: Wehave nearly 3 million in 'Unassigned' spend. Implementing a strict data governance policy for procurement coding could reallocate this spend and provide a more accurate picture of departmental budgets.
## Conclusion
[Conclusion here] - remove
## Project Assets
- Raw dataset: 
- Cleaned dataset:
- Power BI visualization:
- Python (link to Google Colab)
