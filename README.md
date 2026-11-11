# Customer Churn & Retention Analysis

## Project Overview

This project analyzes customer churn in a telecommunications company using Python and the IBM Telco Customer Churn dataset. The objective is to identify high-risk customer segments, understand patterns associated with customer departures, and recommend data-driven retention strategies.

## Business Problem

Customer churn can reduce recurring revenue and increase the cost of acquiring replacement customers. This analysis investigates which customer characteristics are associated with higher churn rates so the business can prioritize retention efforts.

## Tools & Technologies

- **Python** — data analysis
- **Pandas** — data cleaning and manipulation
- **Matplotlib** — data visualization
- **Seaborn** — statistical visualizations
- **Jupyter Notebook** — analysis workflow

## Dataset

The dataset contains **7,043 customer records** and 21 original columns, including customer tenure, contract type, payment method, internet service, monthly charges, total charges, and churn status.

The dataset file is located at `Data/Telco-Customer-Churn.csv`.

## Methodology

1. **Data inspection:** Examined the dataset's structure, column types, and duplicate records.
2. **Data cleaning:** Converted `TotalCharges` to a numeric data type and handled 11 blank values by replacing them with zero. These records had zero tenure and no recorded churn.
3. **Exploratory data analysis:** Calculated churn rates across contract types, tenure groups, payment methods, internet services, and support-related services.
4. **Customer comparison:** Compared monthly charges for customers who churned with those who remained.
5. **Segment analysis:** Combined contract type, tenure group, and payment method to identify high-risk customer segments.
6. **Business recommendations:** Used the observed patterns to propose retention strategies for further testing.

## Key Findings

- **Overall churn:** 26.54% of customers churned.
- **Contract type:** Month-to-month customers had a 42.71% churn rate, compared with 11.27% for one-year contracts and 2.83% for two-year contracts.
- **Early customer churn:** Customers with 0–6 months of tenure had a 52.94% churn rate.
- **Payment method:** Customers paying by electronic check had a 45.29% churn rate.
- **Internet service:** Fiber-optic customers had a 41.89% churn rate.
- **Monthly charges:** Customers who churned paid an average of $74.44 per month, compared with $61.27 for retained customers.
- **Highest-risk segment:** Month-to-month customers with 0–6 months of tenure who paid by electronic check had a 67.65% churn rate. This segment included 680 customers, of whom 460 churned.

### Contract Churn Comparison

| Contract Type | Churn Rate |
|---|---:|
| Month-to-month | 42.71% |
| One year | 11.27% |
| Two year | 2.83% |

### Monthly Charges Comparison

| Customer Group | Average Monthly Charges |
|---|---:|
| Churned customers | $74.44 |
| Retained customers | $61.27 |

## Business Recommendations

1. **Improve early onboarding:** Contact new customers during their first six months to identify service problems, billing confusion, and unmet expectations.
2. **Test contract incentives:** Evaluate transparent, financially viable offers that encourage eligible month-to-month customers to consider longer-term contracts.
3. **Investigate electronic-check customers:** Review billing complaints, payment friction, and customer experience before assuming the payment method causes churn.
4. **Review fiber-optic service:** Investigate pricing, service reliability, and support experiences among fiber-optic customers.
5. **Prioritize high-risk segments:** Consider targeted retention outreach for new month-to-month customers, especially those paying by electronic check.
6. **Measure campaign effectiveness:** Test retention interventions against a suitable control group and compare churn outcomes before expanding the program.

## Project Deliverables

- `Customer_Churn_Analysis.ipynb` — analysis, calculations, and visualizations.
- `churn_summary.csv` — summary table of key churn metrics.
- `Data/Telco-Customer-Churn.csv` — source dataset.

## Limitations

- The analysis identifies historical associations; it does not prove that contract type, payment method, internet service, or other factors cause churn.
- The monthly charges associated with churned customers are not necessarily equivalent to actual revenue losses or recoverable revenue.
- The analysis is descriptive and does not establish whether a particular retention strategy will prevent churn.
- Retention recommendations should be validated through further investigation and controlled testing.
- The findings describe this dataset and may not generalize to every telecommunications company.

## How to Run

1. Download or clone this repository.
2. Install Python and the required libraries.
3. Open `Customer_Churn_Analysis.ipynb` in Jupyter Notebook.
4. Ensure the dataset is available at `Data/Telco-Customer-Churn.csv`.
5. Run the notebook cells in order.

Install the main libraries with:

```bash
pip install pandas matplotlib seaborn jupyter
```

## Author

Business Analytics Portfolio Project
