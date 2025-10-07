# Sales Data Analysis & Visualization Project

## 📊 Overview
This project demonstrates a complete **end-to-end data analysis pipeline** — from data cleaning to dashboard visualization. The workflow involves using **Python, Excel, PostgreSQL, Snowflake, and Power BI** to process and visualize sales data.

---

## 🧩 Steps Involved

### 1. 📥 Data Collection
- Downloaded the **raw sales dataset** from **Kaggle**.
- The dataset contained fields such as `OrderDate`, `Customer`, `Category`, `Region`, `Quantity`etc...

---

### 2. 🧹 Data Cleaning (Python)
Used **Python (Pandas)** for cleaning and preprocessing:
- Removed **duplicate rows**.
- Handled **missing values** appropriately.
- Standardized **date formats** (e.g., converted `mm/dd/yyyy` → `yyyy-mm-dd`).
- Verified column data types and renamed columns where necessary.

---

### 3. 📘 Data Enhancement (Excel)
Performed further data enhancement in **Excel**:
- Added a **new calculated column**:  
  `Revenue = Quantity × Unit_Price` (if not present).
- Applied **Conditional Formatting** to highlight:
  - Revenue > 3500 (colored green).
- Created **Pivot Tables** and **Pie Charts** on new sheets:
  - **Revenue by Category**
  - **Revenue by Region**

Saved the final version as **`sales_data_cleaned.csv`**.

---

### 4. 🐘 Data Loading (PostgreSQL)
- Imported the cleaned CSV file into **PostgreSQL** using `COPY` command.
- Created a table named `sales_data`.
- Wrote **5–7 SQL queries** for analysis, including:
  - Total revenue by region.
  - Top 5 customers by revenue.
  - Monthly sales trend.
  - Average revenue per category.
  - Total quantity sold by region.

---

### 5. 📈 Power BI Dashboard (PostgreSQL)
- Connected Power BI Desktop to PostgreSQL.
- Imported the `sales_data` table.
- Designed an interactive dashboard featuring:
  - **Decomposition Tree**
  - **Cards** (for KPIs like Total Revenue, Average Revenue)
  - **Pie Chart** (Revenue by Region)
  - **Bar Chart** (Revenue by Category)
  - **Line Chart** (Revenue over Time)
  - **Slicer** (Filter by Region or Category)

<img width="1308" height="723" alt="Dashboard_1" src="https://github.com/user-attachments/assets/9280b3dc-b148-42dc-b2e5-1efff3f04632" />


### 6. ☁️ Cloud Integration with Snowflake
- Alternatively, the Excel-modified dataset was uploaded to **Snowflake** for cloud-based storage.
- Created a database: `SALES_PROJECT`
- Schema: `CLEANED_DATA`
- Table: `SALES_DATA`
- Connected Power BI to Snowflake via:
  - Server: `OGJVEXN-HI94808.snowflakecomputing.com`
  - Warehouse: `MY_WH`
  - Database: `SALES_PROJECT`
  - Schema: `CLEANED_DATA`

Reused the same Power BI **dashboard template** for visualization on Snowflake data.

---

## 🧠 Tools & Technologies Used
| Tool | Purpose |
|------|----------|
| **Kaggle** | Source of raw dataset |
| **Python (Pandas)** | Data cleaning & preprocessing |
| **Excel** | Data enhancement & visualization |
| **PostgreSQL** | Local data storage and SQL querying |
| **Snowflake** | Cloud data storage |
| **Power BI** | Dashboard design and business insights |

---

## 📸 Dashboard Components
- Decomposition Tree (category->products)
- KPI Cards (Total Revenue, unitprice)
- Pie Chart (Revenue by Region)
- Bar Chart (Revenue by Category)
- Line Chart (Monthly Revenue Trend)
- Slicer (Interactive filtering)

---

## ✅ Conclusion
This project showcases a full analytics workflow:
- **Data Cleaning → Data Transformation → SQL Analysis → BI Visualization**
- Demonstrates working knowledge of **Python, Databases, Cloud, and Power BI integration**.

