# 💰 Sales Revenue Analytics — End-to-End Data Analytics Project

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)
![SQL](https://img.shields.io/badge/SQL-Business%20Analysis-lightblue?style=flat-square)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=flat-square&logo=powerbi)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)

> **Which products are silently killing your margins?**
> This project analyzes **9,994 transactions (~$2.3M in sales, $286K profit)** across a retail business to uncover what's driving profit — and what's destroying it.

---

## 📌 Project Overview

This end-to-end analytics project examines retail sales performance across product categories, customer segments, regions, and time — following a full ETL → EDA → SQL Analysis → Visualization workflow.

The goal: translate raw transactional data into clear, actionable business insights that support data-driven decisions on pricing, discounting, and product strategy.

---

## 📂 Repository Structure

```
Sales-Revenue-Analytics/
│
├── dataset/              # Raw and cleaned Superstore Sales CSV files
├── notebooks/            # Python EDA notebook + SQL queries (.sqbpro)
├── images/               # SQL screenshots + Python visualizations
│   ├── 01_kpis.sql.png
│   ├── 02_category_performance.sql.png
│   ├── 03_loss_making_subcategories.sql.png
│   ├── 04_monthly_sales_trend.sql.png
│   ├── 05_discount_analysis.sql.png
│   ├── 06_top_customers.sql.png
│   ├── 07_region_performance.sql.png
│   ├── discount_vs_profit.png
│   ├── loss_subcategories.png
│   ├── monthly_sales_trend.png
│   ├── profit_by_category.png
│   └── sales_by_category.png
└── README.md
```

---

## 📊 Dataset

- **Source:** Superstore Sales Dataset (retail transactional data)
- **Size:** ~10,000 records, 21 columns
- **Key Features:**

| Dimension | Variables |
|---|---|
| Financial | Sales, Profit, Discount, Quantity |
| Product | Category, Sub-Category |
| Customer | Segment, Customer Name |
| Geography | Region, State, City |
| Time | Order Date, Ship Date |

---

## 🔧 Tech Stack

| Area | Tools |
|---|---|
| Language | Python 3.8+ |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Power BI |
| SQL Analysis | SQL (DB Browser / SQLite) |
| Environment | Google Colab, GitHub |

---

## ⚙️ ETL Pipeline

### Extract
- Loaded raw CSV with explicit encoding handling to avoid character errors

### Transform
- Converted `Order Date` and `Ship Date` columns to datetime format
- Engineered time-based features: `Year`, `Month` for trend analysis
- Created `Profit Margin` metric: `Profit / Sales`
- Standardized column names for consistency across Python and SQL analysis

### Load
- Exported cleaned dataset for reuse in SQL queries and Power BI dashboards

---

## 🔍 Analysis Performed

### Python (EDA & Visualization)
- Overall business KPIs: Total Sales, Profit, Orders, Unique Customers
- Sales and profit breakdown by Category and Sub-Category
- Loss-making sub-category identification
- Discount vs. Profit impact analysis
- Monthly sales trend with seasonality patterns
- Top customers by revenue contribution

### SQL (Business Intelligence Queries)
Seven focused SQL analyses were run on the cleaned dataset:

| # | Query | Purpose |
|---|---|---|
| 01 | KPIs | Total Sales, Profit, Orders, Customers |
| 02 | Category Performance | Sales & profit by product category |
| 03 | Loss-Making Sub-Categories | Identifying unprofitable product lines |
| 04 | Monthly Sales Trend | Time-series revenue patterns |
| 05 | Discount Analysis | Discount threshold impact on profit |
| 06 | Top Customers | Highest-value customers by sales |
| 07 | Region Performance | Geographic revenue and profit breakdown |

---

## 📈 Key Insights & Business Findings

### 🏆 What's Working
- **Technology** is the highest-profit category — **$145K profit**, strong margins
- **Top customers** contribute up to **$25K in individual sales** — retention focus recommended
- Sales show clear **seasonal peaks** — inventory and marketing can be timed accordingly

### ⚠️ What's Hurting the Business
- **Tables sub-category** is the single largest loss-maker at **-$17.7K** — pricing or sourcing needs review
- **Furniture** overall has high sales volume but dangerously thin margins
- **Discounts above 30% consistently produce negative profit** — discount policy needs a hard cap
- The discount-profit relationship is not linear: moderate discounts (10–20%) are sustainable, but deep discounts eliminate margin entirely

### 💡 Business Recommendation
> Implement a **30% discount ceiling** company-wide. Re-evaluate the Tables product line for either repricing or discontinuation. Redirect marketing spend toward Technology, where margin per dollar of revenue is highest.

---

## 📸 Sample Visualizations

> *(Screenshots available in the `/images` folder)*

- `profit_by_category.png` — Category-level profit comparison
- `discount_vs_profit.png` — Scatter plot showing discount–profit relationship
- `monthly_sales_trend.png` — Time-series revenue trend across months
- `loss_subcategories.png` — Bar chart of loss-making sub-categories
- `01_kpis.sql.png` through `07_region_performance.sql.png` — SQL query outputs

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/AnnBMariyam/Sales-Revenue-Analytics.git
cd Sales-Revenue-Analytics

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Run the notebook
jupyter notebook notebooks/
```

For SQL analysis, open the `.sqbpro` file in [DB Browser for SQLite](https://sqlitebrowser.org/).

---

## 👩‍💻 Author

**Ann B Mariyam**
MS Data Analytics — University of Illinois Springfield
[LinkedIn](https://www.linkedin.com/in/ann-b-mariyam-a238a7275/) | [GitHub](https://github.com/AnnBMariyam) | annbijumariyam02@gmail.com
