🧾 Retail Sales Data Analysis – End-to-End Project
📊 Overview

This project demonstrates a complete data analytics workflow — from data collection to cloud integration and visualization — using Python, PostgreSQL, Snowflake, and Power BI.

🧩 Steps Involved
1️⃣ Dataset Collection

Downloaded raw retail dataset from Kaggle / generated sample data using ChatGPT.

The dataset contains information such as Order ID, Customer, Region, Category, Quantity, Price, and Order Date.

2️⃣ Data Cleaning & Preprocessing (Jupyter Notebook)

Loaded the raw dataset into Jupyter Notebook using Python’s pandas library.

Performed the following data cleaning steps:

✅ Removed duplicate records.

✅ Formatted Date columns into proper DD-MM-YYYY format.

✅ Handled and filled missing (null) values appropriately.

Saved the cleaned dataset back to CSV.

3️⃣ Data Enhancement in Excel

Further refined and verified data using Microsoft Excel:

Calculated Revenue using the formula:

=Quantity * Price


Applied Conditional Formatting to highlight:

Revenue > 3000 (highlighted in green or bold).

Created Pivot Tables & Charts for:

📈 Revenue by Category

🌍 Revenue by Region

Added Slicers based on Region for dynamic filtering.

4️⃣ Database Integration (PostgreSQL)

Created a new PostgreSQL database.

Imported the cleaned CSV data into a table named sales_data.

Executed SQL queries to derive insights such as:

Total revenue by region/category.

Top-performing products.

Nth highest sales analysis.

5️⃣ Data Visualization (Power BI)

Connected Power BI directly to the PostgreSQL database.

Designed an interactive dashboard with:

🧩 Decomposition Tree to explore revenue breakdowns.

🔍 Slicers for region and category filtering.

💳 Cards for key metrics (Total Revenue, Average Order Value, etc.).

📈 Line and Bar Charts for revenue trends and comparisons.

6️⃣ Cloud Integration (Snowflake)

Set up a Snowflake environment for cloud-based analytics.

Created:

A database, schema, and table for SALES_DATA.

File format and stages for data loading.

Loaded cleaned data from local CSV to Snowflake using Python (Snowflake Connector).

Wrote and executed an upsert (MERGE) script to:

Automatically insert new records.

Update modified records without duplication.

⚙ Tools & Technologies Used
Category	Tool/Technology
Data Source	Kaggle / ChatGPT
Data Cleaning	Python (Pandas), Excel
Database	PostgreSQL
Visualization	Power BI
Cloud Data Warehouse	Snowflake
IDE/Notebook	Jupyter Notebook
Languages	Python, SQL

🚀 Key Highlights

End-to-end pipeline from raw data → insights → cloud → visualization.

Real-time data updates handled via Snowflake upsert script.

Integration between Excel, Python, PostgreSQL, and Power BI for complete analytics workflow.
