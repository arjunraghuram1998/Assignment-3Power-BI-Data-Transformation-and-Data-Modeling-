# Assignment-3Power-BI-Data-Transformation-and-Data-Modeling-
Power BI: Data Transformation and Data Modeling 
Power Bi Assignment 1

Power BI Assignment 1 – Data Transformation & Data Modeling 


E-Commerce Sales Analysis , below 3 dataset has been loaded to Power Bi and Transforming data.
List of Orders.csv 
Order Details.csv 
Sales target.csv 

*Data Transformation*: 

1.Restrict the "List of Orders" table to only the first 500 rows has been done - by keep rows option
2.The “Order Date” column in the “List of Orders” table is set to data type 'Date'.- Done
3.Change the data type of “Amount” and “Target” columns to ‘Fixed Decimal Number’. -Done
4.The "CustomerName" column into proper case, capitalization each word - Done
5.Merge the "State" and "City" columns to create a new column named "Location" in the format ‘City, State’ - Done using Merge column option
6.Create a new custom column named "Profit Margin" as the percentage of "Profit" divided by "Amount". - here Profit is in -ve values so profit margin also comes -ve figure. so here created a total sales column and assuming a percentage of sales to it to find profit margin.
7.A new conditional column added - named "Profit Status" based on the values in the "Profit" column. The conditions are as follows: if the profit is less than 0, the label should be "Loss"; if the profit equals 0, the label should be "Break-Even"; and if the profit is greater than 0, the label should be "Profit". 


Merging Data (Joins): 
1. Merge the "List of Orders" and "Order Details" tables into a new single table named 
"Orders Data" based on the "Order ID" relationship. using merge queries done


Handling Missing Data & Duplicate Data: 
1.Identify missing values in the data and determine a strategy to address them. - fill down or up functions /coalesce with 0
2.Check for duplicate rows and define a strategy to handle duplicates. removed by duplicate roving option

Sorting and Filtering Data: 

 In the ‘Orders Data’ table,  sorting and filtering techniques are used to Sort the orders by Order Date in descending order to analyze recent trends &  Filter the orders to focus only on a specific state (e.g., Tamil Nadu) for 
regional analysis.


Grouping and Aggregating Data: 

1. Duplicate the “Order Details” table and calculate the count of each Order ID, average 
profit by Category or total amount by Sub-Category. - done 
2. Duplicate the “Sales Target” table and aggregate the total target amount by Month of 
Order Date. there is no month in dataset, so created using add column.
 
Data Modeling: 

1.Establish a relationship between the “List of Orders” and “Order Details” tables using 
the ‘Order ID’ column. 
2. Build a relationship between the “Order Details” and “Sales Target” tables based on 
the ‘Category’ column. Click "Manage relationships" and ensure this relationship is 
active.


