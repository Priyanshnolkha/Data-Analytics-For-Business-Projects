BlinkIT Grocery Sales Dashboard

📌 Project Overview

The BlinkIT Grocery Sales Dashboard is an interactive Business Intelligence project developed using Power BI to analyze BlinkIT grocery sales and outlet performance. The dashboard provides a consolidated view of sales, item counts, ratings, item visibility, outlet characteristics, and category-level performance.

The project also demonstrates the integration of a MySQL database with Power BI, using Power Query for data connection and transformation and DAX for analytical measures and interactive dashboard controls.

🎯 Objectives

Analyze overall BlinkIT sales performance across outlets.

Identify high-performing item categories and outlet types.

Compare sales across outlet location tiers and outlet sizes.

Analyze the impact of item fat content on sales.

Track outlet establishment performance from 2012 to 2022.

Monitor key measures such as Total Sales, Avg Sales, No. of Items, and Avg Rating.

Build an interactive dashboard using slicers and toggle buttons.

Connect Power BI with MySQL for structured and refreshable reporting.

Support data-driven retail and outlet-management decisions.

🛠️ Tools & Technologies

Power BI Desktop - Dashboard development and visualization

Power BI Service - Dashboard publishing and online sharing

MySQL - Database storage and management

Power Query - Data connection, cleaning, and transformation

DAX - Measures and field-parameter calculations

Excel - Initial/source data preparation

📊 Dataset

The project uses BlinkIT Grocery sales data sourced from a MySQL database named blinkit_db and loaded into Power BI through Power Query.

Each row represents an item sold at a specific outlet.

Important Columns

Item Fat Content - Low Fat or Regular

Item Identifier - Unique item code

Item Type - Product category such as Fruits and Vegetables, Snack Foods, Household, Dairy, Frozen Foods, and others

Outlet Establishment Year - Year in which the outlet was established

Outlet Identifier - Unique outlet code

Outlet Location Type - Tier 1, Tier 2, or Tier 3

Outlet Size - Small, Medium, or High

Outlet Type - Grocery Store, Supermarket Type1, Supermarket Type2, or Supermarket Type3

Sales - Sales value used for business analysis

Item Visibility - Visibility measure for items

Rating - Customer rating measure

🧹 Data Cleaning & Transformation

The data was connected to Power BI using:

Get Data → MySQL Database → blinkit_db.blinkit_grocery

The following Power Query transformations were applied:

Previewed and validated the incoming table.

Promoted the first row to column headers.

Correctly assigned data types to text, whole-number, and decimal fields.

Verified that the dataset contained no fully blank rows.

Renamed the query to BlinkIT Grocery Data.

Loaded the cleaned data into the Power BI model.

🗄️ Data Modelling

The project uses a single cleaned fact table:

BlinkIT Grocery Data

The table contains:

Item Fat Content

Item Identifier

Item Type

Outlet Establishment Year

Outlet Identifier

Outlet Location Type

Outlet Size

Outlet Type

Sales

Item Visibility

Rating

No additional dimension tables were required. Slicers and visuals directly use fields from the single table, keeping the model simple and performant.

📐 DAX Measures & KPIs

A DAX field parameter called metrics was used to allow the dashboard to switch between:

Total Sale

Avg Sales

No Of Items

Avg Rating

This parameter powers the interactive toggle buttons used with the main Fat Content and Item Type visuals.

Main KPI Values

KPI

Value

Total Sales

$1.20M

Avg Sales

$141

No. of Items

8,523

Avg Rating

3.9

🔌 MySQL Integration

The BlinkIT data was connected from MySQL to Power BI using the following connection:

MySQL Server
     ↓
blinkit_db
     ↓
blinkit_grocery
     ↓
Power Query
     ↓
Power BI Data Model
     ↓
BlinkIT Grocery Sales Dashboard

Power BI used the MySQL connection:

= MySQL.Database("127.0.0.1:3306", "blinkit_db", [ReturnSingleDatabase=true])

