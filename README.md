# 🛒 Superstore Multi-Page Executive & Product BI Report (Power BI)

## 📌 Project Overview
An advanced, multi-page **Power BI** business intelligence solution built to analyze retail enterprise operations. The project provides high-level executive financial metrics on one page and granular product/logistics dynamics on another, utilizing dynamic bookmarks for an interactive pop-up filter pane.

---

## 📷 Dashboard Previews

### 1. Executive Summary View
![Executive Summary](images/executive_summary.png)

### 2. Interactive Filter Pane (Bookmarks & Selection Pane)
![Filter Pane](images/filter_pane.png)

### 3. Product & Logistics Analysis View
![Product Analysis](images/product_analysis.png)

---

## 📊 Key Insights & Metrics

### 🏢 Page 1: Executive Summary
* **Financial Overview:**
  - **Total Sales:** **$2.30M**
  - **Total Profit:** **$286.40K**
  - **Overall Profit Margin:** **12.47%**
* **Year-over-Year (YoY) Performance:**
  - Rapid recovery and surge in sales growth reaching **+29% YoY in 2018**, followed by steady expansion (**+20% YoY in 2019**).
* **Shipping Performance:**
  - **Standard Class** represents the vast majority of volume (**$1.36M**), followed by **Second Class ($459K)** and **First Class ($351K)**.
* **Geographical Distribution (Treemap):**
  - **West ($725.46K)** and **East ($678.78K)** lead revenue generation, outperforming Central and South markets.

### 📦 Page 2: Product & Logistics Analysis
* **Operational Performance:**
  - **Average Shipping Days:** **3.93 Days** order-to-ship cycle.
  - **Average Discount Rate:** **10.93%**.
* **Category Profit Dynamics:**
  - **Office Supplies:** Achieves the healthiest profit margin (**23.82%**) with 7,235 items sold.
  - **Technology:** Delivers high volume with strong margin (**17.58%**).
  - **Furniture:** High sales volume ($252.6K) but operates at a narrow margin (**4.55%**).
* **Top Profit Generating Products:**
  - Led by **Canon imageCLASS 2200 Advanced Copier** generating ~$6.7K net profit.

---

## 🛠️ Advanced DAX & BI Architecture

* **Time Intelligence & DAX Measures:**
  - `YoY Sales Growth = DIVIDE([Total Sales] - [Previous Year Sales], [Previous Year Sales], 0)`
  - Cumulative Running Total by day/year.
  - Profit Margin %: `DIVIDE([Total Profit], [Total Sales], 0)`
  - Average Shipping Duration: `AVERAGE(DATEDIFF(Orders[Order Date], Orders[Ship Date], DAY))`
* **UX/UI & Advanced Interactivity:**
  - **Interactive Pop-up Filter Pane:** Built using Power BI **Bookmarks**, **Selection Pane**, and action buttons to maximize canvas workspace.
  - Slicers reset button ("Clear all slicers").
  - Unified Cyan & Dark Slate theme.

---

## 🚀 How to Run Locally

1. Clone the repository:
   ```bash
   git clone [https://github.com/zaidziad/superstore-bi-executive-dashboard.git](https://github.com/zaidziad/superstore-bi-executive-dashboard.git)
