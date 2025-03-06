# 📊 **Sales Insights Dashboard – Power BI & MySQL** 🚀  

## 🔍 **Project Overview**  
This project provides **deep insights into company sales performance** using **Power BI** for visualization and **MySQL** for data processing. The dashboard helps business users analyze:  

✅ **Revenue trends over time**  
✅ **Top-performing products & customers**  
✅ **Market-wise sales distribution**  
✅ **Total sales revenue & quantity**  

---

## 🛠 **Tools & Technologies Used**  

| 🛠 Tool         | 📌 Purpose |
|-------------|--------------------------------------------------|
| **Power BI** | Data visualization & interactive dashboards  |
| **MySQL**   | Database management & data transformation |
| **Power Query** | Pre-processing data before importing to Power BI |
| **DAX** | Custom calculations & measures in Power BI |
| **Python** | Additional data validation & visualization |

---

## 🏗 **Data Pipeline & Sources**  

### **1️⃣ Data Extraction & Transformation**  
🔹 **Source:** MySQL Database  
🔹 **Processing:** All **Power Queries were executed directly in MySQL**  
🔹 **Export:** Processed data tables were exported from MySQL to **CSV format**  

### **2️⃣ Datasets Used**  
The following **9 datasets** were extracted & used in Power BI:  

| 📂 Dataset Name       | 📊 Columns | 📄 Description |
|----------------------|-----------|-------------|
| **Revenue_YOY**        | Revenue, cy_date | Year-over-Year revenue trends |
| **Top_5_Products**     | Revenue, product_code | Top 5 revenue-generating products |
| **Top_5_Customers**    | custmer_name, Revenue | Top 5 highest-paying customers |
| **Dates**              | cy_date | Time dimension for trend analysis |
| **Years**              | year | Distinct years in dataset |
| **Revenue**            | Revenue | Total revenue summary |
| **SalesQty**          | Sales Qty | Total sales quantity summary |
| **Revenue_by_Markets** | Revenue, markets_name | Market-wise revenue distribution |
| **Sales_Qty_by_Markets** | Sales Qty, markets_name | Market-wise sales quantity |

---

## 📊 **Key Insights from the Dashboard**  

### 📈 **1️⃣ Revenue Trends Over Time**  
📌 **Revenue fluctuates** over time, showing seasonal patterns.  
📌 **Highest revenue recorded on:** **January 1, 2018**  
📌 **Total Revenue:** **₹984,813,463** (≈ ₹984.8 million)  

### 🛒 **2️⃣ Top 5 Products by Revenue**  
📌 **Best-performing product:** *Blank Product*  
📌 **A few products contribute significantly to total revenue**.  

### 👥 **3️⃣ Top 5 Customers**  
📌 **Top revenue-generating customer:** **Electricalsara Stores**  
📌 **Customer retention is key for maintaining revenue.**  

### 🌍 **4️⃣ Market-Wise Revenue & Sales Distribution**  
📌 **Highest Revenue Market:** **Delhi NCR**  
📌 **Market with the Highest Sales Quantity:** **Delhi NCR**  
📌 **Total Sales Quantity:** **2,429,282** units  

---

## 🏗 **Data Model & Relationships**  

📌 **Fact Tables:**  
🔹 `Revenue_YOY`  
🔹 `Revenue_by_Markets`  
🔹 `Sales_Qty_by_Markets`  

📌 **Dimension Tables:**  
🔹 `Top_5_Customers`  
🔹 `Top_5_Products`  
🔹 `Dates`  
🔹 `Years`  

📌 **Key Relationships:**  
✔ `Dates` ↔ `Revenue Tables` (cy_date)  
✔ `Markets` ↔ `Revenue & Sales Tables` (markets_name)  
✔ `Customers & Products` ↔ `Revenue Tables` (customer_name, product_code)  

---

## 🚀 **How to Use the Dashboard**  

✅ **Apply Filters:** Select **dates, products, customers, or markets** to drill down into details.  
✅ **Hover Over Graphs:** See **detailed tooltips** with insights.  
✅ **Switch Between Pages:** Explore different **report views** in Power BI.  
