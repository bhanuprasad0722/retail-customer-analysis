# 🛒 Retail Customer Purchase Behavior Analysis

This project analyzes transaction and customer data from a retail environment to uncover insights into customer behavior, product preferences, and segment-based trends for snack purchases - specifically focused on chips.

## 📌 Objective

The primary goal of this project was to explore and analyze customer purchase behavior in the chips category by:

- Cleaning and preparing retail transaction and customer data
- Engineering new features for improved insights
- Segmenting customers by lifestyle and purchasing power
- Visualizing sales trends and segment behavior
- Extracting business insights to support retail strategy decisions

---

## 📁 Dataset Overview

Two main datasets were used:

1. `QVI_transaction_data.xlsx`  
   - Transaction-level data
   - Contains store number, transaction ID, date, product name, quantity, and total sales

2. `QVI_purchase_behaviour.csv`  
   - Customer-level data
   - Contains customer ID, lifestyle stage (e.g., "Young Singles/Couples"), and premium customer tier (e.g., "Budget", "Mainstream", "Premium")

---

## 🔧 Tools Used

- **Python**
- **Google Colab / Jupyter Notebook**
- **Pandas** – for data wrangling and feature engineering  
- **Matplotlib & Seaborn** – for data visualization  
- **Numpy** – for numerical operations

---

## 🔄 Steps Performed

### 1. 📥 Data Loading

Loaded both datasets using `pandas` and inspected their basic structure.

---

### 2. 🧹 Data Cleaning

- **Formatted `DATE` column** to correct datetime type
- **Checked for null values** in both datasets
- **Dropped** redundant columns after feature extraction

---

### 3. 🏷️ Feature Engineering

- Extracted `PACK_SIZE` from `PROD_NAME`
- Extracted `BRAND_NAME` from `PROD_NAME`
- Filtered transactions to only include products from the **"Chips"** category
- Merged customer data with transaction data on `LYLTY_CARD_NBR`

---

### 4. 🔍 Exploratory Data Analysis (EDA)

#### 📊 General Analysis

- Total sales, number of transactions, and number of customers
- Monthly sales trend over time

#### 📈 Brand Analysis

- Identified top-selling brands based on total revenue
- Compared popularity of brands across customer segments

#### 📦 Pack Size Preferences

- Analyzed which pack sizes were most frequently purchased
- Found that 175g was the most common size

#### 👥 Customer Segmentation

- Analyzed purchasing behavior by:
  - `LIFESTAGE` (e.g., "Young Singles/Couples", "Midage Singles/Couples")
  - `PREMIUM_CUSTOMER` tier (e.g., "Budget", "Mainstream", "Premium")

- Found that:
  - **"Mainstream Midage Couples"** and **"Premium Families"** contributed significantly to total sales
  - **Budget segments** still made frequent purchases but preferred smaller pack sizes or different brands

---

## 📌 Key Insights

- **175g** chip packets are the most popular across all customer types
- **A few premium brands** dominate the sales, indicating brand loyalty
- **Premium Families** and **Mainstream Midage Couples** spend the most on chips
- Lifestyle and spending behavior strongly influence purchase patterns — great insight for targeting

---

