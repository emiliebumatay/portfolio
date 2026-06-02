# Procurement - Spend Analytics Project
## Problem Statement
Axiom Strat Technologies is facing a 13.6% budget variance, resulting in a 9.34 million overspend. This analysis investigates exactly which departments and expense categories are driving these losses.
## Dataset
- Transaction Log with purchase orders, dates, department, budgets, actual spend, and expense categories
- Years covered: 2023 to 2025
- Number of usable rows:
- Original number of rows: 
[Delete later: To diagnose this issue, I analyzed Axiom Strat's transaction log dataset spanning three years from 2023 to 2025. The dataset contains [XXXX] rows and [xxxx] columns, capturing key fields like transaction dates, department names, budgets, actual spend, and expense categories.]
## Tools
- Excel and Python – Data processing, cleaning, and exploratory data analysis (EDA)
- Excel and Power BI - visualizations and data analysis
## Methodology
### Data Cleaning
Excel was used to handle initial data cleaning. I removed duplicate rows and filtered the dataset to include only 'Approved' transactions, dropping any pending or rejected requests. I also standardized the spend amounts into a consistent numeric format.

To fix inconsistent date formats, I moved the data into Google Colab and used Python to clean the dates efficiently. While in Python, I also standardized the department and vendor names to ensure consistent spelling and capitalization across the board.
### Data Analysis and Visualization
Finally, I used Excel pivot tables to perform a quick validation of the over-budget areas, before loading the clean dataset into Power BI to build the relational data model, write my KPI measures, and design the final dashboard.
## Insights
- Marketing & Sales and Facilities & Ops are our primary risk areas. Together, they drive over 8.6 million of the total budget overrun.
- HR & Admin presents the opposite probelm, significantly under-spending their budget by nearly 3.49 million. While this looks like savings on parper, a large negative variance like this often indicates delayed projects or under-staffing that needs to be investigated.
- There is 2.96M (3.8% of total spend) currently unassigned to any department. This represents a gap in data tracking.
- Hardware Procurement and Software Licenses are the biggest expense categories, together representing the largest share of corporate spend.
## Visualizations
[Power BI visualizations here]
## Recommendations
- Audit Hardware Procurement and Software Licenses: We need to audit these two categories to see if purchases are being misclassified, and enforce stricter spending limits.
- Budget reallocation: Since HR & Admin is under budget, a portion of HR & Admin's unused 3.49 million can be reallocated to cover the operational needs of Marketing & Sales and Facilities & Ops next year.
- Implement Monthly Budget Tracking: Instead of reviewing spending at the end of the year when it's too late, we should track budget vs actual spend monthly. This will let management catch overspending early and enforce discipline before it gets out of hand.
- Strengthen Data Governance: Wehave nearly 3 million in 'Unassigned' spend. Implementing a strict data governance policy for procurement coding could reallocate this spend and provide a more accurate picture of departmental budgets.
## Conclusion
[Conclusion here]
## Project Assets
- Raw dataset:
- Cleaned dataset:
