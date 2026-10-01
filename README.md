# Customer Churn Analysis using SQL

## Overview

This project analyzes customer subscription data using MySQL to identify patterns associated with customer churn.

The analysis focuses on customer contract type, internet service, payment method, monthly charges, and customer tenure.

---

## Dataset

**Telco Customer Churn Dataset**

The dataset contains **7,043 customer records** and includes information such as:

- Customer demographics
- Tenure
- Contract type
- Internet service
- Payment method
- Monthly charges
- Churn status

**Dataset Source:** [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

## Tools Used

- MySQL
- SQL
- MySQL Workbench

---

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
- Conditional Aggregation

---

## Analysis Performed

### 1. Overall Churn

Calculated the total number of customers and the overall churn rate.

**Overall observed churn rate: 26.54%**

---

### 2. Churn by Contract

Compared churn rates across different contract types:

- Month-to-month
- One year
- Two year

**Key result:**

- Month-to-month: 42.71%
- One year: 11.27%
- Two year: 2.83%

---

### 3. Churn by Internet Service

Compared churn rates across:

- Fiber optic
- DSL
- No internet service

**Key result:**

- Fiber optic: 41.89%
- DSL: 18.96%
- No internet service: 7.40%

---

### 4. Churn by Payment Method

Compared churn rates across different payment methods.

**Key result:**

- Electronic check: 45.29%
- Mailed check: 19.11%
- Bank transfer (automatic): 16.71%
- Credit card (automatic): 15.24%

---

### 5. Monthly Charges

Compared average monthly charges between customers who churned and customers who stayed.

- Customers who stayed: **61.27**
- Customers who churned: **74.44**

---

### 6. Tenure Analysis

Created tenure groups using `CASE WHEN` and compared churn rates across different customer tenure ranges.

**Key result:**

- 0–12 months: 47.44%
- 13–24 months: 28.71%
- 25–48 months: 20.39%
- 49+ months: 9.51%

---

## Key Observations

- The overall observed churn rate was **26.54%**.
- Month-to-month customers had an observed churn rate of **42.71%**.
- Fiber-optic customers had an observed churn rate of **41.89%**.
- Electronic-check customers had an observed churn rate of **45.29%**.
- Customers who churned had higher average monthly charges than customers who stayed.
- The 0–12 month tenure group had an observed churn rate of **47.44%**, while the 49+ month group had a rate of **9.51%**.

> These observations describe associations in the dataset and do not establish causation.

---

## Project Structure

```text
customer-churn-sql-analysis/
│
├── churn_analysis.sql
└── README.md
```

## How to Run

1. Install MySQL and MySQL Workbench.
2. Create a database named `customer_churn`.
3. Create the `customers` table.
4. Load the Telco Customer Churn dataset into the table.
5. Open `churn_analysis.sql`.
6. Run the SQL queries in MySQL Workbench.

---

## Author

**Ishika Gupta**
