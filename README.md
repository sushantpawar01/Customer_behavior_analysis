
## 📌 Project Overview
This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across various products categories.
The goal is to uncover the insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.

## 📂 Dataset Summary
* **Dimensions:** 3,900 Rows, 18 Columns
* **Key Features:** * **Customer Demographics:** Age, Gender, Location, Subscription Status 
* **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color 
* **Behavior:** Discount Applied, Promo Code Used, Previous Purchases, Frequency, Review Rating, Shipping Type
* **Data Quality:** Identified 37 missing values in the `Review Rating` column.

## 🛠 Tech Stack
* **Python (Pandas):** Data cleaning, imputation, and feature engineering.
* **PostgreSQL:** Structured data analysis and business transaction queries.
* **Power BI:** Interactive dashboard for data visualization.

## ⚙️ Methodology

### 1. Data Cleaning & Feature Engineering (Python)
* **Imputation:** Missing `Review Rating` values were filled using the median rating of each product category.
* **Standardization:** Columns were renamed to snake_case for better readability].
* **Feature Engineering:** * Created `age_group` column by binning customer ages.
    * Created `purchase_frequency_days` column.
* **Optimization:** Verified redundancy and dropped `promo_code_used`.

### 2. Exploratory Data Analysis (SQL)
Structured SQL queries were executed to answer key business questions. 
Key findings included:

* **Revenue by Gender:** Male customers generated significantly higher revenue ($157,890) compared to Female customers ($75,191).
* **Shipping Analysis:** The average spend for "Express" shipping ($60.48) is slightly higher than "Standard" shipping ($58.46).
* **Subscription Insights:**
    * **Subscribers:** 1,053 customers | Avg Spend: $59.49 | [cite_start]Total Revenue: $62,645.
    * **Non-Subscribers:** 2,847 customers | Avg Spend: $59.87 | [cite_start]Total Revenue: $170,436[cite: 49].
    * Repeat buyers (>5 purchases) are significantly less likely to be subscribers (958 Yes vs 2,518 No).
* **Top Products:** The highest-rated items include Gloves (3.86), Sandals (3.84), and Boots (3.82).
* **Customer Segmentation:** The majority of the customer base falls into the "Loyal" segment (3,116 customers) compared to "Returning" (701) and "New" (83).

### 3. Visualization (Power BI)
An interactive dashboard was created to visualize the findings:
* **Total Customers:** 3.9K 
* **Avg Purchase Amount:** $59.76 
* **Avg Review Rating:** 3.75 
* **Revenue by Age Group:** Young Adults contribute the highest revenue ($62,143), followed by Middle-aged ($59,197) and Adults ($55,978).

## 🚀 Business Recommendations
Based on the analysis, the following strategies are recommended:
1.  **Boost Subscriptions:** Promote exclusive benefits for subscribers to increase the conversion rate (currently only 27%).
2.  **Customer Loyalty Programs:** Implement rewards for repeat buyers to maintain the high volume of customers in the "Loyal" segment.
3.  **Review Discount Policy:** Strategies should balance sales boosts with margin control, particularly for high-discount items.
4.  **Targeted Marketing:** Focus marketing efforts on high-revenue segments like **Young Adults** and customers utilizing **Express Shipping**.
5.  **Product Positioning:** Highlight top-rated products (Gloves, Sandals) in marketing campaigns to build trust.

