# 🛒 Retail Sales Analysis (SQL Project)

## 📌 Overview
This project performs end-to-end SQL analysis on a retail dataset containing customer, product, and sales information.  
It includes **data cleaning**, **validation**, and **exploratory data analysis (EDA)** to produce meaningful business insights.

The goal of this project is to replicate real-world SQL tasks performed by data analysts.

---

## 🧹 Data Cleaning & Preprocessing

### ✔️ Fixed Column Name Issues
- Resolved encoding problems and renamed incorrectly formatted columns.
- Improved dataset consistency by standardizing column names.

### ✔️ Removed Duplicate Records
- Identified duplicate `TransactionID` and removed extra entries safely.
- Ensured each transaction is unique and valid.

### ✔️ Handled Missing & Invalid Values
- Checked for NULL or blank fields in all three tables.
- Corrected missing `Location` values by replacing with `"NA"`.
- Removed invalid records such as unrealistic ages.



### ✔️ Corrected Price Mismatch
- Compared product price in `sales_transaction` vs `product_inventory`.
- Updated incorrect prices to ensure consistent and accurate calculations.

### ✔️ Validated Business Rules
- Ensured stock levels were non-negative.
- Checked for invalid or zero product prices.
- Identified and removed impossible future JoinDates.

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 1. Product Performance
- Identified top-selling products based on total quantity sold.
- Calculated revenue per product to determine high-performing items.

### 🔹 2. Category-Level Insights
- Rank-ordered categories by:
- Total quantity sold  
- Total revenue  
- Identified which categories drive the most business value.

### 🔹 3. Customer Purchase Frequency
- Counted total number of transactions per customer.
- Created meaningful customer segments:
- **Low Buyers**
- **Medium Buyers**
- **High Buyers**

### 🔹 4. Monthly Sales Trend
- Evaluated month-by-month sales to find:
- Peak selling months  
- Seasonal demand patterns  

### 🔹 5. High-Value Customers
- Identified top 5 customers by total spend.
- Useful for loyalty programs or targeted marketing.

### 🔹 6. Customer Loyalty Tracking
- Calculated days between first and last purchase.
- Highlighted long-term and consistent customers.

### 🔹 7. Product Preference by Customer
- Analyzed which products customers repeatedly purchase.
- Useful for personalization and recommendations.

---

## ❓ Business Questions Answered

| Business Question | Output |
|-------------------|--------|
| Which products sell the most? | Ranking by quantity & revenue |
| Which category performs best? | Top category by sales & demand |
| How often does each customer purchase? | Customer segmentation report |
| When do sales peak? | Month-wise trend analysis |
| Who are the highest spending customers? | Top 5 spenders list |
| Are product prices consistent across tables? | Identified & corrected mismatches |
| How loyal are customers? | Duration analysis between purchases |

---

## 🧠 SQL Skills Demonstrated
This project uses a wide range of SQL concepts:

- **Data Cleaning**
- **String manipulation**
- **Joins & aggregations**
- **GROUP BY + HAVING**
- **Window logic (conceptually)**
- **Conditional statements (CASE)**
- **Date functions**
- **Data validation techniques**
- **Business logic application**
- **Insight extraction using SQL queries**

-------------------------------------------------------------




### ✔️ Standardized Date Formats
- Converted date strings into proper MySQL DATE format using:
