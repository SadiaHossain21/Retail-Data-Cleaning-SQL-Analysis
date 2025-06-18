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

- What products generate the highest revenue?
- Which countries have the most transactions?
- Are there customers that generate most of the business?
- What percentage of orders are canceled?

---

## Dataset Source

[UCI Machine Learning Repository – Online Retail](https://archive.ics.uci.edu/ml/datasets/online+retail)

---

## Author

**Sadia Hossain**  
MSc Data Science | SQL • Python • Power BI  
sadiahossain2101@gmail.com  
🔗 [LinkedIn Profile](https://linkedin.com/in/yourprofile)

---
