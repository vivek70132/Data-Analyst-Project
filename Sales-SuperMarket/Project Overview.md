# 📊 Sales Analysis Dashboard (Power BI)

![Power BI](https://img.shields.io/badge/Tool-PowerBI-yellow)
![Data](https://img.shields.io/badge/Data-Excel-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)
![Level](https://img.shields.io/badge/Level-Intermediate-orange)

---

## 🧭 Overview

This project presents a **multi-page Sales Analysis Dashboard** built using Power BI to analyze business performance across:

- Revenue & Profitability  
- Product Performance  
- Discount Impact  
- Customer Segmentation  
- Geographic Trends  

The solution is designed with a **Dashboard (Executive Summary)** and **Report Pages (Deep Analysis)** approach.

---

## 🎯 Objectives

- Track overall **sales performance**
- Identify **profit drivers and loss-making products**
- Analyze **impact of discounts on profit**
- Understand **customer segments and regions**
- Build an **interactive, business-driven dashboard**

---

## 📂 Dataset

- Source: Excel  
- Data includes:
  - Orders (Date, ID)
  - Customer (Name, Segment)
  - Geography (Region, State, City)
  - Product (Category, Sub-Category)
  - Metrics: Sales, Profit, Quantity, Discount

---

## 📊 Dashboard Structure

### 🔷 1. Executive Dashboard
- KPI Cards (Sales, Profit, Orders, Margin)
- Sales Trend
- Sales by Category
- Sales by Region

---

### 🔷 2. Product Analysis
- Profit by Sub-Category
- Top 10 Products
- Loss-making products

---

### 🔷 3. Discount Analysis
- Scatter Plot: Discount vs Profit
- Avg Discount by Category
- Profit by Discount Band

---

### 🔷 4. Customer Analysis
- Sales by Segment
- Top Customers
- Order Distribution

---

### 🔷 5. Geography Analysis
- Sales by Region
- Profit by Region
- Map (Sales by City)

---

## 📸 Screenshots

### 🏠 Dashboard Overview
![Dashboard](images/dashboard.png)

### 📦 Product Analysis
![Product](images/product.png)

### 📉 Discount Analysis
![Discount](images/discount.png)

### 👥 Customer Analysis
![Customer](images/customer.png)

### 🌍 Geography Analysis
![Geography](images/geography.png)

---

## 🧠 Key Insights

- 📉 **High discounts (>40%) reduce profitability**
- 📦 Some products generate **sales but negative profit**
- 💡 Sales ≠ Profit (critical business insight)
- 🌍 Regional performance varies significantly
- 👥 Consumer segment drives highest revenue

---

## 🛠️ DAX Measures

```DAX
Total Sales = SUM('Sales Overview Data xlsx - Sales Data'[Sales])
Total Profit = SUM('Sales Overview Data xlsx - Sales Data'[Profit])
Total Orders = DISTINCTCOUNT('Sales Overview Data xlsx - Sales Data'[Order ID])
Profit Margin = DIVIDE([Total Profit], [Total Sales])
