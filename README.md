# Sales_Analysis_YoY using Tableau Public

## Project Overview
This project features a fully interactive Year-over-Year (YoY) Sales Performance Dashboard built using Tableau Desktop Public. The goal was to provide an at-a-glance comparison of key sales metrics across years (2020–2023), enabling deep-dive analysis by product categories and regional breakdowns.
___________________________________
## Dashboard 
#### Explore the interactive visualization here: https://public.tableau.com/app/profile/irena.iverson/viz/SalesAnalysisYoY/SalesDashboard
The dashboard is fully dynamic:
- Tracks three primary KPIs: sales, profit, and quantity sold, all with YoY comparisons
- Includes interactive trendlines for both monthly and weekly views
- Provides comparative visuals for sales and profit by subcategory
- Features conditional formatting to highlight top and bottom months
- Displays dynamic bars for weekly data relative to average performance
  _________________________________
#### Interactive Filters
- Year selector covering 2020 to 2023
- Product category filter: Office Supplies, Furniture, Technology
- Region filter: East, South, West, Central
- Additional filters: State and City for local-level analysis
_______________________________
## Dataset & Data Model
The analysis was based on four separate CSV files integrated within Tableau:
- customers.csv – customer details including IDs, segments, and demographics
- location.csv – geographic data containing region, state, and city
- orders.csv – transactional data with order dates, quantities, sales, and profit
- products.csv – product catalog including category and subcategory information

Each dataset was connected using key fields such as Customer ID, Product ID, and Location ID to create a unified data model for analysis.

#### Data Model

The central table in this model is Orders.csv, which serves as the primary fact table containing transactional data. It is linked to three dimension tables — Customers.csv, Location.csv, and Products.csv — using inner joins based on unique identifiers.

This star-like structure allows efficient aggregation and filtering of sales and profit metrics by customer, product, and geographic attributes.
<img width="691" height="340" alt="Picture 2025-10-24 at 6 38 33 PM" src="https://github.com/user-attachments/assets/963d00b2-dcf8-4afa-852f-695b8ea30b26" />

________________________________
## Key Requirements

KPI Summary Overview
- Provide a high-level snapshot of total sales, profit, and quantity sold, comparing the current year to the previous year
- Include visual indicators for year-over-year changes, such as percentages and directional arrows

Monthly Performance Trends
- Display monthly progression for each KPI (sales, profit, quantity)
- Overlay current year data with the previous year for side-by-side comparison
- Clearly highlight the best and worst performing months for quick insight

Product Subcategory Breakdown
- Visualize performance across product subcategories, comparing this year’s sales to last year’s
- Include a dual view that reflects both sales and associated profit per subcategory
- Make underperforming or unprofitable subcategories stand out visually

Weekly Sales and Profit Analysis
- Show week-by-week fluctuations in sales and profit for the current year
- Calculate and display average weekly performance as a benchmark
- Use color cues or labels to spotlight weeks performing above or below average
  _________________________________
## Key Calculations used
- To be added
-   _________________________________
## Insights and Findings (2023 vs. 2022)

Sales

- Sales totaled $733.2K in 2023, a 20.4% increase over 2022
- Phones, chairs, and binders led sales performance
- December marked the highest sales month, while February was the lowest

Profit

- Profit rose to $93.4K, up 14.2% year-over-year
- Accessories, appliances, and labels showed negative profit, warranting further review

Quantity

- Quantity sold reached 12.5K units, a 26.8% increase from the previous year

All visualizations update based on filter selections, allowing for targeted, real-time analysis.

<img width="1394" height="796" alt="Picture 2025-10-24 at 1 37 16 PM" src="https://github.com/user-attachments/assets/e774c2aa-929b-4513-be52-e1974dfe5e53" />
<img width="1381" height="794" alt="Picture 2025-10-24 at 1 37 49 PM" src="https://github.com/user-attachments/assets/a21e0e76-ffce-466d-8be7-7c6017af9543" />


