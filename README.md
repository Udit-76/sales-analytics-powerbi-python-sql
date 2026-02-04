# sales-analytics-powerbi-python-sql
# 📊 Sales Performance Analysis | Python • SQL • Power BI

A complete end-to-end Data Analytics project demonstrating data cleaning, EDA, SQL querying, and interactive dashboard creation using Power BI.  
This project is designed to showcase the skill set of a Data Analyst: Python, SQL, Visualization, and Business Insights.

---

## 🚀 Project Overview
The goal of this project is to analyze sales performance to understand:

- Top-performing products and categories  
- Regional profitability  
- Customer behavior  
- Sales trends over time  
- Key metrics such as revenue, profit, and quantity sold  

The final deliverable is an interactive **Power BI Dashboard** supported by Python-based EDA and SQL queries.

---

# 📁 Folder Structure

```
Sales-Performance-Analysis/
│
├── data/
│   └── cleaned_superstore_data.csv
│
├── notebooks/
│   └── Sales_Analysis_Python.ipynb
│
├── dashboard/
│   └── Sales_Dashboard.pbix
│
├── images/
│   ├── dashboard_preview.png
│   └── kpi_section.png
│
└── README.md
```


---

## 🛠 Tools & Technologies Used

### **🔹 Python**
- Pandas (Data Cleaning & Transformation)
- NumPy
- Matplotlib / Seaborn (Visual EDA)
- Jupyter Notebook

### **🔹 SQL**
- Data extraction
- Filtering, grouping, aggregation
- Analytical queries

### **🔹 Power BI**
- Data modeling  
- DAX for KPIs  
- Interactive dashboard  

---

## 🧹 1. Data Cleaning (Python)

Key steps performed in Python:

- Handled missing values  
- Removed duplicates  
- Converted date columns  
- Standardized categorical values  
- Added calculated fields (profit %, discount impact, etc.)  

Example code snippet:

```python
df['Order Date'] = pd.to_datetime(df['Order Date'])
df.drop_duplicates(inplace=True)
df['Profit Margin'] = (df['Profit'] / df['Sales']) * 100
```

The cleaned dataset is saved as:  
✔ `cleaned_superstore_data.csv`

---

## 📊 2. Exploratory Data Analysis (Python)

Performed EDA to understand:

- Category-wise sales performance  
- Most profitable sub-categories  
- Monthly sales trends  
- Region-wise breakdown  

Charts created:
- Bar charts  
- Line charts  
- Heatmaps  
- Top 10 products  

Notebook is available here:  
✔ `/notebooks/Sales_Analysis_Python.ipynb`

---

## 🗄 3. SQL Analysis (Optional)

Sample SQL queries used:

```sql
SELECT Category, SUM(Sales) AS TotalSales
FROM sales
GROUP BY Category
ORDER BY TotalSales DESC;
```

```sql
SELECT Region, SUM(Profit) AS TotalProfit
FROM sales
GROUP BY Region;
```

---

## 📈 4. Power BI Dashboard

The dashboard includes:

### **✨ KPI Cards**
- Total Sales  
- Total Profit  
- Avg Profit Margin  
- Total Quantity Sold  

### **📊 Visuals**
- Sales by Category (Bar Chart)
- Profit by Region (Map)
- Monthly Sales Trend (Line Chart)
- Top 10 Products (Bar Chart)
- Customer Segment Breakdown (Donut Chart)

### Dashboard Preview  
📌 *(screenshot stored under `/images/dashboard_preview.png`)*  
![Dashboard Preview](images/dashboard_preview.png)

---

## 🔍 Key Insights

- Technology category contributes the highest sales.  
- East region is the most profitable.  
- Some products with high sales show low profit margin → discount impact.  
- Sales peak during November–December due to seasonal trends.  

---

## 🧾 Conclusion

This project demonstrates:

✔ Data Cleaning (Python)  
✔ SQL for business insights  
✔ EDA for patterns  
✔ Power BI dashboard development  
✔ End-to-end analyst workflow  

---

## 📬 Connect With Me  
If you found this project interesting, feel free to connect with me:

🔗 **LinkedIn:** *add your link*  
🔗 **GitHub:** *add your profile*  

---

## ⭐ If you like this project, consider giving it a star on GitHub!

