# Data Analysis Internship — Week 1

## Project
Retail Store Sales Data Cleaning

## Objective
Clean and prepare a messy retail sales dataset for analysis while documenting all cleaning decisions.

## Tools
- Excel
- Python
- Pandas
- NumPy
- Jupyter Notebook

## Repository structure
```text
data_analysis_internship_week1/
├── data/
│   ├── retail_store_sales_raw.csv
│   └── retail_store_sales_cleaned.csv
├── notebooks/
│   └── Week1_Data_Cleaning.ipynb
├── reports/
│   └── Week1_Data_Cleaning_Report.md
├── Week1_Data_Cleaning.xlsx
└── README.md
```

## Key cleaning results
- Raw rows: 12,575
- Cleaned rows: 11,971
- Rows removed because Quantity and Total Spent were both missing: 604
- Missing Price Per Unit values reconstructed: 609
- Missing Item values reconstructed in retained rows: 609
- Missing Discount Applied values labeled `Unknown`: 3,988
- Exact duplicates: 0
- Duplicate Transaction IDs: 0
- Valid outliers retained: 60

## Cleaning approach
1. Inspected structure, types, missing values, and duplicates.
2. Standardized column names.
3. Converted numeric/date fields to appropriate types.
4. Reconstructed missing prices using `Total Spent / Quantity`.
5. Reconstructed missing items using the unique Category + Price mapping.
6. Removed rows where Quantity and Total Spent were both unavailable.
7. Labeled unknown discount status as `Unknown`.
8. Reviewed IQR outliers and retained valid high-value transactions.
9. Validated the cleaned data and exported the final dataset.

## Files to submit
The main Week 1 deliverables are the raw dataset, cleaned dataset, Jupyter notebook, cleaning report, and Excel workbook.