This setup makes the dashboard suitable for database-based reporting and future refreshable data connections.

📈 Dashboard Features

The dashboard contains:

Total Sales KPI Card

Avg Sales KPI Card

No. of Items KPI Card

Avg Rating KPI Card

Outlet Establishment Trend from 2012 to 2022

Total Sale by Fat Content using a Donut Chart

Fat Content by Outlet Location Tier using a Bar Chart

Total Sale by Item Type using a Bar Chart

Outlet Size Distribution using a Donut Chart

Total Sale by Outlet Location Tier using a Bar Chart

Detailed Outlet Type Table

Interactive slicers for:

Outlet Location Type

Outlet Size

Item Type

Toggle buttons for:

Total Sale

Avg Sales

No. of Items

Avg Rating

💡 Key Business Questions

The dashboard is designed to answer:

What is the overall sales performance across all BlinkIT outlets?

Which outlet establishment year produced the strongest sales performance?

Do Regular or Low Fat items generate more sales across outlet tiers?

Which item categories should receive more shelf space and promotional focus?

Which outlet size and location tier contribute the most to sales?

Which outlet type is the strongest performer?

Are there outlet formats with unusually high visibility or other performance characteristics?

🔍 Key Insights

BlinkIT generated $1.20M in total sales from 8,523 items, with $141 average sales and an average rating of 3.9.

Outlets established around 2018 showed the strongest performance, reaching approximately $205K in the establishment trend.

Regular items generated more sales than Low Fat items, at approximately $776.32K versus $425.36K.

Fruits and Vegetables and Snack Foods were the strongest item categories, at approximately $0.18M each.

Seafood and Breakfast contributed the least sales among the highlighted categories.

Small-format outlets generated the highest total sales at approximately $507.90K.

Tier 3 outlets led location-based sales with approximately $472.13K.

Supermarket Type1 was the strongest outlet type, generating approximately $787.55K in sales.

Grocery Stores showed relatively high item visibility (0.10) despite carrying fewer items, suggesting an efficient and focused assortment.

📌 Business Recommendations

Increase shelf space and promotional activity for Fruits and Vegetables and Snack Foods.

Review the assortment strategy for lower-performing categories such as Seafood and Breakfast.

Investigate the operating model of outlets established around 2018 and identify successful factors that can be replicated.

Study the Small-format outlet strategy and apply useful assortment or space-management practices to Medium outlets.

Use the Grocery Store format's high item visibility as a benchmark for improving product discoverability.

Continue monitoring Avg Rating alongside Total Sale so that outlets with increasing sales but declining ratings can be identified early.

☁️ Power BI Service

The completed BlinkIT dashboard was published to the Blinkit Dashboard workspace in Power BI Service for online access and sharing.

Power BI Service:
View BlinkIT Dashboard in Power BI Service

Note: The exact report URL is not included in the project report provided for this README, so the generic Power BI Service link is used here.

🔗 Project Repository

GitHub Repository:
https://github.com/Priyanshnolkha/Data-Analytics-For-Business-Projects/tree/main/Final_Project_Blinkit_Grocery_Dashboard

📁 Suggested Project Structure

Final_Project_Blinkit_Grocery_Dashboard/
│
├── README.md
├── BlinkIT Dashboard.pbix
├── BlinkIT Grocery Data.xlsx
├── SQL/
│   └── blinkit_grocery.sql
│
└── Screenshots/
    └── BlinkIT_Dashboard.png

The exact filenames may differ from the final repository contents.

🚀 Conclusion

The BlinkIT Grocery Sales Dashboard delivers an end-to-end Business Intelligence solution for grocery retail analysis. The project connects item- and outlet-level data from MySQL, performs cleaning and transformation in Power Query, uses a single Power BI data model, and applies a DAX field parameter to create interactive metric switching.

The final dashboard enables management to move from overall performance to outlet type, location tier, item category, and product-related analysis through interactive filters and visuals. These insights can support assortment planning, outlet expansion, visibility improvement, and data-driven retail decision-making.
