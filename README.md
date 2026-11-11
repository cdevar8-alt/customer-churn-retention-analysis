# Customer Churn & Retention Analysis

## Project Overview
This project analyzes customer churn in a telecommunications company using Python and the IBM Telco Customer Churn dataset. The objective is to identify high-risk customer segments and recommend data-driven retention strategies.

## Tools & Technologies
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset
The dataset contains 7,043 customer records covering customer tenure, contract type, payment method, internet service, monthly charges, and churn status.

## Key Findings
- Overall customer churn rate: **26.54%**
- Month-to-month contract churn rate: **42.71%**
- Churn rate among customers with 0–6 months of tenure: **52.94%**
- Electronic-check customer churn rate: **45.29%**
- Fiber-optic customer churn rate: **41.89%**
- Average monthly charges: **$74.44 for churned customers**, compared with **$61.27 for retained customers**
- Highest-risk segment: month-to-month customers with 0–6 months of tenure paying by electronic check, with a **67.65% churn rate** across 680 customers.

## Business Recommendations
1. Improve onboarding and customer support during the first six months.
2. Test incentives for eligible customers to move to longer-term contracts.
3. Investigate billing issues and customer experiences associated with electronic-check payments.
4. Review pricing and service quality among fiber-optic customers.
5. Test retention campaigns and measure their impact against a suitable control group.

## Project Deliverables
- `Customer_Churn_Analysis.ipynb` — data analysis and visualizations.
- `churn_summary.csv` — summary of key churn metrics.

## Limitations
The findings show historical associations, not causation. Monthly charges associated with churned customers are not necessarily recoverable revenue. Retention strategies should be tested before implementation.

## Author
Business Analytics Portfolio Project
