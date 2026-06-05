# Procurement - Spend Analytics Project
## Problem Statement
Axiom Strat Technologies is currently facing a 9.34 million pesos overspend (13.6% variance). To bring operations back within a standard corporate threshold of 3% (2.06 million pesos), this analysis aims to bridge the gap by identifying the remaining 7.28 million pesos in addressable savings across departments.
## Dataset
- **Source:** A 3-year synthetic corporate ERP procurement dump (2023–2025) generated using AI.
- **Volume:** 1,265 raw records optimized down to 618 fully processed, "APPROVED" transaction rows.
- **Key Attributes:** Tracks transaction details across Fiscal Years, Departments, Vendors, and Amounts (PHP).
<img width="100%" alt="Cleaned Transactions (sample)" src="https://github.com/user-attachments/assets/99929a48-b96d-43af-8569-1315558dc0fa" />
<img width="35%" alt="Executive Summary" src="https://github.com/user-attachments/assets/312baef9-0762-4906-85fe-705f387df2f0" />
## Tools
- Excel and Python – Data processing, cleaning, and exploratory data analysis (EDA) --- (use Python only)
- Excel and Power BI - visualizations and data analysis
## Methodology
### Data Cleaning
Excel was used to handle initial data cleaning. I removed duplicate rows and filtered the dataset to include only 'Approved' transactions, dropping any pending or rejected requests. I also standardized the spend amounts into a consistent numeric format.
(used Pandas)
(you can also create visualizations using Python -- matplotlib, seaborn -- pip install matplotlib)

To fix inconsistent date formats, I moved the data into Google Colab and used Python to clean the dates efficiently. While in Python, I also standardized the department and vendor names to ensure consistent spelling and capitalization across the board.
### Data Analysis and Visualization
I used Excel pivot tables to perform a quick validation of the over-budget areas, before loading the clean dataset into Power BI to build the relational data model, write my KPI measures, and design the final dashboard.
## Insights
- Marketing & Sales and Facilities & Ops are our primary risk areas. Together, they drive over 8.6 million of the total budget overrun. (Pareto)
- HR & Admin presents the opposite problem, significantly under-spending their budget by nearly 3.49 million. While this looks like savings on paper, a large negative variance like this often indicates delayed projects or under-staffing that needs to be investigated.
- There is 2.96M (3.8% of total spend) currently unassigned to any department. This represents a gap in data tracking.
- Hardware Procurement and Software Licenses are the biggest expense categories, together representing the largest share of corporate spend.
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
