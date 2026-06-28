💊 Supplement Sales Analysis


Exploratory Data Analysis (EDA) on weekly supplement sales data — uncovering revenue drivers, return patterns, platform performance, and top products.


📌 Project Overview

This project performs a full EDA on a weekly supplement sales dataset. The analysis covers:


Data cleaning — handling nulls, duplicates, and date parsing
Descriptive statistics — numerical and categorical summaries
Revenue trends — time-series analysis of daily revenue
Category & product performance — which categories and products generate the most revenue
Platform & location breakdown — revenue by sales channel and geography
Return rate analysis — identifying which categories have the highest return rates



📊 Key Findings

InsightDetail💰 Price vs RevenueStrong positive correlation — price is the main revenue driver📦 Units Sold vs RevenueWeak correlation — volume alone doesn't determine revenue🏆 Top Revenue CategoryIdentified via grouped bar chart🛒 Best PlatformVisualized via pie chart by platform revenue share🔁 Highest Return RateIdentified per category using calculated return rate metric🥇 Top 5 ProductsRanked by total revenue


🛠️ Tech Stack

LibraryPurposepandasData loading, cleaning, and aggregationnumpyNumerical operationsmatplotlibStatic charts and plotsseabornHeatmaps and styled bar chartsplotlyInteractive visualizations


⚙️ Getting Started

1. Clone the repository

bashgit clone https://github.com/YOUR_USERNAME/supplement-sales-analysis.git
cd supplement-sales-analysis

2. Install dependencies

bashpip install pandas numpy matplotlib seaborn plotly jupyter

3. Run the notebook

bashjupyter notebook notebooks/supplements.ipynb


Update the dataset path inside the notebook to point to data/Supplement_Sales_Weekly_Expanded.csv




📈 Visualizations

All charts are saved in the visuals/ folder. Here is a summary of what each covers:

FileDescriptioncorrelation_heatmap.pngCorrelation matrix across all numeric featuresrevenue_over_time.pngDaily revenue trend (line chart)revenue_by_category.pngTotal revenue per product category (bar chart)location_platform_revenue.pngStacked bar — revenue by location and platformplatform_revenue_pie.pngRevenue share across sales platforms (pie chart)top5_products.pngTop 5 products by total revenuereturn_rate_by_category.pngAverage return rate per product category


📂 Dataset

File: Supplement_Sales_Weekly_Expanded.csv

Key columns include:


Date — Week of sale
Product Name — Supplement product
Category — Product category (e.g., Protein, Vitamins, etc.)
Platform — Sales channel (e.g., Amazon, Website, Retail)
Location — Geographic region
Price — Unit price
Units Sold — Number of units sold
Units Returned — Number of units returned
Revenue — Total revenue for that entry



🧮 Engineered Features

Two new columns were created during analysis:


returned_rate — Units Returned / Units Sold
returned_percentage — Return rate expressed as a percentage (rounded to 1 decimal)



👤 Author

Khaled Ayman
Feel free to fork, star ⭐, or open an issue if you have suggestions.


📄 License

This project is open source under the MIT License.
