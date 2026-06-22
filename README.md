# **Sales & Customers Dashboard | Tableau Project**

An end-to-end Tableau analytics project featuring two fully interactive, navigation-linked dashboards, a Sales Dashboard and a Customers Dashboard built from three relational datasets cleaned in SQL Server and Excel. The project follows the structured 4-step  dashboard design methodology from the Tableau Ultimate Course 

------------------------------------------------------------------

## **Dashboard Previews**

https://github.com/AdeniyiEmmanuel1/customers-dashboard-/blob/main/Sales%20Dashboard.png



------------------------------------------------------------------------

## **Project Overview**


This project provides an executive-level view of sales performance and customer 

behaviour across multiple years, product categories, and geographies. Both dashboards 

share a single filter panel and are connected via navigation buttons, allowing users to 

switch between the Sales view and the Customers view instantly.

## **Sales Dashboard - Features & KPIs**

	  •	Total Sales KPI - $733K with ▲20.36% year-on-year change vs. Prior Year, monthly sparkline with highest and lowest month dots
	  
	  •	Total Quantity KPI — $12K with ▲26.83% vs. PY
	  
	  •	Total Profit KPI — $93K with ▲14.24% vs. PY

•	Sales & Profit Performance by Sub-Category - dual horizontal bar chart showing sales (dark) vs. profit/loss (blue/orange) per product line; Tables and Bookcases highlighted as loss-making

•	Sales and Profit Trends Over Time — dual step-line chart with dashed average reference lines (Avg. $4K sales, Avg. $1K profit) showing above/below average periods

## **Customers Dashboard - Features & KPIs**

	•	Total Customers KPI: 573 with ▼3.70% vs. PY, monthly sparkline
	
	•	Total Orders KPI: ▲7.12% vs. PY with trend line
	
	•	Total Sales KPI: ▲0.90% vs. PY
	
	•	Customer Distribution by Number of Orders — bar chart showing 262 customers placed 1 order, 199 placed 2, tapering to 2 customers who placed 6 orders
	
	•	Top 10 Customers by Profit: ranked table showing customer name and most recent order date
	
	•	Dynamic filter panel: Year, Category, Sub-Category, Region, State, City

# **Navigation & Interactivity**

Both dashboards include navigation icon buttons in the top right corner. Clicking the bar chart icon navigates to the Sales Dashboard. Clicking the people icon navigates to the Customers Dashboard. The filter panel is accessible from both dashboards via the funnel icon. This creates a seamless single-project experience across two dashboard views.

# **Tools & Technologies**

	•	**Microsoft Excel:** Source data exploration and initial validation of all three datasets
	
	•	**SQL Server:** Data cleaning, joining Customers, Products, and Orders tables, data type validation, null handling, and transformation
	
	•	**Tableau Desktop:** All visualisations, calculated fields, KPI design, sparklines, container layout, navigation button actions, and dashboard assembly

## **Datasets**

	•	**Customer.csv:** Customer ID, customer name, segment, region, state, city
	
	•	**Products.csv:** Product ID, category, sub-category, product name
	
	•	**Orders.csv:** Order ID, customer ID, product ID, order date, sales, profit, quantity

## **Dashboard Design Process**

**This project followed the 4-step dashboard design methodology:**

	Step 1: Analyse Requirements: Defined user stories and KPI requirements for both dashboards, chose appropriate chart types (sparklines, dual bar charts, step-line charts, ranked tables), sketched mockups, and selected the blue/orange colour palette.
	   
	Step 2: Build Data Source: Connected all three CSV files in Tableau, created the data model by joining on Customer ID and Product ID, renamed fields and tables, checked data types, and explored the data.
	   
	Step 3: Build Charts: Created and tested all calculated fields, built each individual chart, then formatted each by removing gridlines, cleaning axis headers, applying consistent colours, and adding tooltips.
	   
	Step 4: Build Dashboard: Drew container mockups for both dashboards, created the vertical main container with horizontal rows for title, KPIs, and charts, added a separate filter panel container, distributed objects evenly, set inner/outer padding, added legends, added navigation button actions, and added icons.
   
## **Key Calculated Fields in Tableau**

	•	Total Sales: SUM([Sales])
	
	•	Total Profit: SUM([Profit])
	
	•	Total Quantity: SUM([Quantity])
	
	•	Total Customers: COUNTD([Customer ID])
	
	•	Total Orders: COUNTD([Order ID])
	
	•	CY (Current Year): Filtered by selected year parameter
	
	•	PY (Prior Year): LOOKUP(SUM([Sales]), -1) computed along Year dimension
	
	•	YoY % Change: (CY Value - PY Value) / ABS(PY Value), formatted as percentage with ▲▼ indicator
	
	•	Top 10 Customers by Profit: RANK(SUM([Profit])) as a table calculation

## **Project File Structure**

	•	Sales_Dashboard.png: Sales Dashboard screenshot
	
	•	Customer_Dashboard.png: Customers Dashboard screenshot
	
	•	Customer.csv: Customer dataset
	
	•	Products.csv: Products dataset
	
	•	Orders.csv: Orders dataset
	
	•	README.md: Project documentation

## **How to Explore This Project

	> Clone the repository: git clone https://github.com/YOUR-USERNAME/sales-customers-dashboard.git
		
	> Open Tableau Desktop and connect to Customer.csv, Products.csv, and Orders.csv.
	    
	> Join the tables: Orders joined to Customers on Customer ID, Orders joined to Products on Product ID.
	    
	> Create the calculated fields listed above.
	    
	> Build the Sales Dashboard first, then the Customers Dashboard, then add navigation button actions between them.
    
## **Acknowledgement**

This project was built following the Tableau Ultimate Course with the mentorship of baraa. The 4-step dashboard design process, container mockup methodology, and project structure are credited to that course.

Author
Created by [Your Name]
LinkedIn: [Your LinkedIn URL]
GitHub: [Your GitHub URL]

