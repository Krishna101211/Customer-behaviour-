---

# 🛍️ Customer Shopping Behavior Analysis

## 📌 Business Problem Statement

A leading retail company wants to better understand its customers’ shopping behavior to improve sales performance, customer satisfaction, and long-term loyalty.

The company observed shifts in:

* Purchasing patterns across demographics
* Product category demand
* Online vs. offline channel preferences
* Discount and subscription behavior

### 🎯 Core Business Question

> **How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?**

---

## 📊 Project Overview

This project analyzes **3,900 customer transactions** to uncover meaningful business insights using:

* **Python (Pandas, NumPy)** – Data Cleaning & EDA
* **PostgreSQL** – Business Querying & Segmentation
* **Power BI** – Interactive Dashboard & Visualization

The objective was to transform raw transactional data into actionable business recommendations.

---

## 🗂️ Dataset Summary

* **Total Records:** 3,900
* **Total Features:** 18
* **Missing Values:** 37 (Review Rating column)

### 🔑 Key Data Categories

**Customer Demographics**

* Age
* Gender
* Location
* Subscription Status

**Purchase Information**

* Item Purchased
* Category
* Purchase Amount (USD)
* Season
* Size & Color

**Shopping Behavior Indicators**

* Discount Applied
* Promo Code Used
* Review Rating
* Previous Purchases
* Frequency of Purchases
* Shipping Type
* Payment Method

---

## 🧹 Data Cleaning & Preparation (Python)

### ✔ Data Exploration

* Used `df.info()` and `df.describe()` for structure and summary statistics.
* Checked for duplicates and inconsistencies.

### ✔ Missing Value Treatment

* Imputed missing review ratings using **median rating per product category** to maintain fairness and reduce bias.

### ✔ Column Standardization

* Renamed columns to **snake_case** for readability and consistency.

### ✔ Feature Engineering

* Created **age_group** (Youth, Adult, Middle-Aged, Senior)
* Converted purchase frequency into numeric days
* Identified redundancy between `discount_applied` and `promo_code_used` → removed `promo_code_used`

### ✔ Database Integration

* Loaded cleaned dataset into PostgreSQL for structured business analysis.

---

## 🗄️ Business Analysis Using PostgreSQL

Performed analytical queries to answer business-driven questions:

### 📌 Revenue Insights

* Revenue comparison by gender
* Revenue contribution by age group
* Subscribers vs Non-subscribers spending patterns

### 📌 Customer Segmentation

Customers classified as:

* **New** (1–2 purchases)
* **Returning** (3–5 purchases)
* **Loyal** (>5 purchases)

Analyzed subscription likelihood among loyal customers.

### 📌 Product Performance

* Top 5 highest-rated products
* Top 3 most purchased products per category
* Discount-dependent products
* High-spending customers who still use discounts

### 📌 Shipping Behavior

* Compared Standard vs Express shipping spending trends

---

## 📈 Power BI Dashboard

An interactive dashboard was built to visualize:

* Total Revenue & KPIs
* Revenue by Gender & Age Group
* Subscription Impact on Sales
* Product Category Performance
* Shipping Type Analysis
* Discount Impact Analysis

### Dashboard Features

* Dynamic slicers (Season, Category, Gender, Subscription)
* KPI Cards
* Drill-through analysis
* Business-friendly layout for executive presentation

---

## 💡 Key Insights

1. **Subscribers generate higher repeat revenue.**
2. Loyal customers are more likely to opt for subscription.
3. Express shipping users show higher average purchase value.
4. Certain products are heavily discount-dependent.
5. Middle-aged and adult segments contribute significantly to revenue.

---

## 🚀 Business Recommendations

### ✅ Strengthen Subscription Programs

Offer exclusive deals and loyalty perks to convert repeat customers.

### ✅ Enhance Loyalty Programs

Reward high-frequency buyers to retain them in the “Loyal” segment.

### ✅ Optimize Discount Strategy

Reduce unnecessary discounting on already high-performing products.

### ✅ Targeted Marketing Campaigns

Focus on high-revenue age groups and express-shipping customers.

### ✅ Promote High-Rated Products

Highlight top-rated and best-selling products in digital campaigns.

---

## 🛠️ Tech Stack

* Python (Pandas, NumPy)
* PostgreSQL
* Power BI
* Jupyter Notebook

---

## 📌 Project Outcome

This project demonstrates:

* End-to-end data analysis workflow
* Strong SQL business querying
* Data cleaning & feature engineering
* Dashboard storytelling
* Converting insights into business strategy

---

## 👨‍💻 Author

**KRUSHNA SHINDE**
Data Analyst | Python | SQL | Power BI

---
