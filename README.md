# Online Retail Data Cleaning & SQL Analysis Project

A full-cycle data cleaning and SQL analytics project based on the UCI Online Retail dataset. This project demonstrates the end-to-end skills of data wrangling, transformation, and SQL-based business analysis using PostgreSQL and Python.

---

## Objectives

- Clean messy real-world retail data with missing values, invalid entries, and duplicate records
- Create new engineered features such as cancellation flags
- Export clean data for SQL querying
- Perform structured SQL analysis to extract valuable business insights

---

## Project Files

- `Online Retail.xlsx` – Raw dataset from UCI repository
- `OnlineRetail_Clean.csv` – Final cleaned Excel file
- `data-cleaning-preparation.ipynb` – Jupyter Notebook for data cleaning using Python
- `SQL Queries.ipynb` – SQL-based data exploration and analysis using PostgreSQL

---

## Data Cleaning & Preparation (Python + Pandas)

Key steps included:
- Converted `InvoiceDate` to datetime format
- Filled missing descriptions with "Unknown"
- Converted `CustomerID` to string format
- Created `IsCancelled` column to flag canceled transactions (based on invoice prefix "C")
- Removed rows with invalid prices or quantities
- Exported cleaned dataset to `.xls` and `.csv` formats

>  Notebook: `data-cleaning-preparation.ipynb`

---

## SQL Analysis (PostgreSQL + SQLAlchemy)

- Loaded cleaned data into PostgreSQL using SQLAlchemy
- Performed analysis with SQL queries to answer business questions:

### Key Insights
- **Top 10 Products by Revenue**
- **Number of Orders per Country**
- **Most Active Customers**
- **Seasonal Trends** (Optional to expand)

>  Notebook: `SQL Queries.ipynb`

---

## Tools & Technologies

- **Python** (Pandas, NumPy)
- **SQL** (PostgreSQL)
- **SQLAlchemy** (database connection)
- **Excel** (initial exploration)
- **Jupyter Notebook**

---

## Sample Business Questions Answered

-  **Which products generate the highest revenue?**  
  → Identified top 10 products using revenue aggregation (`SUM(revenue)`)

-  **Which countries have the most transactions and revenue?**  
  → Analyzed `COUNT(DISTINCT InvoiceNo)` and `SUM(revenue)` grouped by `Country`

-  **Who are the most valuable customers?**  
  → Calculated Customer Lifetime Value and top 3 customers by country (window function)

-  **What percentage of orders are canceled?**  
  → Used flags on `InvoiceNo` and calculated cancellation rates by country

-  **Which products are most frequently returned?**  
  → Queried canceled transactions grouped by `Description`

-  **Are there seasonal or monthly sales trends?**  
  → Grouped by `yearmonth` to assess revenue trends over time

-  **What is the average order value and how do orders segment by spend?**  
  → Derived using subqueries and case conditions for "High Value" vs "Regular"

-  **When are customers most active during the day?**  
  → Extracted order timestamps to identify peak purchase hours

-  **How many customers are repeat buyers?**  
  → Classified customers as “Repeat” or “One-Time” using invoice counts

---

## Dataset Source

[UCI Machine Learning Repository – Online Retail](https://archive.ics.uci.edu/ml/datasets/online+retail)

---

## Author

**Sadia Hossain**  
MSc Data Science | SQL • Python • Power BI  
sadiahossain2101@gmail.com  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/sadia-hossain-297993251/)

---
