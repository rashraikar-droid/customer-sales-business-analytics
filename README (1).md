# Customer Sales Performance & Business Analytics Dashboard

## Internship Task 2 - Data Analysis with Python

This project extends the Task 1 work into advanced Pandas, data wrangling, feature engineering, multi-table integration, business analysis, visualization and reporting.

### Dataset

Public retail sales dataset reference:

- Public source mirror: https://huggingface.co/datasets/wdncjenrc/TEST-PROVA/blob/main/retail_sales_dataset.csv
- Original public dataset reference: https://github.com/Oragant/Retail-Sales-Dashboard/blob/main/retail_sales_dataset.csv

I used a 251-row working sample from the public file. The source file does not provide product IDs, cost, profit or region.

### Modelling note

To demonstrate Task 2's relational workflow without inventing missing business fields, the transaction file is normalized into three working tables:

- `customers.csv`
- `products.csv`
- `sales.csv`

`product_id` is an engineered key made from product category and listed unit price. It is not an original source field. Profit is not calculated because the source has no cost data.

### What is covered

- Data quality checks
- Duplicate and missing-value checks
- Data type conversion
- Revenue validation
- Pandas merge
- GroupBy
- Pivot tables
- Cross-tabulation
- Date/time features
- Customer segmentation
- Price bands
- IQR outlier detection
- Customer ranking
- Monthly sales summaries
- Matplotlib
- Seaborn
- Excel/CSV/PDF reporting
- HTML dashboard
- Documentation and reusable modules

### Folder structure

```text
Task-2/
├── data/
│   ├── raw/
│   ├── processed/
│   └── cleaned/
├── notebooks/
├── src/
├── reports/
├── charts/
├── dashboard/
├── screenshots/
├── diagrams/
├── docs/
└── tests/
```

### How to run

```bash
pip install -r requirements.txt
python src/main.py
```

Open `notebooks/customer_sales_business_analysis.ipynb` for the step-by-step analysis.

### Main outputs

- `reports/Business_Report.xlsx`
- `reports/Technical_Report.pdf`
- `docs/Technical_Report.docx`
- `dashboard/dashboard.html`
- `data/cleaned/merged_customer_sales.csv`
- charts and dashboard screenshots

### Limitations

This is an internship practice project. The source is a synthetic retail dataset and the working sample is smaller than the complete public file. Because cost data is not available, profit is not calculated. The engineered product table is used only to demonstrate the multi-table analytics workflow.
