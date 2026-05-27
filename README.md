# Banking Analytics Dashboard using SQL & Power BI

An end to end banking analytics project focused on customer behavior analysis, transaction monitoring, account insights, and financial trend visualization using SQL Server and Power BI.

---

## Dashboard Preview

<img width="1905" height="1064" alt="Dashboard Preview" src="YOUR_IMAGE_LINK_HERE">

---

# Project Overview

This project focuses on building a complete banking analytics workflow using SQL Server and Power BI.

The project includes:
- Synthetic data generation
- SQL-based data cleaning
- Data integration using joins
- Power Query transformations
- KPI creation using DAX
- Interactive dashboard development

The final dashboard provides insights into:
- Customer demographics
- Transaction activity
- Account performance
- Inactive accounts
- Financial irregularities
- Monthly transaction trends

---

# Business Problem

Banks generate large amounts of customer and transaction data daily. However, raw data alone is difficult to analyze without proper cleaning and visualization.

The objective of this project was to:
- analyze customer transaction behavior
- monitor account activity
- identify inactive accounts
- understand customer demographics
- detect unusual financial patterns

The dataset intentionally included:
- mixed date formats
- null values
- inconsistent text formatting
- invalid relationships
- outlier balances

to simulate real world banking data challenges.

---

# Tools & Technologies Used

- SQL Server
- Power BI Desktop
- Power Query
- DAX
- Notion
- XMind
- GitHub

---

# Dataset Overview

The project consists of three primary tables:

## Customers Table
Contains customer-related information:
- CustomerID
- Name
- Gender
- DateOfBirth
- Address
- Email
- Phone

---

## Accounts Table
Contains account-level details:
- AccountID
- CustomerID
- Account Type
- OpenDate
- Balance

---

## Transactions Table
Contains transaction-related records:
- TransactionID
- AccountID
- TransactionDate
- Transaction Type
- Amount
- Currency

More than 10,000 synthetic transaction records were generated for analysis.

---

# Data Generation & Dataset Design

Synthetic banking data was generated using SQL along with AI assisted prompt engineering through Perplexity.

Several intentional inconsistencies were introduced to simulate realistic operational data issues such as:
- mixed date formats
- null values
- inconsistent capitalization
- invalid foreign key relationships
- outlier balances
- duplicate possibilities
- inconsistent currency values

---

# SQL Data Cleaning

The dataset contained multiple inconsistent date formats across different tables.

To standardize the data:
- `TRY_CONVERT()` was used
- `CASE` statements handled multiple date patterns
- dates were converted into a consistent `MM/dd/yyyy` format

Additional cleaning steps included:
- handling inconsistent text values
- validating date conversions
- preserving invalid records for analysis
- preparing data for Power BI compatibility

---

# Combining Tables Using SQL Joins

The Customers, Accounts, and Transactions tables were combined using SQL joins to create a centralized analytical dataset.

`LEFT JOIN` operations were used intentionally to preserve:
- unmatched records
- incomplete relationships
- invalid account references

The final combined table:
```sql
CombinedBankingDataset
```

was later imported into Power BI for analysis and visualization.

---

# Power BI & Power Query Workflow

After connecting SQL Server to Power BI:
- Power Query Editor was used for additional cleaning
- null descriptions were replaced with `"Unknown"`
- inconsistent currency values were standardized
- account type capitalization was corrected
- data types were validated
- locale-based date conversion was applied to fix parsing issues

---

# Dashboard KPIs

The dashboard includes the following KPIs and visualizations:

- Transactions by Type
- Monthly Transaction Trends
- Total Balance by Account Type
- Total Balance by Name
- Inactive Accounts by Month
- Customer Gender Distribution
- Customers by Age Group
- Accounts by Account Type
- Transaction Volume Trend
- Customer Location Distribution

---

# Key Insights

- Credit and Debit transactions showed nearly equal distribution
- Monthly transaction activity fluctuated across the year
- Savings and Current accounts showed balanced distribution
- Multiple inactive accounts were identified
- Financial outliers and negative balances were detected
- Customer demographic trends were visualized successfully

---

# Dashboard Screenshots

## Main Dashboard

<img width="1905" height="1064" alt="Dashboard" src="YOUR_IMAGE_LINK_HERE">

---

# Challenges Faced

- Mixed date formats
- Locale conversion issues in Power BI
- Null value handling
- Invalid account relationships
- Data standardization inconsistencies

---

# Key Learnings

Through this project, I gained practical experience in:
- SQL data cleaning
- Power Query transformations
- DAX calculations
- Dashboard design
- Data visualization
- Business-oriented analytics workflows

---

# Future Improvements

- Real-time data integration
- Customer churn analysis
- Fraud detection KPIs
- Advanced forecasting
- Cloud-based dashboard deployment

---

# Project Structure

```bash
Banking-Analytics-Dashboard/
│
├── SQL Queries/
├── Power BI File/
├── Dataset/
├── PPT Presentation/
├── Mindmap/
└── README.md
```

---

# Author

Mayank Gupta
