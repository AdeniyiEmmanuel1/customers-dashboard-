# **Customers Dashboard | Tableau Project**

## **Objectives**

An end-to-end data analytics project that transforms raw customer, product, and order data into a fully interactive Tableau dashboard. The project follows a structured 4-step dashboard design process and covers SQL data cleaning, Excel validation, Tableau calculated fields, and professional dashboard layout design.

---------------------------------------


## **Dashboard Preview**


[Insert image here — add this line to your README.md: ![Customers Dashboard](Customer_Dashboard.png)]

-----------------------------------------

## **Project Overview**

This dashboard provides an executive-level view of customer behaviour, order trends, and sales performance with full interactivity through dynamic filters for year, product category, sub-category, region, state, and city.


### **Dashboard Features**

•	**KPI Cards:** Total Customers, Total Orders, Total Sales: each with year-on-year % change vs. Prior Year

•	Sparkline trend lines on each KPI with highest month (orange dot) and lowest month (blue dot) highlighted

•	**Customer Distribution chart:** shows how many customers placed 1, 2, 3, 4, 5, or 6+ orders

•	**Top 10 Customers by Profit:** ranked table with customer name and most recent order date

•	**Dynamic Filter Panel:** Year, Category, Sub-Category, Region, State, City

•	Navigation buttons to switch between Sales Dashboard and Customers Dashboard views

### **Tools & Technologies**

•	**Microsoft Excel:** Source data exploration and initial validation

•	**SQL Server:** Data cleaning, joining Customers, Products, and Orders tables, type checking and transformation

•	**Tableau Desktop:** All visualisations, calculated fields, KPI design, container layout, and dashboard assembly

### *Dataset*

•	**Customer.csv:** Customer ID, name, segment, region, state, city

•	**Products.csv:** Product ID, category, sub-category, product name

•	**Orders.csv:** Order ID, customer ID, product ID, order date, sales, profit, quantity

### **Dashboard Design Process**

This project followed the 4-step dashboard design methodology:

9.	Step 1: Analyse Requirements: Collected user story requirements, chose appropriate chart types, drew mockups, and selected a colour palette.
    
10.	Step 2: Build Data Source: Connected the three CSV files in Tableau, created the data model by joining tables, renamed fields, checked data types, and explored the data.
    
11.	Step 3: Build Charts: Created calculated fields and tested them, built each individual chart, then formatted by removing gridlines, cleaning axis headers, applying colours, and adding tooltips.
  
12.	Step 4: Build Dashboard: Drew a container mockup, created the vertical and horizontal container structure in Tableau, assembled all charts, distributed objects evenly, added legends, applied inner and outer padding, added dynamic filters, and added navigation icons.
    
### **Key Calculated Fields in Tableau**

•	Total Customers: SUM(IF [Metric] = 'Total Customers' THEN [Value] END)

•	Total Orders: SUM(IF [Metric] = 'Total Orders' THEN [Value] END)

•	Total Sales: SUM(IF [Metric] = 'Total Sales' THEN [Value] END)

•	YoY % Change: (Current Year Value - Prior Year Value) / ABS(Prior Year Value), formatted as percentage

•	Top 10 Customers by Profit: RANK(SUM([Profit])) with computed table calculation


### **Project File Structure**

•	Customer_Dashboard.png: Final Tableau dashboard screenshot

•	Customer.csv: Customer dataset

•	Products.csv: Products dataset

•	Orders.csv: Orders dataset

•	README.md: Project documentation


### **How to Explore This Project**

17.	Clone the repository: git clone https://github.com/YOUR-USERNAME/customers-dashboard.git
    
19.	Open Tableau Desktop and connect to the three CSV files (Customer.csv, Products.csv, Orders.csv).
    
21.	Join the tables on Customer ID and Product ID as shown in the data model.
    
23.	Recreate or explore the calculated fields listed above.
    
25.	Rebuild or reference the dashboard using the container structure described in Step 4.
    
### **Acknowledgement**

This project was built following mentorship with Baraa. The dashboard design process, container mockup methodology, and project steps are credited to his mentorship. 

## **Author**

Created by Aden Emmanuel 

LinkedIn: https://www.linkedin.com/in/aden-emmanuel-117440142/

GitHub: 
