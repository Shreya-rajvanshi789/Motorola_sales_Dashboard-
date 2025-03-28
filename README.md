# Motorola_sales_Dashboard

# MOTOROLA SALES DASHBOARD
In this project i had created a Dashboard of motorola sales using PowerBI .


### Dashboard Link : https://1drv.ms/u/c/df29bfb6512c5c25/Ea4WRq9EGvVGiEcsmu_oPIMBLWuYKowT9ygiklH7pLmV3w?e=OLOgQV

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
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Arrival Delay".
 
- Step 6 : In the report view, under the view tab, theme was selected.
- step 7 : In the report view, under the insert tab, using shapes option from elements group a rectangle was inserted & similarly using image option company's logo was added to the report design area.

- Step 8 : Visual filter (Slicer) were added for field "Month" .

- step 9 :  New measure was created to find total sales of Motorola.

Following DAX expression was written for the same,
        
        Total_Sales = SUM(Sales_data,[Units Sold]*[Price Per Unit])
        
A card visual was used to represent Total_Sales.

[Image](https://github.com/user-attachments/assets/4c55c6bb-113a-43f2-a40d-0e261b7833f9)




- Step 10 : New measure was created to find total quantity of units sold.

Following DAX expression was written for the same,
        
        Total_quantity = SUM(Sales_data[Units Sold])
        
A card visual was used to represent Total_quantity.

[Image](https://github.com/user-attachments/assets/df96689a-b442-461b-bede-dffc3d64c279)

        
 - Step 11 : New measure was created to find  total no. of Transactions.
 
 Following DAX expression was written for the same,
 
         Transactions = COUNTROWs(Sales_data)
 
 A card visual was used to represent Transactions.
 

 
[Image](https://github.com/user-attachments/assets/8c466d63-ca50-4753-ab81-dda97666da3e)

 
 - Step 12 : New measure was created to calculate Average of price per unit.
 
 Following DAX expression was written to find Average,
 
         Average = average(Sales_data[Price Per Unit])
          A card visual was used to represent Average.
 
 
[Image](https://github.com/user-attachments/assets/ed94b5be-1dc9-416f-85fa-5ff578bd2242)


- Step 13 : Four card visuals were added to the canvas, for "Total_Sales", "Total_Quantity", "Total_Transactions" and "Average" .
           
           Although, by default, while calculating average, blank values are ignored.

- Step 14 : A column chart was also added for representing Total_Sales by Mobile_Models. 

- step 15 : A line chart was added to  represent Total quantity of units sold by month . 

- step 16 : A funnel chart was also added for representing customer ratings via count of customer ratings .

- step 17 : An area chart was added to represent Total sales by day name .

- step 18 : A map is also added to see in which areas sales is high or in which areas it is low by the name of cities .

- step 19 : A Donut chart was also added to represent Total_quantity and Total_Sales by the brands of Mobile Models.



# Insights

A single page report was created on Power BI Desktop . 

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 

 

           
### [2] Average Ratings



 ### [4] Some other insights
 
 
