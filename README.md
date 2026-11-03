## Project Overview

An end-to-end business analytics project using SQL and Power BI to analyse customer churn patterns, 
identify customer segments associated with higher churn and develop data-driven recommendations for customer retention.

## Business Problem

Customer churn can affect a bank's ability to maintain customer relationships and retain deposits.

For this case study, the analysis aims to:

- Understand how credit score, age, account balance, and number of products relate to customer churn.

- Analyze churn patterns across different geographic regions.

- Compare customer churn behaviour between active and inactive members.

- Identify high-churn customer segments and highlight areas for targeted retention strategies.

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
SQLite / SQLiteStudio — Data validation,cleaning and SQL analysis

Power BI — Interactive dashboard and business insights

GitHub — Project documentation and portfolio

## **Data Validation and Cleaning**
Initial data-quality checks covered record counts, column inspection, data types, missing values, 
and duplicate customer identifiers.
Initial Observations :

-Total records: 10,000 customers.

-Missing values: 3 missing values in Surname.

-Invalid values: 3 records in EstimatedSalary contain -999999, which requires investigation.

-Data types: SQLite initially reported all imported columns as TEXT.

-Duplicate records: No duplicate CustomerId values were found in the initial check.

Cleaning Actions :

- Missing values: Reviewed the 3 missing values in Surname.
  Since this column was not required for the churn analysis, it was excluded from the analytical queries.
  
- Invalid salary values: Replaced the 3 invalid EstimatedSalary values (-999999) with NULL to avoid treating
  them as genuine salary values.
  
- Data types: Used appropriate type casting in SQL queries to handle numeric columns initially imported as TEXT.
  
- Duplicate records: Verified that no duplicate CustomerId values were present.
  
- Data validation: Rechecked record counts and missing or invalid values after cleaning to ensure data consistency.

## Key Performance Indicators (KPIs) and Analytical Measures

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

- Overall churn: 2,037 out of 10,000 customers exited, resulting in an overall churn rate of 20.37%.

- Geographic pattern: Germany recorded the highest churn rate at 32.44%, compared with Spain at 16.67% and France at 16.15%.

- Customer activity: Inactive customers had a churn rate of 26.85%, compared with 14.27% among active customers.

- Age group: Customers aged 51–60 recorded the highest churn rate at 56.21%, followed by the 41–50 age group at 33.98%.

- Product relationship: Customers holding three products had an 82.71% churn rate, while those holding four products had a 100% churn rate.   These groups had relatively small customer counts.

- Account balance: Churned customers had an average balance of 91,108.54, compared with 72,745.30 among retained customers.

- Priority segments: Inactive customers aged 41–50 in Germany and France contributed the largest numbers of churned customers among the analysed combinations.

## Conclusions

The analysis shows that customer churn is concentrated in particular geographic, age, activity, and product segments rather than being evenly distributed across the customer base.

The findings provide the bank with a basis for prioritising further investigation into customer engagement, product suitability, and customer experience. Targeted retention initiatives can then be developed and evaluated using appropriate customer and service data.





