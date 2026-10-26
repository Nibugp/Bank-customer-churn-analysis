## Project Overview

An end-to-end business analytics project using SQL and Power BI to analyse bank customer churn, 
identify customer segments associated with higher churn and support data-driven retention decisions.

## Business Problem
Customer churn can affect a bank's ability to maintain customer relationships and retain deposits.
The business wants to:
Identify customers likely to churn
Understand the impact of credit score, age, balance, and products on churn
Analyze churn patterns across geographic regions
Compare active vs inactive customer behavior.

## Dataset
- **Source:** Bank Customer Churn Dataset 
- **Domain:** Banking & Customer Retention
- **Format:** CSV
- **Records:** 10,000 customers

### Data Dictionary
| Column | Description |
|---|---|
| `CustomerId` | Unique customer identifier |
| `CreditScore` | Customer credit score |
| `Geography` | Country of the customer |
| `Gender` | Customer gender |
| `Age` | Customer age |
| `Tenure` | Number of years with the bank |
| `Balance` | Customer account balance |
| `NumOfProducts` | Number of bank products held |
| `HasCrCard` | Whether the customer has a credit card |
| `IsActiveMember` | Customer activity status |
| `EstimatedSalary` | Estimated annual salary |
| `Exited` | Customer churn status (1 = churned, 0 = retained) |

## Tools & Technologies
SQLite / SQLiteStudio — Data validation and SQL analysis

SQL — Data cleaning, aggregation, segmentation, and window functions

Power BI — Interactive dashboard and business insights

GitHub — Project documentation and portfolio

## **Data Validation and Cleaning**
Initial data-quality checks covered record counts, column inspection, data types, missing values, 
and duplicate customer identifiers.
Initial Observations :
Total records: 10,000 customers.
Missing values: 3 missing values in Surname.
Invalid values: 3 records in EstimatedSalary contain -999999, which requires investigation.
Data types: SQLite initially reported all imported columns as TEXT.
Duplicate records: No duplicate CustomerId values were found in the initial check.

## Key Performance Indicators (KPIs)

| KPI | Business Purpose |
|---|---|
| Total Customers | Measures the customer base |
| Churned Customers | Counts customers who exited |
| Retained Customers | Counts customers who did not exit |
| Churn Rate | Measures the percentage of customers who exited |
| Retention Rate | Measures the percentage of customers retained |
| Churn by Geography | Compares churn across geographic groups |
| Churn by Activity Status | Examines churn among active and inactive customers |
| Churn by Age Group | Identifies demographic patterns |
| Average Balance by Churn Status | Compares balances of churned and retained customers |
| Balance Associated with Churn | Sums the balances of customers who exited |
| Segment Churn Rate | Measures churn within a defined customer segment |

## Analysis Areas

- Overall customer churn and retention
- Geographic churn patterns
- Customer engagement and activity
- Age-group analysis
- Account balance and product relationships
- High-churn segment identification and retention prioritisation
- Customer segment ranking using SQL window functions

## Key Insights

## Conclusions







