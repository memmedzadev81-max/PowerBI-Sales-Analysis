# Power BI Sales Analysis Dashboard

This project is a Power BI dashboard created for analyzing sales data from 2024-2025.

## About the Project

I prepared this analysis as a junior data analyst to gain practical experience. The data covers sales across different regions of Azerbaijan (Baku, Ganja, Sumgayit, Lankaran, Shaki).

### Key Metrics (KPIs)
- Total Sales Volume
- Total Profit (Sales - Cost)
- Average Order Value
- Discount Impact
- Performance by Region and Category

### Dashboard Pages
1. **Overview** – Main KPI cards, sales trend (line chart), region map
2. **Product Performance** – Bar charts by category and product, top 10 products
3. **Customer Analysis** – Customer segmentation, repeat purchases
4. **Regional Deep Dive** – Detailed view with region filters

## Setup Instructions

1. Import the `data/sales_data.csv` file into Power BI Desktop
2. Create a Date table in the data model (based on OrderDate)
3. Add the DAX measures from the `measures/` folder
4. Build the visuals as described in the documentation

## Data Source
- 50 sample order records (can be easily expanded)
- Date range: January 2024 – August 2025
- Fields: OrderID, OrderDate, Region, Category, Product, Customer, Quantity, UnitPrice, Discount%, SalesAmount, Cost

## Note
This project is for training purposes only. It does not contain real business data.  
If you have any questions, feel free to open an issue or contact me.

---
Vusal Mammadzade  
Junior Data Analyst  
