
# 🛍️ Customer Shopping Behavior Analysis

A comprehensive end-to-end data analysis project that uncovers insights into customer spending patterns, product preferences, customer segmentation, and subscription behavior using **Python**, **PostgreSQL**, and **Power BI**.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Summary](#dataset-summary)
- [Tech Stack](#tech-stack)
- [Project Workflow](#project-workflow)
- [Key Findings](#key-findings)
- [Dashboard](#dashboard)
- [Business Recommendations](#business-recommendations)

---

## 📌 Project Overview

This project analyzes **3,900 customer transactions** across various product categories. The goal is to derive actionable business insights by exploring:

- Customer spending patterns by demographics
- Product performance and ratings
- Subscription behavior and its impact on revenue
- Customer loyalty segmentation
- Discount dependency across product lines

---

## 📊 Dataset Summary

| Property | Details |
|----------|---------|
| **Total Rows** | 3,900 |
| **Total Columns** | 18 |
| **Missing Data** | 37 values in `Review Rating` column |
| **Age Range** | 18 – 70 |
| **Purchase Amount Range** | $20 – $100 |
| **Average Review Rating** | 3.75 |

### Features

- **Demographics** — Age, Gender, Location, Subscription Status
- **Purchase Details** — Item Purchased, Category, Purchase Amount, Season, Size, Color
- **Behavior** — Discount Applied, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) | Data cleaning & EDA |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) | Data manipulation |
| ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white) | SQL business analysis |
| ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black) | Interactive dashboard |

---

## 🔄 Project Workflow

### 1. 🐍 Exploratory Data Analysis (Python)

- **Data Loading** — Imported dataset using `pandas`
- **Initial Exploration** — Used `df.info()` and `.describe()` for structure and statistics
- **Missing Data Handling** — Imputed missing `Review Rating` values using the **median rating per product category**
- **Column Standardization** — Renamed all columns to `snake_case`
- **Feature Engineering**
  - Created `age_group` column by binning customer ages
  - Created `purchase_frequency_days` column from purchase data
- **Data Consistency Check** — Verified and dropped the redundant `promo_code_used` column
- **Database Integration** — Loaded cleaned DataFrame into **PostgreSQL** for SQL analysis

---

### 2. 🗄️ SQL Business Analysis (PostgreSQL)

Ten structured queries were run to answer key business questions:

| # | Analysis | Insight |
|---|---------|---------|
| 1 | **Revenue by Gender** | Male: $157,890 / Female: $75,191 |
| 2 | **High-Spending Discount Users** | 839 customers used discounts but spent above average |
| 3 | **Top 5 Products by Rating** | Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78) |
| 4 | **Shipping Type Comparison** | Express avg: $60.48 / Standard avg: $58.46 |
| 5 | **Subscribers vs. Non-Subscribers** | Similar avg spend (~$59); Non-subscribers contribute more total revenue |
| 6 | **Discount-Dependent Products** | Hat (50%), Sneakers (49.66%), Coat (49.07%), Sweater (48.17%), Pants (47.37%) |
| 7 | **Customer Segmentation** | Loyal: 3,116 / Returning: 701 / New: 83 |
| 8 | **Top 3 Products per Category** | Jewelry, Blouse, Sandals, Jacket lead their categories |
| 9 | **Repeat Buyers & Subscriptions** | 2,518 repeat buyers are non-subscribers vs. 958 subscribers |
| 10 | **Revenue by Age Group** | Young Adults lead at $62,143, followed by Middle-aged at $59,197 |

---

### 3. 📊 Power BI Dashboard

An interactive dashboard was built to visualize all key metrics with filters for Subscription Status, Gender, Category, and Shipping Type.

**Dashboard KPIs:**
- 🧑‍🤝‍🧑 **3.9K** Total Customers
- 💰 **$59.76** Average Purchase Amount
- ⭐ **3.75** Average Review Rating

---

## 📈 Key Findings

- **Clothing** is the top revenue-generating category
- **Young Adults** contribute the highest revenue across all age groups
- **73%** of customers are non-subscribers, representing a major growth opportunity
- **80%** of customers are classified as "Loyal" based on purchase history
- Products like **Hat and Sneakers** have high discount dependency (~50%)
- Express shipping users spend slightly more than standard shipping users

---

## 💡 Business Recommendations

| Recommendation | Action |
|---------------|--------|
| 🔔 **Boost Subscriptions** | Promote exclusive perks and benefits for subscribers |
| 🏆 **Customer Loyalty Programs** | Reward repeat buyers to retain and grow the Loyal segment |
| 💸 **Review Discount Policy** | Balance promotional discounts with profit margin control |
| 🌟 **Product Positioning** | Highlight top-rated products (Gloves, Sandals) in marketing campaigns |
| 🎯 **Targeted Marketing** | Focus campaigns on Young Adults and Express-shipping users |

---

#youtube video link of this above project 
https://youtu.be/P6Zp_y8Rdug

