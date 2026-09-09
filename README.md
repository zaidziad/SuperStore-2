# 🛒 Superstore Multi-Page Executive & Product BI Report (Power BI)

## 📌 Project Overview
An advanced, multi-page **Power BI** business intelligence solution built to analyze retail enterprise operations. The project provides high-level executive financial metrics on one page and granular product/logistics dynamics on another, utilizing dynamic bookmarks for an interactive pop-up filter pane.

---

## 📷 Dashboard Previews

### 1. Executive Summary View
<img width="1418" height="808" alt="Excutive Summary" src="https://github.com/user-attachments/assets/3ade762d-90fa-4528-b1de-53f44f49c17d" />


### 2. Interactive Filter Pane (Bookmarks & Selection Pane)
<img width="1414" height="790" alt="Filter" src="https://github.com/user-attachments/assets/7e1bfc5c-c641-4381-8ee6-c81c559658c8" />


### 3. Product & Logistics Analysis View
<img width="1450" height="810" alt="Product Analysis" src="https://github.com/user-attachments/assets/17c0cd81-1b00-4848-8a41-68333b4e63ef" />


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
