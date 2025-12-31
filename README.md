# Customer-Behavior-Analysis

## 📌 **Overview**

This project analyzes **customer shopping behavior for a retail business** using **Python, SQL (specifically PostgreSQL), and Power BI.**
The **goal** is to understand **how customer demographics, discounts, subscriptions, and product categories** influence **purchasing decisions and long-term loyalty**.

The project follows an **end-to-end analytics workflow — from raw data cleaning and exploratory analysis in Python to business insights via SQL queries and an interactive Power BI dashboard**.

## 📂 **Dataset**

-> Records: 3,900 purchase transactions

-> Features: 18 columns

-> Product Categories: Clothing, Accessories, Footwear, Outerwear

## **Key Attributes:**

-> Customer demographics: age, gender, location

-> Purchase details: item, category, amount, season

-> Behavioral data: discounts, review ratings, purchase frequency

-> Subscription and shipping preferences

## **Data Issues Addressed**

-> 37 missing values in the _review_rating_ column

-> Redundant promotional fields

-> Inconsistent column naming

## **Tools & Technologies**

-> Python: pandas, numpy, matplotlib, seaborn

-> Database: PostgreSQL

-> Visualization: Power BI

-> Presentation: Gamma

-> Environment: Jupyter Notebook

## 🔄 Project Workflow
### 1️⃣ Data Cleaning & EDA (Python – Jupyter Notebook)

-> Loaded dataset using pandas and performed initial inspection (info(), describe()).

-> Identified missing values and data inconsistencies.

-> Imputed missing **review_rating** values using median rating per product category.

-> Standardized column names to **snake_case.**

-> Verified data consistency between discount_applied and promo_code_used.

-> Removed redundant columns to simplify analysis.

### 2️⃣ Feature Engineering

-> Created age_group feature by binning customer ages.

-> Derived purchase frequency indicators from previous purchase data.

-> Prepared cleaned and structured data for database loading.

### 3️⃣ Database Integration (PostgreSQL)

-> Connected Python to PostgreSQL.

-> Loaded the cleaned DataFrame into relational tables for SQL analysis.

### 4️⃣ Business Analysis (SQL)

-> Executed SQL queries to answer key business questions:

-> Revenue contribution by gender

-> Spending behavior of discount users

-> Product performance based on customer ratings

-> Subscriber vs non-subscriber comparison

-> Shipping type impact on purchase value

-> Customer segmentation (New, Returning, Loyal)

-> Revenue contribution by age group

### 5️⃣ Data Visualization (Power BI)

-> Built an interactive dashboard with KPIs and filters.

-> Visualized revenue distribution, customer segments, subscriptions, and product performance.

### 6️⃣ Reporting & Presentation

-> Created a detailed analytical report summarizing findings.

-> Designed a stakeholder-ready presentation using Gamma.

## 📊 Power BI Dashboard Highlights

### Key KPIs

-> **Total Customers:** 3.9K

-> **Average Purchase Amount**: $59.76

-> **Average Review Rating**: 3.75

-> **Subscription Split**: 27% Subscribers | 73% Non-Subscribers

### Revenue & Sales Visuals

-> Revenue distribution by product category (Clothing, Accessories, Footwear, Outerwear)

-> Sales and revenue comparison across age groups

-> Category-wise sales contribution for performance tracking

### Customer Segmentation View

-> Visual breakdown of customers into New, Returning, and Loyal

-> Highlights dominance of loyal customers and retention strength

### Subscription Analysis

-> Comparison of spending patterns between subscribers and non-subscribers

-> Helps assess subscription impact on revenue and customer value

### Product Performance

-> Displays top-rated products based on average review ratings

-> Supports data-driven product promotion decisions

### Interactive Filtering

**Filters for:**

-> Gender

-> Product Category

-> Subscription Status

-> Shipping Type

-> **Enables stakeholders to explore insights dynamically**

## 🔍 Key Insights

### Revenue by Gender

-> Male customers generate approximately **2× higher total revenue** than female customers, indicating stronger purchase volume or higher-value transactions.

### Customer Loyalty

-> Around **80% of customers are classified as Loyal**, showing strong retention and repeat purchasing behavior.

-> A smaller segment of **Returning customers** presents an opportunity for targeted loyalty programs.

### Discount Behavior

-> Over **800 customers** used discounts while still spending **above the average purchase amount.**

-> Discounts attract value-conscious customers without necessarily lowering revenue.

### Product Performance

-> Products such as **Gloves, Sandals, and Boots** consistently receive the **highest average ratings**.

-> High-rated products should be prioritized in marketing and promotions.

### Subscription Opportunity

-> Only **27% of customers are subscribers**, indicating significant scope to improve subscription adoption.

-> Subscribers and repeat buyers show potential for higher long-term value.

### Age Group Contribution

-> **Young adults and middle-aged customers** contribute the **highest share of revenue**.

-> Revenue distribution across age groups remains balanced, suggesting broad market appeal.
