# Banking & Credit Risk Analytics

## Overview

Banking & Credit Risk Analytics is an interactive Power BI project developed to analyze loan portfolios, borrower characteristics, and credit default risk.

The project uses a real-world public credit-risk dataset containing more than 32,000 loan records. The dashboard provides a business-focused view of loan exposure, customer defaults, loan characteristics, and borrower risk patterns.

## Business Objective

The objective of this project is to help banking and lending teams understand credit-risk patterns and identify borrower segments that may require closer risk assessment.

The analysis focuses on:

- Loan portfolio size and exposure
- Customer and default volumes
- Default rates
- Loan-grade risk
- Loan-purpose risk
- Interest-rate patterns
- Historical default behavior
- Borrower income and age
- Employment length
- Home ownership
- Credit history length

## Dataset

The project uses a public credit-risk dataset containing approximately 32,000+ loan records.

### Key Features

- Person age
- Person income
- Home ownership
- Employment length
- Loan intent
- Loan grade
- Loan amount
- Interest rate
- Loan percent income
- Historical default indicator
- Credit history length
- Current loan status

### Loan Status

`loan_status` is used as the current default indicator:

- `0` = No Default
- `1` = Default

## Tools & Technologies

- Power BI
- Power Query
- DAX
- CSV
- Git
- GitHub

## Data Preparation

Power Query was used to prepare the dataset for analysis.

The data preparation process included:

- Replacing the initial learning dataset with the real public dataset
- Promoting column headers
- Setting appropriate data types
- Creating a unique row-based customer identifier
- Preparing the dataset for Power BI analysis

## Dashboard

The dashboard provides an interactive overview of the credit-risk portfolio.

### Key Areas

- Portfolio KPIs
- Default analysis
- Loan-grade analysis
- Loan-purpose analysis
- Home-ownership analysis
- Historical-default analysis
- Interest-rate analysis
- Loan-amount analysis
- Borrower demographic analysis
- Employment and credit-history analysis

## Key Metrics

The dashboard includes the following measures:

- Total Loan Amount
- Total Customers
- Default Rate
- Defaulted Customers
- Average Loan Amount
- Average Interest Rate
- Defaulted Loan Amount
- Default Exposure Rate
- Loan to Income Ratio

## Risk Analysis

The dashboard analyzes important credit-risk questions such as:

- Which loan grades have higher default rates?
- Which loan purposes show higher default risk?
- How does historical default relate to current default?
- How does interest rate vary with default outcomes?
- How does loan amount relate to default behavior?
- How do borrower characteristics relate to default patterns?

## Business Insights

The analysis provides several business-oriented insights:

- Loan-grade analysis helps lenders identify segments that may require stronger credit assessment and monitoring.
- Loan-purpose analysis helps compare default behavior across different lending categories.
- Historical default behavior can be used as an important indicator when evaluating current credit risk.
- Interest-rate analysis helps examine differences in borrowing costs across default outcomes.
- Comparing loan amounts with borrower income helps assess potential repayment pressure.
- Home-ownership, employment, age, and credit-history characteristics provide additional dimensions for borrower risk segmentation.
- Default exposure analysis helps lenders understand not only how many customers defaulted, but also how much loan value is associated with those defaults.

## DAX Measures

The project uses DAX measures to calculate important portfolio and risk metrics.

Example:

```DAX
Total Loan Amount =
SUM(credit_risk[loan_amount])