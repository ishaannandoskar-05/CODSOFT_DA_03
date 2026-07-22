# Retail Sales — Data Visualization Report

Task 3: Meaningful visualizations using Matplotlib, Seaborn, and Plotly, with an interactive
dashboard as a bonus.

## Dataset

`sales_data.csv` — synthetic Superstore-style retail sales data, 2,200 orders spanning
Jan 2023 – Dec 2024.

| Column | Description |
|---|---|
| Order_ID | Unique order identifier |
| Order_Date | Date of order |
| Category | Furniture / Office Supplies / Technology |
| Sub_Category | Product sub-category |
| Region | East / West / North / South |
| Segment | Consumer / Corporate / Home Office |
| Sales | Order revenue (USD) |
| Quantity | Units sold |
| Profit | Order profit (USD) |
| Discount | Discount rate applied |

## Files

| File | Description |
|---|---|
| `retail_visualization_report.ipynb` | Main notebook — all charts, code, and insights |
| `report_view.html` | Static HTML export of the notebook (no Jupyter needed) |
| `01_bar_sales_profit_by_category.png` | Bar chart |
| `02_line_monthly_sales_trend.png` | Line chart |
| `03_pie_sales_by_region.png` | Pie chart |
| `04_histogram_profit_distribution.png` | Histogram |
| `05_scatter_sales_vs_profit.png` | Scatter plot |
| `sales_data.csv` | Source dataset |

## Charts & What They Show

1. **Bar Chart** — Total Sales vs Profit by Category. Technology leads on both; Furniture sells
   well but profits thin.
2. **Line Chart** — Monthly sales trend by category, 2023–2024. Clear Nov–Dec seasonal spike.
3. **Pie Chart** — Sales share by region. Fairly even split, no single dominant region.
4. **Histogram** — Distribution of profit per order, with a break-even line marking loss-making
   orders (concentrated in discounted Furniture).
5. **Scatter Plot** — Sales vs Profit by category, bubble size = quantity. Shows high sales don't
   always mean high profit, especially for Furniture.

## How to Run

```bash
pip install pandas numpy matplotlib seaborn plotly jupyter nbformat nbconvert
jupyter nbconvert --to notebook --execute --inplace retail_visualization_report.ipynb
```
