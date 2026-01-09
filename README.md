# Sales-Revenue-Analytics
End-to-end sales analytics project using ETL, Python, and data visualization

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

##  Business Recommendations
- Restrict excessive discounting.
- Reassess pricing strategy for loss-making products.
- Prioritize high-margin categories for growth.
- Align promotions with seasonal demand patterns.

---

##  Tools Used
- Python (Pandas, NumPy)
- Matplotlib, Seaborn
- Google Colab
- GitHub

---
