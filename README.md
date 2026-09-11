# Miniso India Retail Sales Analytics Dashboard (2025)

An end-to-end Business Intelligence project developed in **Microsoft Power BI Desktop** analyzing retail transaction trends, product category velocity, and store-level revenue distributions across major metropolitan hubs in India for calendar year 2025.

---

## 📊 Dashboard Preview

![Dashboard Overview](dashboard_preview.png)

> *Tip: Ensure you upload your screenshot named `dashboard_preview.png` to the repository so it displays here.*

---

## 🎯 Business Context & Objectives

Fast-moving lifestyle retailers require clear visibility into product mix performance, regional sales disparities, and seasonal purchasing behaviors.

This project delivers actionable insights by:
- Monitoring high-level retail KPIs: **Total Revenue**, **Units Sold**, and **Average Order Value (AOV)**.
- Evaluating performance across key product divisions (Plush & IP, Health & Beauty, Homeware & Lifestyle, Digital & Tech, Stationery, Fashion Accessories).
- Identifying top revenue-generating markets across India (Delhi NCR, Mumbai, Kolkata, Bengaluru, Ahmedabad, and Guwahati).
- Analyzing monthly seasonality and sales momentum throughout FY2025.

---

## 🛠️ Tech Stack & Skills

- **Platform:** Microsoft Power BI Desktop
- **Data Modeling:** Analytical schema with clean dimensional typing
- **Calculations:** DAX (Data Analysis Expressions) for dynamic aggregation
- **ETL & Data Prep:** Power Query for data cleansing, date formatting, and type casting
- **Source Data:** Transaction-level retail sales logs (CSV)

---

## 📈 Key Metrics & DAX Measures

```dax
// Total Gross Revenue
Total Sales = SUM('Sales'[Amount])

// Total Physical Units Sold
Total Units Sold = SUM('Sales'[Number of Units Sold])

// Average Transaction Value
Average Basket Size = AVERAGE('Sales'[Amount])

// Average Price Realization
Average Unit Price = DIVIDE([Total Sales], [Total Units Sold], 0)
