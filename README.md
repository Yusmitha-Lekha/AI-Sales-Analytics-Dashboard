# 🤖 AI-Enhanced Sales Analytics Dashboard (SQL + Python + Power BI)

## 📌 Project Overview

This project performs end-to-end retail sales analysis using SQL, Python, and Business Intelligence tools.  

The objective is to simulate a real-world **AI-enabled Data Analyst workflow**:

Raw CSV Data → SQL Data Modeling → Business KPI Analysis → Time-Series Insights → Dashboard Visualization → Executive Summary

The dataset contains **9,800 retail transactions** across multiple regions and product categories.

---

## 🛠 Tools & Technologies

- **MySQL** – Data import, cleaning, KPI calculation
- **SQL** – Aggregations, GROUP BY, date transformations
- **Python (Planned Phase)** – EDA & forecasting
- **Power BI (Planned Phase)** – Interactive dashboard
- **AI (Planned)** – Automated executive insight generation

---

## 📂 Dataset Information

- Records: 9,800
- Regions: West, East, Central, South
- Categories: Technology, Furniture, Office Supplies
- Fields: Sales, Order Date, Customer Name, State, Segment, etc.

---

# 📊 SQL Business Analysis Results

## 💰 Total Revenue
**$2,261,536.78**

---

## 🌎 Revenue by Region

| Region  | Revenue |
|----------|----------|
| West     | $710,219.68 |
| East     | $669,518.73 |
| Central  | $492,646.91 |
| South    | $389,151.46 |

**Insight:**  
West region leads revenue generation, while South underperforms — indicating geographic optimization opportunities.

---

## 🛍 Revenue by Category

| Category         | Revenue |
|------------------|----------|
| Technology       | $827,455.87 |
| Furniture        | $728,658.58 |
| Office Supplies  | $705,422.33 |

**Insight:**  
Technology is the highest-performing category, contributing the largest share of revenue.

---

## 📅 Time-Series Analysis

Converted text-based dates into structured format using:

```sql
DATE_FORMAT(STR_TO_DATE(`Order Date`, '%m/%d/%Y'), '%Y-%m')
