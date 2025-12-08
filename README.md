# [cite_start]Customer Shopping Behavior Analysis [cite: 1]

## 📌 Project Overview
[cite_start]This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across various product categories[cite: 3]. [cite_start]The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions[cite: 4].

## 📂 Dataset Summary
* [cite_start]**Dimensions:** 3,900 Rows, 18 Columns [cite: 6, 7]
* [cite_start]**Key Features:** * **Customer Demographics:** Age, Gender, Location, Subscription Status [cite: 9]
    * [cite_start]**Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color [cite: 10]
    * [cite_start]**Behavior:** Discount Applied, Promo Code Used, Previous Purchases, Frequency, Review Rating, Shipping Type [cite: 11]
* [cite_start]**Data Quality:** Identified 37 missing values in the `Review Rating` column[cite: 12].

## 🛠 Tech Stack
* [cite_start]**Python (Pandas):** Data cleaning, imputation, and feature engineering[cite: 15, 19].
* [cite_start]**PostgreSQL:** Structured data analysis and business transaction queries[cite: 25, 27].
* [cite_start]**Power BI:** Interactive dashboard for data visualization[cite: 62].

## ⚙️ Methodology

### 1. Data Cleaning & Feature Engineering (Python)
* [cite_start]**Imputation:** Missing `Review Rating` values were filled using the median rating of each product category[cite: 19].
* [cite_start]**Standardization:** Columns were renamed to snake_case for better readability[cite: 20].
* [cite_start]**Feature Engineering:** * Created `age_group` column by binning customer ages[cite: 22].
    * [cite_start]Created `purchase_frequency_days` column[cite: 23].
* [cite_start]**Optimization:** Verified redundancy and dropped `promo_code_used`[cite: 24].

### 2. Exploratory Data Analysis (SQL)
[cite_start]Structured SQL queries were executed to answer key business questions[cite: 27]. Key findings included:

* [cite_start]**Revenue by Gender:** Male customers generated significantly higher revenue ($157,890) compared to Female customers ($75,191)[cite: 34, 37].
* [cite_start]**Shipping Analysis:** The average spend for "Express" shipping ($60.48) is slightly higher than "Standard" shipping ($58.46)[cite: 46].
* **Subscription Insights:**
    * **Subscribers:** 1,053 customers | Avg Spend: $59.49 | [cite_start]Total Revenue: $62,645[cite: 49].
    * **Non-Subscribers:** 2,847 customers | Avg Spend: $59.87 | [cite_start]Total Revenue: $170,436[cite: 49].
    * [cite_start]Repeat buyers (>5 purchases) are significantly less likely to be subscribers (958 Yes vs 2,518 No)[cite: 59].
* [cite_start]**Top Products:** The highest-rated items include Gloves (3.86), Sandals (3.84), and Boots (3.82)[cite: 43].
* [cite_start]**Customer Segmentation:** The majority of the customer base falls into the "Loyal" segment (3,116 customers) compared to "Returning" (701) and "New" (83)[cite: 54].

### 3. Visualization (Power BI)
[cite_start]An interactive dashboard was created to visualize the findings[cite: 63]:
* [cite_start]**Total Customers:** 3.9K [cite: 68]
* [cite_start]**Avg Purchase Amount:** $59.76 [cite: 70]
* [cite_start]**Avg Review Rating:** 3.75 [cite: 72]
* [cite_start]**Revenue by Age Group:** Young Adults contribute the highest revenue ($62,143), followed by Middle-aged ($59,197) and Adults ($55,978)[cite: 61].

## 🚀 Business Recommendations
Based on the analysis, the following strategies are recommended:
1.  [cite_start]**Boost Subscriptions:** Promote exclusive benefits for subscribers to increase the conversion rate (currently only 27%)[cite: 80, 99].
2.  [cite_start]**Customer Loyalty Programs:** Implement rewards for repeat buyers to maintain the high volume of customers in the "Loyal" segment[cite: 102].
3.  [cite_start]**Review Discount Policy:** Strategies should balance sales boosts with margin control, particularly for high-discount items[cite: 103].
4.  [cite_start]**Targeted Marketing:** Focus marketing efforts on high-revenue segments like **Young Adults** and customers utilizing **Express Shipping**[cite: 105].
5.  [cite_start]**Product Positioning:** Highlight top-rated products (Gloves, Sandals) in marketing campaigns to build trust[cite: 104].

