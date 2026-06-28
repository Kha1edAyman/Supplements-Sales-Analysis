# 💊 Supplement Sales Analysis
 
> **Exploratory Data Analysis (EDA) on weekly supplement sales data — uncovering revenue drivers, return patterns, platform performance, and top products.**
 
---
 
## 📁 Repository Structure
 
```
supplement-sales-analysis/
│
├── data/
│   └── Supplement_Sales_Weekly_Expanded.csv   # Raw dataset
│
├── notebooks/
│   └── supplements.ipynb                      # Main analysis notebook
│
├── visuals/
│   ├── correlation_heatmap.png
│   ├── revenue_over_time.png
│   ├── revenue_by_category.png
│   ├── location_platform_revenue.png
│   ├── platform_revenue_pie.png
│   ├── top5_products.png
│   └── return_rate_by_category.png
│
└── README.md
```
 
---
 
## 📌 Project Overview
 
This project performs a full EDA on a weekly supplement sales dataset. The analysis covers:
 
- **Data cleaning** — handling nulls, duplicates, and date parsing
- **Descriptive statistics** — numerical and categorical summaries
- **Revenue trends** — time-series analysis of daily revenue
- **Category & product performance** — which categories and products generate the most revenue
- **Platform & location breakdown** — revenue by sales channel and geography
- **Return rate analysis** — identifying which categories have the highest return rates
---
 
## 📊 Key Findings
 
| Insight | Detail |
|---|---|
| 💰 Price vs Revenue | Strong positive correlation — price is the main revenue driver |
| 📦 Units Sold vs Revenue | Weak correlation — volume alone doesn't determine revenue |
| 🏆 Top Revenue Category | Identified via grouped bar chart |
| 🛒 Best Platform | Visualized via pie chart by platform revenue share |
| 🔁 Highest Return Rate | Identified per category using calculated return rate metric |
| 🥇 Top 5 Products | Ranked by total revenue |
 
---
 
## 🛠️ Tech Stack
 
| Library | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, and aggregation |
| `numpy` | Numerical operations |
| `matplotlib` | Static charts and plots |
| `seaborn` | Heatmaps and styled bar charts |
| `plotly` | Interactive visualizations |
 
---
 
## ⚙️ Getting Started
 
### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/supplement-sales-analysis.git
cd supplement-sales-analysis
```
 
### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```
 
### 3. Run the notebook
```bash
jupyter notebook notebooks/supplements.ipynb
```
 
> Update the dataset path inside the notebook to point to `data/Supplement_Sales_Weekly_Expanded.csv`
 
---
 
## 📈 Visualizations
 
All charts are saved in the `visuals/` folder. Here is a summary of what each covers:
 
| File | Description |
|---|---|
| `correlation_heatmap.png` | Correlation matrix across all numeric features |
| `revenue_over_time.png` | Daily revenue trend (line chart) |
| `revenue_by_category.png` | Total revenue per product category (bar chart) |
| `location_platform_revenue.png` | Stacked bar — revenue by location and platform |
| `platform_revenue_pie.png` | Revenue share across sales platforms (pie chart) |
| `top5_products.png` | Top 5 products by total revenue |
| `return_rate_by_category.png` | Average return rate per product category |
 
---
 
## 📂 Dataset
 
**File:** `Supplement_Sales_Weekly_Expanded.csv`
 
**Key columns include:**
 
- `Date` — Week of sale
- `Product Name` — Supplement product
- `Category` — Product category (e.g., Protein, Vitamins, etc.)
- `Platform` — Sales channel (e.g., Amazon, Website, Retail)
- `Location` — Geographic region
- `Price` — Unit price
- `Units Sold` — Number of units sold
- `Units Returned` — Number of units returned
- `Revenue` — Total revenue for that entry
---
 
## 🧮 Engineered Features
 
Two new columns were created during analysis:
 
- `returned_rate` — Units Returned / Units Sold
- `returned_percentage` — Return rate expressed as a percentage (rounded to 1 decimal)
---
 
## 👤 Author
 
**Khaled Ayman**
Feel free to fork, star ⭐, or open an issue if you have suggestions.
 
---
 
## 📄 License
 
This project is open source under the [MIT License](LICENSE).
 
