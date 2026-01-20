# Retail Invoice Revenue Analysis (Python)

## Overview
This project analyzes retail invoice-level data to examine revenue distribution, customer concentration, and geographic purchasing behavior using Python. The analysis focuses on understanding how invoice revenue is distributed, how concentrated total revenue is among high-value orders, and whether purchasing behavior differs between UK and non-UK customers.

## Dataset
- Publicly available online retail transaction data
- Transactions aggregated to the invoice level for analysis
- Raw data excluded from the repository due to file size constraints

## Tools Used
- Python
- pandas
- numpy
- matplotlib
- scipy

## Data Preparation
- Standardized column names for consistency
- Removed zero-value transactions
- Aggregated line-item transactions to invoice-level metrics
- Engineered time-based features (year, month)

## Key Analyses

### Invoice Revenue Distribution
Invoice revenue is highly right-skewed, with most invoices clustered at lower values and a long tail of high-value purchases.

To make this distribution interpretable, invoice revenue was visualized using a focused histogram covering invoices between $0 and $5,000 with controlled bin widths. This approach highlights typical purchasing behavior while preserving the presence of high-value outliers in summary statistics.

### Average Order Value (AOV)
- Mean invoice revenue: approximately $481  
- Median invoice revenue: approximately $303  

The difference between the mean and median confirms a right-skewed distribution driven by a small number of large orders.

### Revenue Concentration
Revenue is highly concentrated among high-value invoices:
- The top 10% of invoices account for approximately 45% of total revenue

This indicates that a relatively small portion of transactions drives a disproportionate share of sales.

### Geographic Comparison (UK vs Non-UK)
Invoice revenue was compared between UK and non-UK customers:
- Non-UK invoices have nearly double the average revenue of UK invoices

A Mann–Whitney U test was used due to non-normal distributions and unequal group sizes:
- The difference in invoice revenue between UK and non-UK customers was statistically significant (p < 0.001)

This suggests meaningful regional differences in purchasing behavior.

## Key Takeaways
- Retail invoice revenue exhibits strong right skew and long-tail behavior
- A small share of high-value invoices contributes disproportionately to total revenue
- Non-UK customers place significantly larger orders on average than UK customers
- Non-parametric statistical testing confirms these differences are statistically significant

## Notes
This project demonstrates practical statistical analysis, data aggregation, and business-focused interpretation using Python. Visualizations and statistical methods were chosen to reflect real-world analyst decision-making rather than purely academic techniques.
