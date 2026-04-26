# Sales Performance & Profitability Analysis | Python, Pandas, Matplotlib,Seaborn

## Business Problem
Retail companies struggle to identify which product categories drive profit and which sub-categories cause losses. High discounts often erode margins without visibility. This analysis uncovers sales trends, profit drivers, and loss-making segments to enable data-driven decisions.

## Project Objective
Analyzed retail sales data to:
1. Identify category-wise sales and profit trends using data aggregation
2. Evaluate key profit drivers and underperforming categories
3. Analyze the impact of discounts on profitability using scatter plot correlation
4. Detect seasonality patterns in monthly sales with time series analysis

## Tech Stack
- Language: Python 
- Libraries: Pandas, NumPy, Matplotlib, Seaborn
- Techniques: Data Cleaning, GroupBy Aggregation, Data Visualization, EDA

## Visualizations

### 1. Bar Chart - Category-wise Sales vs Profit
Compares total sales and profit across main product categories to identify high-revenue vs high-margin segments.
[Category Wise Sales and Profit](category_wise_sales_and_profit.png)

### 2. Scatter Plot - Discount vs Profit  
Shows relationship between discount percentage and profit. Identifies if heavy discounts lead to losses.
[Discount vs Profit](discount_vs_profit)

### 3. Line Chart - Monthly Sales Trend
Displays seasonality patterns by plotting total sales across months. Helps with inventory planning.
[Monthly Sales Trend](monthly_sales_trend.png)

## Data Processing Pipeline
1. Data Loading: Import CSV using `pd.read_csv()`
2. Data Cleaning:
   - Standardized column names to `lowercase_with_underscores`
   - Converted `order_date` to datetime and extracted `month`, `year`
   - Handled missing values in `sales`, `profit`, `quantity`, `discount` columns
   - Created `profit_margin` metric: `(profit/sales)*100`
3. Data Analysis: Used `groupby()` + `agg()` to calculate KPIs by category and sub-category
4. Data Visualization: Matplotlib used for bar, scatter, and line charts

