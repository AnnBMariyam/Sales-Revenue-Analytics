# Sales-Revenue-Analytics
End-to-end sales analytics project using ETL, Python,SQL and data visualization

##  Project Overview
This project analyzes sales and revenue data to uncover key business insights related to profitability, discounting, product performance, and seasonal trends.

The goal is to demonstrate end-to-end data analytics skills including ETL, exploratory data analysis, visualization, and business storytelling.

---

##  Dataset
- Source: Superstore Sales Dataset
- Records: ~10,000 transactions
- Key Features:
  - Sales, Profit, Discount, Quantity
  - Product Category & Sub-Category
  - Customer Segment & Region
  - Order and Ship Dates

---

##  ETL Process
**Extract**
- Loaded raw CSV data with explicit encoding handling.

**Transform**
- Converted date columns to datetime.
- Created time-based features (year, month).
- Engineered profit margin metric.
- Standardized column names.

**Load**
- Saved cleaned dataset for reuse in analysis and dashboards.

---

##  Key Analyses Performed
- Overall business KPIs (Sales, Profit, Orders, Customers)
- Sales and profit by category
- Loss-making sub-category analysis
- Discount vs profit impact
- Monthly sales trend analysis

---

##  Key Insights
- Technology is the most profitable category.
- Furniture has high sales but weak margins.
- Tables are the largest loss-making sub-category.
- Discounts above 30% consistently lead to losses.
- Sales exhibit clear seasonal patterns.

---

## SQL Analysis

This project also includes SQL-based business analysis on the cleaned sales dataset.

SQL queries were used to analyze:
- total sales and profit KPIs
- category performance
- loss-making sub-categories
- monthly sales trends
- discount impact on profitability
- top customers by sales
- region-wise performance

Screenshots are added in the imgaes file and the .sqbpro is uploaded in the notebooks file.

---

##  Tools Used
- Python (Pandas, NumPy)
- SQL
- Matplotlib, Seaborn
- Google Colab
- GitHub

---
