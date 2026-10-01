# Customer Churn Analysis using SQL

## Overview

This project analyzes customer subscription data using MySQL to identify patterns associated with customer churn.

The analysis focuses on customer contract type, internet service, payment method, monthly charges, and tenure.

## Dataset

Telco Customer Churn dataset.

The dataset contains 7,043 customer records and includes information such as:

- Customer demographics
- Tenure
- Contract type
- Internet service
- Payment method
- Monthly charges
- Churn status

Dataset source:
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

## Tools Used

- MySQL
- SQL
- MySQL Workbench

## SQL Concepts Used

- SELECT
- WHERE
- GROUP BY
- ORDER BY
- COUNT()
- SUM()
- AVG()
- ROUND()
- CASE WHEN
- Conditional aggregation

## Analysis Performed

### 1. Overall Churn

Calculated the total number of customers and overall churn rate.

Overall churn rate: 26.54%

### 2. Churn by Contract

Compared churn rates across:

- Month-to-month
- One year
- Two year

### 3. Churn by Internet Service

Compared churn rates across:

- Fiber optic
- DSL
- No internet service

### 4. Churn by Payment Method

Compared churn rates across different payment methods.

### 5. Monthly Charges

Compared average monthly charges between customers who churned and those who stayed.

### 6. Tenure Analysis

Created tenure groups to compare churn rates among customers with different lengths of service.

## Key Observations

- Overall observed churn rate was 26.54%.
- Month-to-month customers had an observed churn rate of 42.71%.
- Fiber-optic customers had an observed churn rate of 41.89%.
- Electronic-check customers had an observed churn rate of 45.29%.
- Customers who churned had higher average monthly charges than customers who stayed.
- The 0–12 month tenure group had an observed churn rate of 47.44%, while the 49+ month group had a rate of 9.51%.

These observations describe associations in the dataset and do not establish causation.

## Project Structure

customer-churn-sql/
│
├── churn_analysis.sql
└── README.md
