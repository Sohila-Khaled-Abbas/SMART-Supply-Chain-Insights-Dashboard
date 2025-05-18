# 📦 SMART Supply Chain Insights Dashboard

A comprehensive end-to-end data analytics project using Python, Excel, and Power BI to extract actionable insights from complex supply chain data. This dashboard supports operational and strategic decision-making by visualizing key KPIs in logistics, fulfillment, sales, and fraud detection.

---

## 🔗 Live Dashboard

🌐 [Click here to explore the dashboard](https://app.powerbi.com/view?r=eyJrIjoiNzc1YzdkYWQtZDlkZC00MDhkLWJhNGEtZDg4YzRmMDI5NTljIiwidCI6IjI1Y2UwMjYxLWJiZDYtNDljZC1hMWUyLTU0MjYwODg2ZDE1OSJ9)

---

## 📁 Project Contents

| Folder | Description |
|--------|-------------|
| `1_Raw_Data/` | Original supply chain datasets and metadata. |
| `2_Cleaned_Data/` | Cleaned dataset in Excel format after EDA. |
| `3_Python_EDA/` | Exploratory data analysis and preprocessing using Python. |
| `4_Data_Modeling/` | Star schema design and relationship mapping in Excel. |
| `5_PowerBI_Dashboard/` | Final `.pbix` file, dashboard screenshots, and schema diagram. |

---
## 🛠️ Tools & Technologies

- **Python** (Pandas, Seaborn, Matplotlib, Plotly, Statsmodels ) – EDA & Cleaning  
- **Excel** – Data modeling & star schema  
- **Power BI** – Data visualization, DAX, storytelling  

---

## 🧪 Python Exploratory Data Analysis (EDA)

This project includes comprehensive exploratory data analysis using the following Python libraries:

- **Pandas** for data cleaning and manipulation  
- **Seaborn**, **Matplotlib**, **Plotly** for visualizations  
- **Statsmodels** for statistical modeling (OLS regression, z-score, IQR)

### 🔍 Analysis Scope

- Numeric Feature Distribution  
- Categorical Analysis  
- Sales & Profit Trends  
- Multiple Numerical Features Analysis  
- Fraud Order Analysis  
- Fraud vs. Non-Fraud (Categorical & Numerical Features)  
- Fraud Trend per Month & per Year  
- Top 10 Customers by Fraud & Cancellation  
- Geographic Insights

---

### 📊 Dataset Highlights

| Metric               | Value                  |
|----------------------|------------------------|
| Unique Customers     | 20,652                 |
| Unique Orders        | 65,752                 |
| Unique Products      | 118                    |
| Order Years          | 2015–2018              |
| First Order Date     | 2015-01-01             |
| Last Order Date      | 2018-01-31             |
| First Shipping Date  | 2015-01-03             |
| Last Shipping Date   | 2018-02-06             |

> ✅ The dataset spans 4 years of transactions, cleaned and validated using Python (Pandas) for BI readiness.

---

## 📌 Key Visual Insights

### 1. Distribution Overview  
Histograms show distribution of:

- **Shipping time**, **delivery risk**, **product pricing**
- **Order quantity**, **discount rates**, **profit ratio**
- **Latitude and longitude** (geo-distribution)

**Business Value**:
- Detect anomalies in shipping and delivery  
- Understand customer & product behavior  
- Optimize pricing and discount strategies  
- Segment regions for targeted action  

---

### 2. 📈 Overall Order Volume Trend (2015–2018)

- **Trend**: Stable volume until mid-2017 → sharp drop in Q3 2017  
- **Interpretation**: Potential system migration, policy shifts, or external disruption  
- **Use**: Plan for seasonal patterns, predict demand, manage risk

---

### 3. 🔥 Correlation Heatmap

| Variable Pair                             | Correlation |
|------------------------------------------|-------------|
| Sales vs Sales per Customer              | +0.99       |
| Profit Ratio vs Benefit per Order        | +0.82       |
| Delivery Risk vs Days to Ship            | –0.37       |
| Product Price vs Item Price              | +0.78       |

---

### 4. 📦 Operational Categorical Patterns

- **Payment Method**: DEBIT most common  
- **Shipping Mode**: Standard dominates, minimal Same Day  
- **Delivery Status**: Majority marked “Late Delivery”  
- **Customer Segment**: Mostly consumers in the USA  
- **Market & Department**: LATAM and Europe; Apparel and Golf top sectors  
- **Order Status**: “COMPLETE” and “PENDING_PAYMENT” dominate  

---

### 5. 🌍 Geographic Insights

- **Top Categories**: Cleats, Men’s Footwear, Women’s Apparel  
- **Top Countries**: USA, France, Mexico, Germany  
- **Top Regions**: Central America and Western Europe  
- **Top States**: Puerto Rico, California, New York

---

### 6. 📅 Sales & Order Trend Analysis

- **Sales Peak**: October each year  
- **Order Volume**: January leads consistently  
- **2017**: Highest annual orders and revenue  
- **Drop in 2018**: Significant decline, likely strategic or operational

---

### 7. 🧠 Advanced Statistical Analysis

#### 🔍 Fraud Detection
- **Anomaly Detection** using **z-score** and **IQR** methods  
- Visualized fraudulent patterns across geography, customer segment, and delivery risk

#### 📉 OLS Regression

- Modeled **Profit per Order** with:
  - Discount rate: –65.28 (p < 0.001)
  - Quantity: +34.74 (p < 0.001)
  - Product price: +0.14 (p < 0.001)
- **R² = 0.026**, indicating other factors influence profit

---

## 💡 Recommendations

- Set **discount limits** and use targeted promotions  
- Incentivize **bulk orders** with loyalty offers  
- Implement **dynamic pricing** to avoid underpriced SKUs  
- Analyze other features like **returns** and **shipping cost** in future iterations

---


## 📊 Dashboard Pages

1. **Order & Fulfillment Performance**  
   - Tracks key order KPIs, delays, and fulfillment rates.

2. **Customer & Market Insights**  
   - Regional performance, customer segments, and market trends.

3. **Product & Profitability Overview**  
   - Top categories, margin analysis, and stock insights.

4. **Shipping & Delivery Performance**  
   - Carrier delays, delivery risk, and on-time metrics.

5. **Time Intelligence & Trends**  
   - Month-to-date, year-to-date, seasonal KPIs, fraud heatmaps, and trends.

---

## 📌 Key Features

- ✅ Star schema modeling in Excel
- ✅ Calendar table using DAX (Power BI)
- ✅ Advanced DAX for time intelligence (MTD, YTD, QTD, Rolling Metrics)
- ✅ Fraud vs Non-Fraud analysis (categorical & numerical)
- ✅ Dynamic filters by Market, Region, Category
- ✅ Custom visuals with conditional formatting and KPI cards

---

## 📥 How to Use

1. Clone the repo  
2. Explore the Jupyter notebook for data understanding  
3. Open `DataCo_StarSchema.xlsx` to view the data model  
4. Open `SMART_SupplyChain_Dashboard.pbix` in Power BI Desktop  
5. Interact with the dashboard or view it [live here](https://app.powerbi.com/view?r=eyJrIjoiNzc1YzdkYWQtZDlkZC00MDhkLWJhNGEtZDg4YzRmMDI5NTljIiwidCI6IjI1Y2UwMjYxLWJiZDYtNDljZC1hMWUyLTU0MjYwODg2ZDE1OSJ9)

---

## 🧠 Author

**Sohila Khaled Abbas**  
🔗 [LinkedIn](https://www.linkedin.com/in/sohilakabbas)  
📧 sohilakhaledabbas@outlook.com

---

## 📌 License

This project is open-source and available under the [MIT License](LICENSE).

