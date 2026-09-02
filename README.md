# Customer Churn Data Analysis

## 📌 Project Overview

This project focuses on analyzing customer churn data using Python, Pandas, and SQLite.

The main objective of this project is to build a structured data analysis workflow starting from loading data from a SQLite database and preparing clean datasets for further analysis, feature engineering, exploratory data analysis, and machine learning.

Currently, the project includes:

# Data Loading
- The raw data is stored in a SQLite database:

-customer_churn.db
The database was connected using Python's sqlite3 library.
The tables were loaded into Pandas DataFrames for further processing.

# Data Cleaning
- The data cleaning process was performed to improve data quality and prepare the datasets for further analysis.

The following cleaning operations were performed:
1. Removing Unnecessary Columns
Columns that were not required for analysis were identified and removed from the datasets.

This helps:

Reduce unnecessary data
Improve dataset readability
Make analysis more efficient

# Data Type Conversion
- Columns were converted into appropriate data types.

For example:

Date columns → datetime
Numerical columns → int or float
Text columns → string
Proper data types are important for accurate analysis and feature engineering.

# Data Standardization
Data values and formats were standardized to maintain consistency across the datasets.

This process helps reduce inconsistencies caused by:

Different text formats
Inconsistent naming
Different value representations
Formatting issues

# Saving Cleaned Data
After completing the cleaning process, the cleaned datasets were saved separately.

The cleaned datasets include:

df_customer_cleaned.parquet
df_subscription_cleaned.parquet
df_support_cleaned.parquet

Parquet format was used because it provides advantages such as:

Preserving data types
Faster data loading
Efficient storage
Better performance for analytical workflows

---

## 📂 Project Structure

```text
churn_data_analysis/
│
├── cleaned_data/
│   ├── df_customer_cleaned.parquet
│   ├── df_subscription_cleaned.parquet
│   └── df_support_cleaned.parquet
│
├── db/
│   └── customer_churn.db
│
├── notebook/
│   ├── data_cleaning.ipynb
│   └── feature_engineering.ipynb
│
├── .gitignore
├── .gitattributes
└── README.md

