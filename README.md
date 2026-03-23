# 📊 Sales & Customer Performance Dashboard (Power BI)

## 📌 Project Overview

This project showcases an interactive **Sales & Customer Performance Dashboard** built using Power BI.
It provides insights into sales trends, customer behavior, and product performance for better business decision-making.

---

## 🎯 Objectives

* Analyze sales and profit performance
* Identify top customers and products
* Track monthly and yearly trends
* Enable interactive filtering
* Apply Row-Level Security (RLS)

---

## 📂 Dataset Used

* **FinalProject_Dataset.xlsx**
* Includes Sales, Customer, Product, and Region data

---

## 🏗️ Data Model

* Star Schema Design
* Fact Table: `Sales_Fact`
* Dimension Tables:

  * `Customer_Dim`
  * `Product_Dim`
  * `Region_Dim`
  * Date Table

---

## 📊 Dashboard Screenshots

### 🟦 Overview Page

![Overview](overview.png)

✔ KPI Cards (Sales, Customers, Orders)
✔ Top Products by Sales
✔ Sales Trend (Monthly)
✔ Category Distribution
✔ Region & Date Filters

---

### 🟩 Customer Analysis Page

![Customer Analysis](customer_analysis.png)

✔ Total Profit & Customers
✔ Top Customers by Profit
✔ Yearly Sales Comparison
✔ Customer-wise Matrix Analysis

---

### 🟨 Product Analysis Page

![Product Analysis](product_analysis.png)

✔ Total Sales, Products, Units Sold
✔ Top Products Performance
✔ Profit Margin Category Analysis
✔ Monthly Sales Trend

---

### 🟥 Drillthrough Page

![Drillthrough](drillthrough.png)

✔ Customer/Product level detailed view
✔ Orders table with metrics
✔ Dynamic filtering via drillthrough

---

## 📱 Mobile Layout

✔ Optimized layout for mobile viewing
✔ KPI-first design approach

---

## 🧠 DAX Measures

```DAX id="dax992"
Total Sales = SUM(Sales_Fact[TotalAmount])
Total Profit = SUM(Sales_Fact[TotalAmount]) * 0.2
Total Orders = COUNT(Sales_Fact[SaleID])
Total Customers = DISTINCTCOUNT(Sales_Fact[CustomerID])
Total Units Sold = SUM(Sales_Fact[UnitsSold])
```

---

## 🚀 Features

* Interactive Slicers (Region, Date, Category)
* Drill Down / Drill Up
* Drillthrough Navigation
* Conditional Formatting
* Custom Navigation Buttons
* Row-Level Security (RLS)

---

## 📁 Project Files

* Power BI Report (.pbix)
* Dataset (.xlsx)
* Dashboard Screenshots

---

## 🏁 Conclusion

This project demonstrates strong Power BI skills including data modeling, DAX calculations, and dashboard design to solve real-world business problems.

---

If you found this useful, give it a ⭐ on GitHub!

