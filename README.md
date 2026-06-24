# Sales Analysis Dashboard – Power BI Project

## Project Overview
This project is part of the Data Analysis Diploma assignments at Route Academy.  
The objective was to build a fully interactive **Sales Dashboard for a bakery** using **Microsoft Power BI**, starting from raw data and ending with actionable insights.

The project covers the complete data analysis workflow:  
**Data Acquisition → Data Cleaning → Data Modeling → Visualization → Insights**

---

## Dataset
The assignment included three data files:
- **Orders** (Excel)  
- **Cookie Types** (Excel)  
- **Customers** (CSV)

---

## Tools & Technologies
- Microsoft Power BI  
- Power Query  
- DAX  
- Excel / CSV

---

## Data Preparation

### **1. Data Cleaning**
Performed in Power Query:
- Converted the data type of the **Date** column in the Orders table to Date.
- Converted the data type of **Customer ID** and **Zip** columns in the Customers table from Text to Whole Number.

### **2. Data Manipulation**
- The *Cookie Types* table did not include a Cookie ID column, and the “Cookie Type” column was used as a foreign key in the Orders file.  
  To optimize storage and improve functionality, a new **CookieID** column was created and used as the foreign key instead of "Product" column in *Orders* table.
- Created multiple DAX measures for KPIs, including:  
  - Avg No. Cookies per Order  
  - Avg Revenue per Order  
  - Total Units Sold  
  - Total Revenue / Total Cost  
  - And other supporting calculations

---

## Data Visualization

Designed the dashboard to be divided into **4 main pages** for a clear and intuitive analysis experience:

### **1. Home Page**
- Displays overall sales KPIs (Total Revenue, Total Cost, Total Units Sold, etc.)
- Highlights the **Top 1** Cookie Type, Customer, and State by Total Revenue

### **2. Orders Page**
- Shows order-related KPIs (Avg No. Cookies per Order, Avg Revenue per Order, etc.)
- Includes column charts comparing Cookie Types and States by Number of Orders

### **3. Products Page**
- Contains a combo chart showing Cookie Types by:
  - **Total Revenue (Line)**
  - **Total Cost (Column)**
- Additional visuals for product-level performance

### **4. Customers Page**
- Donut charts illustrating Units Sold and Number of Orders per customer  
- Other focused customer performance analysis

### **Filters**
To allow dynamic exploration:
- **Year slicer**  
- **Month slicer**  
Both synchronized across all dashboard pages.

---

## Key Insights
- Chocolate Chip is the top-performing cookie type in both revenue and units sold.
- ACME Bites is the top customer in both revenue and no. orders.
- Despite a small client base (5 customers), their consistent demand contributes to healthy bakery sales.  
- Monthly revenue shows clear seasonal patterns.

---

## Conclusion
This project walks through the end-to-end data analysis process — starting from raw files, cleaning and modeling the data, and creating an interactive dashboard that communicates insights effectively.  

Throughout this assignment, I strengthened my skills in:
- Power Query transformations  
- Data modeling best practices  
- Building meaningful visualizations  
- Writing DAX measures for deeper analysis

### **Future Enhancements**
- Add advanced DAX measures (YoY and MoM comparisons)   
- Automate data refresh for real-time analysis

---
