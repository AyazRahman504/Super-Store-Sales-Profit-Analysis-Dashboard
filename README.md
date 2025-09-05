
# 🏬 Super Store Sales Dashboard  

🔗 **[Dashboard Link](https://app.powerbi.com/links/6cTM6Msjdb?ctid=20f04eaf-31a8-4701-b965-9be849057364&pbi_source=linkShare)**

---

## 📌 Problem Statement  
This dashboard provides **Super Store** with a detailed analysis of **sales performance, customer behavior, product categories, and profitability** across regions.  
With KPIs on **total sales, profit, orders, shipping performance, and profit margin**, the dashboard helps identify **high-performing areas, optimize operations, and forecast future growth**.  

Through **segment, category, and payment mode analysis**, management can make informed decisions to **improve profitability, enhance customer satisfaction, and strengthen sales strategies**.  

---

## 🛠 Steps Followed  

1. **Load Data:** Imported the `SuperStore_Sales_Dataset.csv` into Power BI Desktop.  
2. **Data Quality Check:** Used Power Query Editor to check for nulls, duplicates, and incorrect data types.  
3. **Date Conversion:** Converted `Order Date` and `Ship Date` fields into date format.  
4. **Remove Redundant Columns:** Dropped empty fields (`ind1`, `ind2`).  
5. **Data Modeling:** Established relationships between order, customer, and product attributes.  
6. **Apply Theme:** Used a custom theme for visual consistency.  
7. **Add KPI Cards:** Created visuals for key metrics: **Total Sales, Total Profit, Total Orders, Avg. Ship Days, Profit Margin**.  
8. **Add Filters & Slicers:** Added slicers for **Region** and **Year** for flexible analysis.  
9. **Visualizations Built:**  
   - **Pie/Donut Charts:** Sales by Segment & Payment Mode  
   - **Line Charts:** Monthly Sales & Profit Trends (2019–2020)  
   - **Bar Charts:** Sales by Category & Sub-Category, Sales by Ship Mode  
   - **Map Visual:** State-wise Sales and Profit distribution  
10. **Forecasting:** Applied **Power BI forecasting** to Sales and Profit trends for the upcoming January month of 2021. 

---

## 📐 DAX Expressions Used  

- **Profit Margin**  
```DAX
Profit Margin = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Sales]))
```  

- **Average Shipping Days**  
```DAX
Avg Ship Days = AVERAGEX(Sales, DATEDIFF(Sales[Order Date], Sales[Ship Date], DAY))
```  

- **Total Orders**  
```DAX
Total Orders = DISTINCTCOUNT(Sales[Order ID])
```  

---

## 📊 Key Insights  

### 🔸 Overall Performance  
- **Total Sales:** 1.57M  
- **Total Profit:** 175K  
- **Total Orders:** 22K  
- **Profit Margin:** 11.2%  
- **Avg. Shipping Days:** 4  

### 🔸 Segment & Customer Insights  
- **Consumer Segment** drives nearly half of sales (~48%).  
- **Corporate Segment** contributes 33%, while **Home Office** lags behind.  

### 🔸 Category & Product Insights  
- **Office Supplies** lead in sales (~0.64M), followed by **Technology (~0.47M)** and **Furniture (~0.46M)**.  
- Top-performing sub-categories include **Phones, Chairs, and Binders**.  

### 🔸 Regional & Shipping Insights  
- **Standard Class** is the dominant shipping mode (~0.33M in sales).  
- Certain states consistently outperform others in sales and profitability.  

### 🔸 Payment Mode Insights  
- **Cash on Delivery (COD):** 43%  
- **Online:** 35%  
- **Cards:** 22%  

### 🔸 Forecasting & Trends  
- **Sales show steady growth**, with strong peaks in **Q4 (Nov–Dec)**.  
- **Profits are volatile**, with occasional losses, indicating areas needing cost optimization.  
- **Forecasting** predicts further sales growth into 2021, though profit fluctuations remain a concern.  

---

## 📷 Dashboard Snapshots  

### 📍 Main Dashboard (KPIs & Segment Analysis)  
![Dashboard Overview](https://github.com/AyazRahman504/Super-Store-Sales-Profit-Analysis-Dashboard/blob/main/Assets/Superstore%20Sales%20Dashboard.png?raw=true)  

### 📍 Sales Forecasting  
![Sales Forecasting](https://github.com/AyazRahman504/Super-Store-Sales-Profit-Analysis-Dashboard/blob/main/Assets/Sales%20Forecasting.png?raw=true)  

### 📍 Profit Forecasting  
![Profit Forecasting](https://github.com/AyazRahman504/Super-Store-Sales-Profit-Analysis-Dashboard/blob/main/Assets/Profit%20Forecasting.png?raw=true)  

---

## 🚀 Business Impact  

- **Consumer segment** remains the primary growth driver.  
- **COD payments** dominate but online payments are increasing, signaling digital adoption.  
- **High volatility in profits** requires review of discounts and pricing strategies.  
- **Office Supplies and Technology** categories are key revenue contributors.  
- **Forecasting shows upward growth**, helping management plan future strategies.  
