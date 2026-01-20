# Retail Invoice Revenue Analysis (Python)

## Overview
This project analyzes retail invoice-level data to examine revenue distribution, customer concentration, and geographic purchasing behavior using Python.

## Tools Used
- Python
- pandas
- numpy
- matplotlib
- scipy

## Key Analysis Steps
- Aggregated transactional data to invoice-level metrics
- Analyzed average order value (AOV) and revenue distribution
- Quantified revenue concentration across invoices
- Compared UK vs non-UK invoice revenue using a Mann–Whitney U test

## Key Findings
- Invoice revenue is highly right-skewed, with mean AOV significantly higher than the median
- The top 10% of invoices account for approximately 45% of total revenue
- Non-UK invoices are significantly larger than UK invoices on average
- Statistical testing confirmed a significant difference in invoice revenue by region (p < 0.001)

## Notes
Raw data is excluded due to file size constraints. Analysis was conducted on a cleaned dataset derived from publicly available retail transaction data.
