# Pizza Sales Report - Power BI Project

## Project Overview
This Power BI project analyzes pizza sales across multiple branches over a 12-day period. The report provides insights into sales performance by state, store manager, and pizza type. It also compares actual sales against daily targets, helping to monitor and improve branch performance.

---

## Data Sources

The project uses three raw Excel files:

1. **Branch Data**
   - Columns: Branch, Manager Name, Country
   - Operations:
     - First row used as header
     - Columns renamed appropriately
     - Branch renamed to **State** for dashboard consistency

2. **Daily Target**
   - Columns: Day, Target
   - Operations:
     - Target formatted as currency with fixed decimals

3. **Sales Table**
   - Columns: S/N, Date, Branch, Pizza Type, Quantity, Time, Time Range, Price
   - Operations:
     - Custom column created in Query Editor: `Sales Amount = Quantity * Price`

---

## Data Model Relationships
- **Daily Target → Sales**: Day (one) to Date (many)  
- **Branch Data → Sales**: Branch (one) to Branch (many)

---

## Dashboard Features

1. **Design Elements**
   - Background applied with pizza-themed visuals
   - Pizza logo and title: *Debashis’ Pizza*
   - Section separators for clarity

2. **Visualizations**
   - **Total Sales:** Card using `Sales Amount` column  
   - **Sales Amount by State:** Shape map using `State` column for interactive filtering  
   - **Sales Amount by Store Manager:** Donut chart using Manager Name and `Sales Amount`, manager logo added  
   - **Sales vs Target by Day:** Clustered bar chart using Day, Target, and `Sales Amount`  
   - **Sales Amount by Pizza Type:** Stacked column chart using Pizza Type and `Sales Amount`  
   - **Slicer:** State selector (5 given state names)

---

## Operations Performed
- Data cleaning and formatting in Query Editor  
- Currency and decimal formatting applied to targets  
- Calculated columns created for sales analysis  
- Relationships defined between tables to enable interactive filtering  

---

## Key Insights
- State-wise sales performance  
- Manager-wise performance evaluation  
- Daily comparison of sales against targets  
- Pizza type popularity trends

---

## Tools Used
- **Power BI Desktop** for dashboard creation and data modeling  
- **Excel** for raw data   

---

![Capture](https://github.com/user-attachments/assets/8d2e827c-1ab9-4153-bfb1-99829460c47b)
