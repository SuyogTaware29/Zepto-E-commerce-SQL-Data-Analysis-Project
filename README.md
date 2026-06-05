# 🛒 Zepto E-commerce SQL Data Analysis Project

## 📌 Project Overview

This project focuses on analyzing Zepto’s e-commerce inventory dataset using SQL and PostgreSQL to uncover meaningful business insights related to pricing, discounts, inventory management, and product availability.

The project simulates real-world data analyst workflows including:

* Data exploration
* Data cleaning
* Business analysis
* Inventory analysis
* Revenue estimation

The objective is to help businesses optimize:

* Inventory management
* Pricing strategy
* Product availability
* Discount planning
* Revenue generation

---

# 🎯 Business Problem

Quick-commerce companies like Zepto manage thousands of products with dynamic pricing, inventory updates, and discount strategies.

The business wants to answer key questions such as:

* Which product categories generate the highest potential revenue?
* Which products are over-discounted?
* Which high-value products are frequently out of stock?
* How can inventory and pricing strategies be optimized?

---

# 📂 Dataset Information

The dataset contains product-level inventory data scraped from Zepto’s platform.

### Dataset Features

* SKU ID
* Product Name
* Category
* MRP
* Discount Percentage
* Discounted Selling Price
* Available Quantity
* Weight in Grams
* Stock Availability
* Package Quantity

Each row represents a unique product SKU.

---

# 🛠️ Technologies Used

## Database & Querying

* PostgreSQL
* SQL
* pgAdmin

## Version Control

* Git & GitHub

---

# 🔄 Project Workflow

## 1️⃣ Database & Table Creation

Created a structured PostgreSQL database and imported raw CSV inventory data.

### SQL Table Example

```sql id="lytmhh"
CREATE TABLE zepto (
  sku_id SERIAL PRIMARY KEY,
  category VARCHAR(120),
  name VARCHAR(150) NOT NULL,
  mrp NUMERIC(8,2),
  discountPercent NUMERIC(5,2),
  availableQuantity INTEGER,
  discountedSellingPrice NUMERIC(8,2),
  weightInGms INTEGER,
  outOfStock BOOLEAN,
  quantity INTEGER
);
```

---

## 2️⃣ Data Exploration

Performed exploratory analysis to:

* Understand dataset structure
* Identify missing values
* Explore product categories
* Compare stock availability
* Detect duplicate product listings

---

## 3️⃣ Data Cleaning

Data preprocessing steps included:

* Removing invalid pricing entries
* Handling null values
* Converting paise into rupees
* Standardizing numerical fields

---

## 4️⃣ Business Analysis using SQL

Performed SQL queries to answer business-driven questions.

### Key Analysis Performed

* Top discounted products
* High-MRP out-of-stock products
* Revenue estimation by category
* Products with low discounts but high prices
* Category-wise average discounts
* Price-per-gram analysis
* Inventory weight analysis
* Product segmentation by weight

---

# 🔍 Key Insights

* Certain categories contribute significantly higher revenue.
* Some premium products frequently remain out of stock.
* High discount percentages do not always guarantee better value.
* Snacks and beverages dominate inventory counts.
* Several products have inconsistent pricing strategies.

---

# 💡 Business Recommendations

* Improve restocking strategies for premium products.
* Optimize discount policies to maintain profitability.
* Focus inventory on high-performing categories.
* Monitor low-margin products with excessive discounts.
* Use category-wise pricing optimization for better revenue growth.

---

# 📁 Project Structure

```bash id="d0lu6j"
Zepto-Ecommerce-SQL-Analysis/
│
├── data/
│   └── zepto_v2.csv
│
├── sql/
│   └── zepto_SQL_data_analysis.sql
│
├── README.md
└── requirements.txt
```

---

# 🚀 How to Run the Project

## 1️⃣ Clone Repository

```bash id="vvh53i"
git clone https://github.com/your-username/Zepto-Ecommerce-SQL-Analysis.git
```

---

## 2️⃣ Create PostgreSQL Database

Create a new PostgreSQL database using pgAdmin.

---

## 3️⃣ Run SQL Script

Execute:

```bash id="70m8x4"
zepto_SQL_data_analysis.sql
```

This script includes:

* Table creation
* Data cleaning
* Data exploration
* Business analysis queries

---

## 4️⃣ Import Dataset

Import the CSV dataset into PostgreSQL using pgAdmin or the COPY command.

---

# 📈 Future Improvements

* Add Power BI dashboard
* Build Streamlit dashboard
* Add predictive analytics
* Automate ETL pipeline
* Create inventory forecasting model

---

# 👨‍💻 Author

## Suyog Taware

Aspiring Data Analyst

### Skills

* SQL
* PostgreSQL
* Python
* Data Analytics
* Business Analysis

GitHub:
https://github.com/SuyogTaware29
