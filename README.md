# Motorola_sales_Dashboard

# MOTOROLA SALES DASHBOARD
In this project i had created a Dashboard of motorola sales using PowerBI .


### Dashboard Link : https://1drv.ms/u/c/df29bfb6512c5c25/Ea4WRq9EGvVGiEcsmu_oPIMBLWuYKowT9ygiklH7pLmV3w?e=3t0Au6

## Problem Statement

This dashboard helps Motorola to improve its sales analysis to make better business decisions.  Currently, sales data is scattered across different regions and products, making it hard to track performance and identify trends. thus to solve this problem, a dashboard is needed to present sales insights in an easy-to-understand way.

This dashboard will help :

- Track Key Metrics : Show total sales, number of transactions, and average sales to measure performance.

- Analyze Sales by Region : Identify the best and worst-performing cities to improve sales strategies.

- Check Product Performance : See which mobile models are selling the most and which need attention.

- Understand Customer Behavior : Analyze customer ratings and buying patterns.

- Predict Future Sales Trends : Use past data to estimate future sales and plan accordingly.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values .
 
- Step 5 : In the report view, under the view tab, theme was selected.
- step 6 : In the report view, under the insert tab, using shapes option from elements group a rectangle was inserted & similarly using image option company's logo was added to the report design area.

- Step 7 : Visual filter (Slicer) were added for field "Month" .

- step 8 :  New measure was created to find total sales of Motorola.

Following DAX expression was written for the same,
        
        Total_Sales = SUM(Sales_data,[Units Sold]*[Price Per Unit])
        
A card visual was used to represent Total_Sales.

![Screenshot 2025-03-28 045210](https://github.com/user-attachments/assets/e3861a82-4f32-477d-acb4-7a5bbce503f6)

- Step 9 : New measure was created to find total quantity of units sold.

Following DAX expression was written for the same,
        
        Total_quantity = SUM(Sales_data[Units Sold])
        
A card visual was used to represent Total_quantity.

![Screenshot 2025-03-28 045001](https://github.com/user-attachments/assets/286dcbfa-64a0-4995-b2c4-9d709367a579)

        
 - Step 10 : New measure was created to find  total no. of Transactions.
 
 Following DAX expression was written for the same,
 
         Transactions = COUNTROWs(Sales_data)
 
 A card visual was used to represent Transactions.

![Screenshot 2025-03-28 045715](https://github.com/user-attachments/assets/8f955700-90da-42b2-9817-d73d231b7e17)

 
 - Step 11 : New measure was created to calculate Average of price per unit.
 
 Following DAX expression was written to find Average,
 
         Average = average(Sales_data[Price Per Unit])
          A card visual was used to represent Average.

![Screenshot 2025-03-28 045901](https://github.com/user-attachments/assets/891b8b7d-4083-447e-8b51-513069d0aeed)


- Step 12 : Four card visuals were added to the canvas, for "Total_Sales", "Total_Quantity", "Total_Transactions" and "Average" .
           
           Although, by default, while calculating average, blank values are ignored.

- Step 13 : A column chart was also added for representing Total_Sales by Mobile_Models. 

- step 14 : A line chart was added to  represent Total quantity of units sold by month . 

- step 15 : A funnel chart was also added for representing customer ratings via count of customer ratings .

- step 16 : An area chart was added to represent Total sales by day name .

- step 17 : A map is also added to see in which areas sales is high or in which areas it is low by the name of cities .

- step 18 : A Donut chart was also added to represent Total_quantity and Total_Sales by the brands of Mobile Models.




# Report Snapshot (Power BI DESKTOP)
![Screenshot 2025-03-31 234533](https://github.com/user-attachments/assets/b45bae5d-3eab-4aae-a8c3-3d390a2d145d)

# Insights

Following inferences can be drawn from the dashboard;

### [1] Total Quntity = 19K

### [2] Customers with Rating 5 = 311

 ### [3] Total Sales = 769M

 ### [4] Region with highest sale = Delhi(204M)

 ### [5] Brand with highest sale = Apple(162M)

### [6] Month with highest sale = July(70M)


 
 
