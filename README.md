# Blinkit-Sales-Intelligence-End-to-End-EDA-KPI-Dashboard

📌 Project Overview
This project performs a full end-to-end data analysis pipeline on Blinkit's sales dataset (8,523 transactions, 12 features). The analysis identifies key revenue drivers, outlet performance patterns, and consumer preference trends — culminating in five business-aligned visualisations that answer concrete operational questions.
Why this matters: Blinkit operates across Tier 1–3 cities with outlets of varying size and vintage. Understanding which combination of location, outlet size, and product type drives the most revenue directly informs expansion strategy, inventory planning, and supplier negotiations.

📊 Key Business KPIs
MetricValueTotal Revenue$1,201,681Average Sale per Transaction$141Unique SKUs Sold1,559Average Customer Rating4.0 / 5.0

🔍 Analytical Findings & Insights
1. Fat Content → Revenue Split
Low Fat products dominate, contributing 64.6% ($776,320) of total sales vs. Regular at 35.4% ($425,362). Average transaction value is nearly identical (~$141) across both categories — meaning the gap is driven by volume, not price. Consumer health preferences are clearly shifting, and stocking depth should reflect this imbalance.
2. Total Sales by Item Type
Fruits & Vegetables lead all categories at $178,124, followed closely by Starchy Foods ($175,434) and Household items ($135,977). Seafood ($9,078) and Breakfast ($15,597) are the weakest performers. The top 5 categories account for ~65% of all revenue — a classic Pareto pattern that justifies a tiered stocking strategy.
3. Fat Content × City Tier
Across all three city tiers, Low Fat products outsell Regular consistently:

Tier 3: Low Fat $306,807 vs. Regular $165,326 — widest gap, suggesting stronger health-consciousness in smaller cities (possibly driven by newer, aspirational consumer segments)
Tier 2: Low Fat $254,465 vs. Regular $138,686
Tier 1: Low Fat $215,048 vs. Regular $121,350

Counterintuitive insight: Tier 1 (metro cities) generates the lowest Low Fat sales — possibly because metros have more product diversity and regular items compete harder there.
4. Sales by Outlet Establishment Year
Outlets founded in 1998 generated the highest revenue ($204,522) — roughly 55% more than any subsequent cohort. All outlets founded after 2000 converge to a ~$130K band, with a notable trough in 2011 ($78,131). This pattern suggests 1998 outlets are significantly larger or in higher-footfall locations. The 2011 dip warrants investigation — likely reflects a batch of smaller-format stores opened that year.
5. Sales by Outlet Size

Medium outlets lead at 42.3% of total sales
Small outlets follow at 37.0% — surprisingly competitive
High (large) outlets account for only 20.7%

This is the most actionable finding: large-format stores are underperforming their expected revenue share. Medium outlets may have the optimal cost-to-revenue ratio, making them the preferred expansion format.
6. Sales by Outlet Location (City Tier)

Tier 3: $472,133 (39.3% of total)
Tier 2: $393,150 (32.7%)
Tier 1: $336,397 (28.0%)

Tier 3 cities are the biggest revenue contributor — despite being "smaller" markets. This likely reflects higher outlet density or lower competitive intensity in those markets.

🛠️ Tech Stack
Python 3.x
├── pandas          — data loading, cleaning, aggregation
├── numpy           — numerical operations
├── matplotlib      — base chart rendering, pie/donut/line charts
└── seaborn         — styled bar charts, grouped charts
