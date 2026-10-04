# SKY-GEN-TASK-NO-2
# Superstore Sales Data Analysis

## Project Overview

This project analyzes Superstore sales data to identify business trends, evaluate profitability, understand customer segments, and explore the relationship between discounts and profit.

The project uses Python and data analytics libraries to clean, transform, analyze, and visualize data. The results are used to develop actionable business insights and recommendations.

## Project Objectives

- Understand the structure and quality of the dataset.
- Clean and preprocess the data.
- Handle missing values and identify potential outliers.
- Create meaningful features from existing columns.
- Analyze sales, profit, quantity, and customer segments.
- Investigate regional and monthly sales performance.
- Explore the relationship between discounts and profitability.
- Develop business insights supported by data.
- Create static and interactive visualizations.

## Dataset Information

The dataset contains Superstore order-level details, including customer information, product categories, sales, discounts, profit, and shipping information.

### Main Features

| Column | Description |
|---|---|
| Row ID | Unique row identifier |
| Order ID | Order identification number |
| Order Date | Date the order was placed |
| Ship Date | Date the order was shipped |
| Ship Mode | Shipping method |
| Customer ID | Customer identification number |
| Customer Name | Customer name |
| Segment | Customer segment |
| Country | Country of the customer/order |
| City | City associated with the order |
| State | State associated with the order |
| Region | Sales region |
| Product ID | Product identification number |
| Category | Product category |
| Sub-Category | Product subcategory |
| Product Name | Product name |
| Sales | Sales amount |
| Quantity | Number of units sold |
| Discount | Discount applied |
| Profit | Profit or loss |

**Dataset source:** Use the original dataset source or download link provided with your project. Confirm the license before redistributing the data.

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Git and GitHub

## Project Workflow

### 1. Data Understanding
- Load the dataset.
- Inspect the first and last records.
- Examine the dataset's shape and column names.
- Review data types and statistical summaries.
- Check missing values and duplicate records.

### 2. Data Cleaning and Preprocessing
- Standardize column names.
- Remove exact duplicate records where appropriate.
- Convert date columns into datetime format.
- Check and correct numeric data types.
- Investigate missing values.
- Detect potential outliers using the Interquartile Range (IQR) method.
- Document cleaning decisions.

### 3. Feature Engineering

Create additional features to support business analysis:

- **Shipping Days:** Difference between shipping date and order date.
- **Order Month:** Month in which an order was placed.
- **Order Year:** Year in which an order was placed.
- **Profit Margin (%):** Profit divided by sales, multiplied by 100.
- **Sales per Unit:** Sales divided by quantity.

These features help analyze shipping duration, seasonal trends, and profitability.

### 4. Exploratory Data Analysis

The analysis investigates:

- Sales and profit distributions.
- Customer segment performance.
- Sales and profit by product category.
- Regional and state-level performance.
- Monthly sales and profit trends.
- Discount levels and profitability.
- Relationships between numerical variables.
- Potential outliers in sales and profit.

### 5. Data Visualization

The project includes visualizations such as:

- Missing-value analysis.
- Sales distribution histogram.
- Profit distribution histogram.
- Customer segment comparison.
- Category sales and profit chart.
- Discount versus profit scatter plot.
- Regional profit comparison.
- Numerical correlation heatmap.
- Monthly sales and profit trends.
- Profit by discount band.
- Interactive category performance chart.
- Interactive monthly trend chart.

## Business Questions

The project addresses five key business questions:

1. Which product categories generate the highest sales and profit?
2. Which regions and states perform best and worst in terms of profitability?
3. How do sales and profit change over time?
4. How are discounts associated with profitability?
5. How do customer segments and shipping modes compare in sales, profit, and shipping duration?

Each question is investigated using data summaries, charts, and relevant business metrics.

## Key Performance Indicators (KPIs)

The following KPIs are calculated from the dataset:

| KPI | Calculation |
|---|---|
| Total Sales | Sum of Sales |
| Total Profit | Sum of Profit |
| Total Quantity | Sum of Quantity |
| Unique Orders | Count of distinct Order IDs |
| Unique Customers | Count of distinct Customer IDs |
| Average Sales per Order | Total Sales / Unique Orders |
| Overall Profit Margin (%) | Total Profit / Total Sales × 100 |
| Average Shipping Days | Mean of Shipping Days |

## Business Insights and Recommendations

The analysis is designed to identify opportunities to:

- Improve profitability across product categories.
- Investigate regions with low or negative profit.
- Understand seasonal sales patterns.
- Review discount policies where profitability is weak.
- Identify customer segments with strong sales and profit.
- Evaluate shipping performance using delivery-duration and profit measures.

Specific recommendations should be based on the actual results generated by the notebook.

## Project Deliverables

- Fully executed Jupyter Notebook.
- Cleaned dataset exported as CSV.
- Data cleaning log.
- Business analysis tables.
- Static charts exported as PNG files.
- Interactive charts exported as HTML files.
- README documentation.
- Five-slide presentation summarizing findings and recommendations.

## Repository Structure

```text
superstore-sales-analysis/
│
├── README.md
├── notebooks/
│   └── Superstore_Sales_Analysis.ipynb
├── data/
│   └── superstore_cleaned.csv
├── outputs/
│   ├── category_performance.csv
│   ├── regional_performance.csv
│   ├── monthly_sales_profit.csv
│   ├── discount_analysis.csv
│   ├── segment_performance.csv
│   ├── shipping_performance.csv
│   ├── outlier_analysis.csv
│   └── data_cleaning_log.csv
└── charts/
    ├── 03_sales_distribution.png
    ├── 04_profit_distribution.png
    ├── 06_category_sales_profit.png
    ├── 07_discount_vs_profit.png
    ├── 08_profit_by_region.png
    ├── 09_correlation_heatmap.png
    ├── 10_monthly_sales_profit.png
    ├── 11_profit_by_discount_band.png
    ├── 12_interactive_category_performance.html
    └── 13_interactive_monthly_trends.html
