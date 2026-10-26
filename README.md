# Retail Sales & Profitability Analysis Using Python

## Project overview
This Business Analytics project analyzes retail sales data to understand revenue, profit, product performance, regional performance, monthly trends, and discount-related profitability. It demonstrates a practical analytics workflow: data cleaning, feature engineering, exploratory analysis, visualization, and business recommendations.

> **Dataset note:** `data/retail_sales_sample.csv` is a reproducible synthetic dataset created for this project. It does not represent a real company. Replace it with a properly licensed real-world dataset if your course requires one.

## Business questions
1. What are total sales, total profit, and overall profit margin?
2. Which categories and sub-categories perform best and worst?
3. Which regions contribute the most profit?
4. How do sales change month by month?
5. How does average profit vary across discount bands?

## Tools
- Python
- Pandas
- Matplotlib
- Seaborn

## Repository structure
```text
retail-sales-business-analytics/
├── data/
│   └── retail_sales_sample.csv
├── outputs/
│   ├── charts/
│   └── (generated reports and CSV summaries appear here after running)
├── src/
│   └── analyze_sales.py
├── requirements.txt
├── .gitignore
└── README.md
```

## How to run (Windows)
1. Install Python 3.10 or newer.
2. Download or clone this repository and open the folder in VS Code or a terminal.
3. Create a virtual environment (recommended):
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Run the analysis:
   ```bash
   python src/analyze_sales.py
   ```

The script creates:
- `outputs/cleaned_retail_sales.csv`
- `outputs/category_summary.csv`
- `outputs/region_summary.csv`
- `outputs/subcategory_profit.csv`
- `outputs/business_summary.txt`
- Four charts in `outputs/charts/`

## Methodology
1. Load the CSV with Pandas.
2. Remove duplicate records and convert columns to suitable data types.
3. Handle invalid dates and missing numeric values.
4. Create month, year, profit-margin, and discount-band features.
5. Aggregate sales and profit by category, region, sub-category, and month.
6. Export visualizations and a text report with data-driven findings.

## Business recommendations
Use the generated results to prioritize product lines with stronger profit, investigate loss-making sub-categories, evaluate discounting using profit rather than sales alone, and plan inventory based on monthly demand patterns. Validate recommendations with real company data before making operational decisions.

## Limitations and future improvements
- The bundled data is synthetic and useful for demonstrating the workflow only.
- The analysis is descriptive; it does not establish that discounts cause profit changes.
- Future extensions: interactive Plotly dashboard, SQL analysis, Power BI dashboard, and sales forecasting.

## Author
Add your name and course details here before submission.
