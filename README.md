# Inventory Management Dashboard

**Dataset:** UCI Online Retail II (Chen et al., 2019)  
**Records:** ~8,000 transactions · 20 products · 7 countries  
**Source:** [UCI ML Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

## What this project covers

A UK-based online gift retailer wants to optimise inventory decisions — identifying slow-moving stock, seasonal demand patterns, reorder alerts, and top revenue drivers.

- **Stock status alerts** — critical, low, and adequate inventory mapped against reorder points
- **Revenue analysis** — by product, category, and country with trend lines
- **Seasonality heatmap** — demand patterns across products and months
- **Reorder planning** — days of stock remaining and ABC analysis
- **Executive dashboard** — 6 KPIs, revenue trend, category split, and live reorder alert panel

## Dashboard Visualizations

### 1. Stock Status Overview
![Stock Status Dashboard](Images/01_stock_status.png)
*Real-time inventory status showing critical, low, and adequate stock levels mapped against reorder points.*

### 2. Revenue & Demand Analysis
![Revenue and Demand](Images/02_revenue_demand.png)
*Product revenue performance and demand trends by category and geography.*

### 3. Seasonality Heatmap
![Seasonality Patterns](Images/03_seasonality.png)
*Demand patterns across products and months, highlighting peak seasons for planning.*

### 4. Reorder Planning
![Reorder Planning](Images/04_reorder_planning.png)
*Days of stock remaining, ABC analysis, and automated reorder triggers.*

### 5. Executive Dashboard
![Executive Dashboard](Images/05_executive_dashboard.png)
*High-level KPIs, revenue trends, category distribution, and live reorder alerts.*

## How to run

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook inventory_dashboard.ipynb
```

## Files

```
inventory_mgmt/
├── inventory_dashboard.ipynb     # Main notebook
├── online_retail_inventory.csv   # Dataset (UCI-faithful structure)
├── Images/                       # Dashboard screenshots
│   ├── 01_stock_status.png
│   ├── 02_revenue_demand.png
│   ├── 03_seasonality.png
│   ├── 04_reorder_planning.png
│   └── 05_executive_dashboard.png
└── README.md
```

## Key findings

- Top 4 products drive ~70% of revenue (classic Pareto/ABC concentration)
- November–December drives a ~80% spike in order volumes — buffer stock critical by October
- UK accounts for 82% of revenue; Germany and France are the strongest international markets
- Automated reorder triggers below 14 days of stock would eliminate most stockout risk
