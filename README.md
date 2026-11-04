# Retail Sales Performance Dashboard (Power BI)

An interactive Power BI dashboard analyzing 12,000 retail orders across regions, product categories, sales channels and discount levels. It answers the questions a business team asks every day: What are we selling? Where? Through which channel? And is it actually profitable?

🌱 This was my very first Power BI dashboard, built during my Power BI learning journey. If you're a learner looking for a comfortable, beginner-friendly dataset to start building dashboards, this is a great one to begin with. 



## Dashboard Preview
![Sales Performance Dashboard](images/dashboard_overview.png)

A PDF export of the full dashboard is also included:
![Sales Performance Dashboard](Dashboard/Retail_Sales_Dashboard.pdf)

## Key Metrics at a Glance
| KPI | Value |
|---|---|
| Total Sales | **$1.98M** |
| Total Profit | **$614.17K** |
| Total Orders | **12K** |
| Avg. Order Value | **$165.32** |
| Average Profit (per order) | **$51.18** |
| Avg. Customer Rating | **4.19 / 5** |

## Dashboard Features

- KPI cards: sales, profit, orders, average order value, average profit and customer rating
- Sales Trend: monthly total sales vs. total profit (area chart)
- Sales by Category: donut chart across 7 product categories
- Sales by Region: column chart across 6 regions
- Sales by Channel: Mobile App vs. Physical Store vs. Website
- Top Products by Sales: table with total sales, total profit and profit margin
- Discount Impact: how discount bands (No Discount, 1-10%, 11-20%, 21-30%) affect sales and profit
- Slicers: filter everything by Time Period, Region and Category, with a reset button

## Key Insights

- Electronics dominates, contributing about 45% of total sales ($900K).
- North America is the top region ($0.61M), followed by Europe ($0.52M) and Asia ($0.47M).
- Mobile App (41.7%) and Website (39.6%) together drive over 80% of sales; physical stores contribute under 19%.
- Sales peak in November, with a sharp rise from October, consistent with a festive/holiday shopping spike.
- Profit margin varies a lot by product: Dress (47.5%) and Jacket (47.2%) earn far higher margins than high-revenue electronics such as Tablet (17.8%), Webcam (18.0%) and Bluetooth Speaker (17.6%).
- Most revenue comes from orders with no discount (about $1.1M+), and sales fall as discount bands get deeper.

## Repository Contents

| File | Location | Description |
|---|---|---|
| `Retail_Sales_Dashboard.pbix` | `dashboard/` | Power BI Desktop project file (open this to explore and edit) |
| `Retail_Sales_Dashboard.pdf` | `dashboard/` | Static PDF export of the dashboard |
| `retail_sales_dataset.csv` | `Data/raw` | Raw dataset (CSV) |
| `retail_sales_dataset.xlsx` | `Data/cleaned` | Cleaned dataset (Excel) |
| `dashboard.png` | `images/` | Dashboard preview screenshot |


## Dataset Overview

- **Rows:** 12,000 orders
- **Columns:** 19
- **Period:** January 2024 – December 2025 (2 years of daily orders)
- **Regions:** Africa, Asia, Europe, North America, Oceania, South America
- **Categories:** Beauty, Books, Clothing, Electronics, Home & Kitchen, Sports, Toys
- **Products:** 42 unique products

| Column | Description |
|---|---|
| `order_id` | Unique order identifier |
| `order_date` | Date the order was placed |
| `customer_id` | Customer identifier |
| `customer_age` | Customer age |
| `gender` | Male / Female / Other |
| `region` | Customer region |
| `product_category` | Product category |
| `product_name` | Product name |
| `unit_price` | Price per unit |
| `quantity` | Units ordered |
| `discount_pct` | Discount applied (%) |
| `order_channel` | Website / Mobile App / Physical Store |
| `payment_method` | Credit Card, Debit Card, UPI/Wallet, Cash on Delivery, Gift Card |
| `shipping_cost` | Shipping charge |
| `delivery_days` | Days taken to deliver |
| `returned` | Whether the order was returned (Yes/No) |
| `customer_rating` | Rating given (1-5) |
| `total_amount` | Final order amount (sales) |
| `profit` | Profit on the order |

## Tools & Skills Used

- **Python (Pandas)** – Data cleaning, manipulation, and exploratory data analysis.
- **Power BI Desktop** – Interactive dashboard development and data visualization.
- **Power Query** for data transformation and preparation.
- **DAX** for measures (total sales, total profit, average order value, profit margin, etc.)
- **Data modelling & visualisation**: KPI cards, area/column/donut charts, tables, slicers
- **Dashboard design**: layout, colour theme and consistent formatting

---

## Learn With This Project

New to Power BI? This dataset is a comfortable place to start because it is:

-  **Clean and well-structured**: one flat table, no complex joins needed
-  **Rich enough to be interesting**: dates, geography, categories, channels, discounts, ratings and profit
-  **Realistic business context**: the kind of questions you'll see in real analyst work
-  **Small enough to stay fast**: 12K rows load instantly

**Practice ideas to go beyond this dashboard:**

1. Build a **date table** and use time-intelligence DAX (YoY, MoM, YTD)
2. Analyse **return rates** by category or product
3. Explore **delivery days vs. customer rating**
4. Segment customers by **age group and gender**
5. Compare **payment methods** and their share of sales
6. Add a **drill-through page** for product-level detail
7. Try **bookmarks, tooltips and conditional formatting**

Feel free to fork this repo, reuse the dataset and build your own version. 

---

## Future Improvements

- Add return-rate and delivery-performance pages
- Customer demographics analysis (age and gender)
- Year-over-year comparison and forecasting
- Publish to Power BI Service with scheduled refresh

---
