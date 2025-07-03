# Digital-Skill-up-Africa-Projects
## Amazon Product Data Analysis – Excel Project 
## Table of Contents
- [Project Overview](#project-overview)
- [Tools Used](#tools-used)
- [Step 1: Data Cleaning](#step-1-data-cleaning)
- [Step 2: Data Analysis](#step-2-data-analysis)
- .[Step 3: Dashboard Creation](#step-3-dashboard-creation)
- [Insights Derived](#insights-derived)
- [Final Dashboard](#final-dashboard)
- [Files in this Repository](#files-in-this-repository)
- [Oluwatosin Moses Adebayo(Author)](#author)

### Project Overview
 
This project focuses on analyzing Amazon product data using Excel tools like Power Query Editor, Pivot Tables, and Dashboarding. The goal was to clean, analyze, and visualize key insights from customer reviews, product ratings, and pricing data.
### Dataset Description 
The dataset contains information scraped from Amazon products 
* Product details: name, category, price, discount, and ratings 
* Customer engagement: user reviews, titles, and content 
* Each row represents a unique product, with aggregated reviewer data 
stored as comma-separated values. 
* Total Records: 1,465, TotalFields: 16 columns 
### Project Objective.
1. What is the average discount percentage by product category? 
2. How many products are listed under each category? 
3. What is the total number of reviews per category?  
4. Which products have the highest average ratings? 
5. What is the average actual price vs the discounted price by category? 
6. Which products have the highest number of reviews? 
7. How many products have a discount of 50% or more? 
8. What is the distribution of product ratings (e.g., how many products are rated 3.0, 
4.0, etc.)? 
9. What is the total potential revenue (actual_price × rating_count) by category? 
10. What is the number of unique products per price range bucket (e.g., <₹200, 
₹200–₹500, >₹500)? 
11. How does the rating relate to the level of discount? 
12. How many products have fewer than 1,000 reviews? 
13. Which categories have products with the highest discounts? 
14. Identify the top 5 products in terms of rating and number of reviews combined.
### Tools Used
* Excel Power Query Editor
* Pivot Tables
* Excel Formulas (IF, COUNTIF, SUM, AVERAGE,)
* Charts & Shapes
* Dashboard Design Tools (Colors, Images, Formatting)

## Step 1: Data Cleaning
* Used Power Query Editor to clean raw data
* Replaced errors and null values
* Removed irrelevant rows/columns
* Used Text to Columns to split long category strings into subcategories
* Renamed column headers for clarity and readability
* Converted data types to appropriate formats (e.g., numbers, dates)
* Standardized the currency format for price-related columns

## Step 2: Data Analysis
 ### Exploratory Data Analysis 
1. Used Pivot Tables to group and summarize data by:
 * Product category
 * Ratings
 * Discount percentage
 * Actual Price
 * Count of Reviews
 * Discount level( price range bucket)
2.  Applied Excel formulas:
 * IF() to flag conditions (e.g., high-rated products)
 * COUNTIF() and SUM() to count and aggregate metrics
 * AVERAGE() for mean rating and pricing
 * Percentage calculations for discount and performance insights
 
 ## Step 3: Dashboard Creation
 ### Designed an interactive and visually appealing Excel dashboard
 Added:
 
  * Charts (bar, pie, line) for key insights
  * Shapes and icons for structure and emphasis
  * Images (e.g., products or Amazon logo)
  * Color fills and consistent theme for a clean layout
  *  -  Excel Analysis [Download Here]https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/main/Amazon%20project%20Cases%20Study%20One.xlsx
       
![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/1786cc85ab6f38a7ff6d7930c6eaddcfc0d11a31/Amazon%20Retail%20product%20Dashboard.png)
 
 ## Insights Derived
 * Top-performing product categories
 * Price vs. Rating correlation
 * Products with highest discounts
 * Average customer satisfaction metrics
### Files in this Repository 


## Oluwatosin Moses Adebayo


# Kultra Inventory Analysis using SQL
## Table of Contents

1. [Project Overview](#project-overview)  
2. [Dataset Overview](#dataset-overview)  
3. [Analysis Questions & SQL Queries](#analysis-questions--sql-queries)  
    3.1. [Product Category with Highest Sales](#1-product-category-with-highest-sales)  
    3.2. [Top 3 and Bottom 3 Regions by Sales](#2-top-3-and-bottom-3-regions-by-sales)  
    3.3. [Total Sales of Appliances in Ontario](#3-total-sales-of-appliances-in-ontario)  
    3.4. [Most Valuable Customer & Their Common Purchases](#4-most-valuable-customer--their-common-purchases)  
    3.5. [Small Business Customer with Highest Sales](#5-small-business-customer-with-highest-sales)  
    3.6. [Corporate Customer with Most Orders (2009–2012)](#6-corporate-customer-with-most-orders-2009–2012)  
    3.7. [Customers Who Returned Items & Their Segment](#7-customers-who-returned-items--their-segment)  
     4. [Result Image Attach](#Result)  
   5. [Contributing](#contributing)

This project presents a comprehensive analysis of Kultra's inventory and sales data using SQL. 
The analysis answers key business questions related to sales performance, customer behavior, and product segmentation.

## Dataset Overview

* This analysis assumes data is available in a relational database with tables such as
( `sales`, `products`, `customers`, `orders`, and `returns`.) 

### Example Tables:
- `products(product_id, name, category, sub_category)`
- `customers(customer_id, name, segment, business_type, region)`
- `orders(order_id, customer_id, order_date, region, status)`
- `order_details(order_id, product_id, quantity, price)`
- `returns(order_id, return_date)`

### Image Attach Result Image Attach

![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/c869092e2d78794604ccf2c677b6a7136486f014/Average%20profit.png)

![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/6d6e0934b91bca0b958bb9ca0d6a58cb8e7a7706/Count.png)

## Analysis Questions & SQL Queries

```sql
SELECT 
   Select * from [dbo].[KMS Sql Case Study2]

Update table [dbo].[KMS Sql Case Study2]
### 1. ---- correcting the data type---
Alter table [dbo].[KMS Sql Case Study2]
Alter column Sales decimal (18, 2)

Alter table [dbo].[KMS Sql Case Study2]
Alter column Discount decimal (18, 2)

Alter table [dbo].[KMS Sql Case Study2]
Alter column Product_Base_Margin decimal (18, 2)

Alter table [dbo].[KMS Sql Case Study2]
Alter column Product_Base_Margin decimal (18, 3)

Select * from [dbo].[KMS Sql Case Study2]

 
 -----count distinct-----
Select Customer_Segment, count(distinct Customer_Segment) as [Total Customer segment]
from [dbo].[KMS Sql Case Study2]
group by Customer_Segment
Order by [Total Customer Segment] desc
------ count----
Select Customer_Segment, count( Customer_Segment) as [Total Customer segment]
from [dbo].[KMS Sql Case Study2]
group by Customer_Segment
Order by [Total Customer Segment] desc

Select Customer_Segment, count( Customer_Segment) as [Total Customer segment]
from [dbo].[KMS Sql Case Study2]
group by Customer_Segment
Order by [Total Customer Segment] Asc
###  Product Category with Highest Sales
-----Top product category----
SELECT TOP 3 Product_Category, Customer_Segment, Sales  AS highest_Product
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category

SELECT TOP 3 Product_Category AS highest_Product
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category DESC

SELECT TOP 3 Product_Category,Customer_Segment, Sales  AS highest_Product
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category Asc;

 ### ----highest Top 3 Region in term of Sales---
SELECT Top 3 Region, Sales  AS highest_Sales
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category Asc

###  ----Bottom 3 region 
SELECT Top 3 Region, Sales  AS Lowest_Sales
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT Min(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category Asc

### ----Top 3 region in term of Product Category
SELECT TOP 3 Product_Category, Region, Sales  AS highest_Product
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category Desc

SELECT TOP 3 Product_Category, Region, Sales  AS highest_Product
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category Asc

###  ----highest Top 3 Product Category in term of Customer Segment and Sales---
SELECT top 3 Product_Category, Customer_Segment, Sales  AS highest_Sales
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category asc

###  -------Maximum product by Region, Profit and Sales
SELECT TOP 3 Product_Category, Region, Profit, Sales 
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category Asc

SELECT TOP 3 Product_Category, Region, Profit, Sales 
FROM [dbo].[KMS Sql Case Study2]
WHERE Product_Category = (SELECT MAX(Product_Category) 
FROM [dbo].[KMS Sql Case Study2])
ORDER BY Product_Category Asc

Select * from [dbo].[KMS Sql Case Study2]

### -----Total Sales by Region----
Select Region, sum(Sales) as [Total Sales]
from [dbo].[KMS Sql Case Study2]
group by Region
order by [Total sales] desc
Select * from [dbo].[KMS Sql Case Study2] 


### ---Total Sales by Ontario--

Select Region, sum(Sales) as [Total Sales]
from [dbo].[KMS Sql Case Study2]
Where Region = 'Ontario'
group by Region
order by [Total sales] 

Select * from [dbo].[KMS Sql Case Study]
### ----Total Profit----
Select Ship_Mode , Sum(Profit) as [Total Profit]
from [dbo].[KMS Sql Case Study2]
group by Ship_Mode
order by [Total Profit] Asc


### ----- Average Profit--
Select Ship_Mode , AVG(Profit) as [Average Profit]
from [dbo].[KMS Sql Case Study2]
group by Ship_Mode
order by [Average Profit] desc

### -----Most shipping cost--

select Ship_Mode, count(Shipping_Cost) as [Most shipping cost]
from [dbo].[KMS Sql Case Study2]
group by Ship_Mode
order by Ship_Mode desc

select Ship_Mode, count(Shipping_Cost) as [Most shipping cost]
from [dbo].[KMS Sql Case Study2]
group by Ship_Mode
order by Ship_Mode Asc

Select * from [dbo].[KMS Sql Case Study2]

### -----Most Valuable Customers

Select Product_Category, count(Customer_Segment) as [Most Valuable Customer]
from [dbo].[KMS Sql Case Study2]
group by Product_Category
Order by [Most Valuable Customer] desc

Select * from [dbo].[KMS Sql Case Study2]

Select Product_Category, MAX(Customer_Segment)
AS [Most Valuable Customer],count(Customer_Segment) As[Total Customers]
from [dbo].[KMS Sql Case Study2]
group by Product_Category

Select * from [dbo].[KMS Sql Case Study2]

###  ----Small business customer with highest sales
Select  Product_Category, MAX(Sales) As [MaxSales]
from [dbo].[KMS Sql Case Study2]
Where Customer_Segment = 'Small Business'
group by Product_Category

Select * from [dbo].[KMS Sql Case Study2]


----maximum order quantity corporate business between year 2009 and 2012

SELECT Product_Category, MAX(Order_Quantity) AS [Maximum Order Quantity]
FROM [dbo].[KMS Sql Case Study2]
WHERE Customer_Segment = 'Corporate'
  AND YEAR(Order_Date) BETWEEN 2009 AND 2012
group by Product_Category

Select * from [dbo].[KMS Sql Case Study2]

### ----- Total profit WHERE Customer Segment = 'Consumer'
SELECT Product_Category, Sum(Profit) AS [Total Profit]
FROM [dbo].[KMS Sql Case Study2]
WHERE Customer_Segment = 'Consumer'
group by Product_Category

### ----- Total profit WHERE Customer Segment = 'Small Business'
SELECT Product_Category, Sum(Profit) AS [Total Profit]
FROM [dbo].[KMS Sql Case Study2]
WHERE Customer_Segment = 'Small Business'
group by Product_Category

### ----- Total profit WHERE Customer Segment = 'Corporate'
SELECT Product_Category, Sum(Profit) AS [Total Profit]
FROM [dbo].[KMS Sql Case Study2]
WHERE Customer_Segment = 'Corporate'
group by Product_Category

### ------Profit WHERE consumer is more profitable'
SELECT Top 1 Product_Category, Max(Profit) AS [Maximum Profit]
FROM [dbo].[KMS Sql Case Study2]
WHERE Customer_Segment = 'Consumer'
group by Product_Category

Select * from  [dbo].[KMS Sql Case Study2]

### -----Small business customer with highest Sales---
SELECT Top 1 Product_Category, Max(Sales) AS [Maximum Sales]
FROM [dbo].[KMS Sql Case Study2]
WHERE Customer_Segment = 'Small business'
group by Product_Category

### ----- Corporate Customer that placed the most number of orders in 2009 – 2012---

SELECT Product_Category, YEAR(Order_Date) AS Order_Year,
  MAX(Order_Quantity) AS [Maximum Order Quantity]
FROM [dbo].[KMS Sql Case Study2]
WHERE Customer_Segment = 'Corporate'
  AND YEAR(Order_Date) BETWEEN 2009 AND 2012
GROUP BY Product_Category, YEAR(Order_Date)
ORDER BY Product_Category, Order_Year;

	
Select * From [dbo].[Order_Status]

### ----- Total Status-----
Select Status,
count(Status) AS Status_Count
 From [dbo].[Order_Status]
 GROUP BY Status
Order by Status;

### ------- Total Status by Order ID-----
Select Order_ID,
count(Status) AS Status_Count
 From [dbo].[Order_Status]
 GROUP BY Order_ID
Order by Order_ID Asc


### ---Join Main table with order status---
SELECT 
    os.Order_ID,
    os.Status,
    o.Customer_Name,
    o.Order_Date,
    o.Sales,
	o.Product_Category,
	o.Customer_Segment,
	o.Region
FROM 
    [dbo].[Order_Status] AS os
JOIN 
    [dbo].[KMS Sql Case Study2] AS o
    ON os.Order_ID = o.Order_ID
ORDER BY 
    os.Order_ID;

### -----Customer that returned items, Segment-----
SELECT 
    o.Customer_Segment,
    COUNT(o.Order_ID) AS Returned_Orders
FROM 
    [dbo].[KMS Sql Case Study2] AS o
JOIN 
    [dbo].[Order_Status] AS os
    ON o.Order_ID = os.Order_ID
WHERE 
    os.Status = 'Returned'
GROUP BY 
    o.Customer_Segment
ORDER BY 
    Returned_Orders DESC;
Select * from [dbo].[KMS Sql Case Study2]


    
