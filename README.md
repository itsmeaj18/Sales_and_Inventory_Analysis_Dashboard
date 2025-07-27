# 📊 Sales & Inventory Analysis Dashboard (Power BI)

This Power BI project provides an in-depth **Sales and Inventory Analysis** using Microsoft’s AdventureWorks2022 dataset. It is designed to give clear and actionable business insights through interactive visuals and drill-down reports.

---

## 📦 Dataset

The dashboard is built using the **AdventureWorks2022** dataset by Microsoft.

🔗 **Download Dataset (.bak)**:  
[AdventureWorks2022.bak](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks2022.bak)

To use:
- Restore the `.bak` file into your **SQL Server Management Studio (SSMS)**.
- Connect Power BI to your local SQL Server instance.
- Use the views or tables as needed to build the data model.

---

## 📈 Dashboard Overview (4 Pages)

### 1. **Sales Overview**
Provides a high-level view of sales performance from 2011–2014:
- 📅 Sales trends over time (line chart)
- 🌍 Sales distribution by region (pie chart)
- 🧱 Sales by product category (bar chart: Bikes, Components, Clothing, Accessories)
- 📌 KPIs: Total Sales, Total Orders, Average Order Value

---

### 2. **Sales Details**
Drills into individual transactions and sales orders:
- 📋 Detailed sales table (SalesOrderID, CustomerID, Product, Quantity, Line Total)
- 👤 Sales by Salesperson (bar chart)
- 🏆 Top Products by Sales Volume (table with revenue per product)

---

### 3. **Inventory Overview**
Shows an overall picture of current inventory:
- 🔢 Total Inventory (card)
- ❌ Out-of-Stock Products (card + table)
- 🧮 Inventory by Product (bar chart)
- 🕒 Inventory Trends Over Time (line chart)
- 🗺️ Inventory by Location (bar chart: Northwest, Southwest, UK, Canada, etc.)

---

### 4. **Inventory Detail**
A deep dive into inventory at product-location level:
- 📍 Inventory by Product and Location (table)
- 📊 Inventory Movement (bar chart by Year & Month showing Inventory In/Out)
- 🔁 Movement KPIs: Inventory In, Inventory Out, Net Movement

---

## 🔧 Tools Used

- **Power BI Desktop**
- **SQL Server** (to host the AdventureWorks2022 DB)
- **DAX** for custom measures
- **SQL Views** for data modeling

---

## 📄 SQL Views Used

The Power BI data model was enhanced using SQL views, including:
1. `SalesByProductcategoryCustomer` – Aggregated sales by product, category, and customer
2. `InventoryLevelsByLocationProduct` – Inventory data by product and warehouse location

See `documentation.pdf` for full SQL code reference.

---

## 🧭 How to Use This Dashboard

1. Download the `.pbix` file from this repository.
2. Restore the **AdventureWorks2022.bak** in your local SQL Server.
3. Open the Power BI file and update the **SQL Server connection**.
4. Refresh data and explore 4 interactive dashboard pages.

---

## 🧑‍💻 Author

**Ajinkya Itale**  
📧 ajinkyaitale18@gmail.com  
[🔗 LinkedIn](https://www.linkedin.com/in/ajinkya-itale-b8048721b)

---

## 📃 License & Credits

- Dataset © Microsoft (for educational/demo use)  
- Dashboard design and implementation © Ajinkya Itale

🔗 Microsoft Sample Dataset License:  
https://github.com/Microsoft/sql-server-samples#license
