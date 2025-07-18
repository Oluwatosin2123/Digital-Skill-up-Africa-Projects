# Digital-Skill-up-Africa-Projects
## Amazon Product Data Analysis – Excel Project 
## Table of Contents
- [Project Overview](#project-overview)
- [Tools Used](#tools-used)
- [Step 1: Data Cleaning](#step-1-data-cleaning)
- [Step 2: Data Analysis](#step-2-data-analysis)
- .[Step 3: Dashboard Creation](#step-3-dashboard-creation)
- [Insights Derived](#insights-derived)
  
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

    ### Products Price Overview and Total Reviews.
 ![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/98f056f15b6c504c8c2d6bcd58c6a84a327687bf/Product%20Price%20overview.png)


### Products Category and Customer Segment.
![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/080b7d104dabd55e0f415744f5c3d4a192a402af/Customer%20segment%20by%20Category.png)

### Pivot Tables
 ![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/09d425a2d164963fc21220094533f8bbe464fb51/PivotTables.png)

![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/3cabe0384eb7a5afbeebff328271d8e5625b671a/Pivot%20Tables.png)

 ## Step 3: Dashboard Creation
 ### Designed an interactive and visually appealing Excel dashboard
 Added:
 
  * Charts (bar, pie, line) for key insights
  * Shapes and icons for structure and emphasis
  * Images (e.g., products or Amazon logo)
  * Color fills and consistent theme for a clean layout
  * Slicer style settings
  * Inserting Pictures, and other visualization format.

       
![image alt](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/41d79bab4a859701f7b8e8be3b58fcec167f6b15/Amazon%20Dasboard%20by%20Oluwatosin%20Moses%20Adebayo.png)
 
 ### Using the logical/conditional functions
    =IF(Discounted price < 200%, " Low", IF (Discounted price <5000, " Meduim", IF (Discounted price <10000, "High", "Very High" )))
    =Countif(Rating, Criteria)
    =Sum(Values)
    =Average(sum(values))
    
    ### Pivot Field list and other formats.
    * Selecting the Row, values, Columns and filter.
    * Sumarization.
    * Sorting Values ( Ascending or descending Order)
    * Number and Label filter.
    * Format Cell : changing currency types from Dollars to English(India) Rupee.
    * Value field settings for changing Data type.
    
 ## Insights Derived
 * Top-performing product categories
 * Price vs. Rating correlation
 * Products with highest discounts
 * Average customer satisfaction metrics

### Files in this Repository 
*  -  Excel Analysis [Download Here](https://github.com/Oluwatosin2123/Digital-Skill-up-Africa-Projects/blob/616daf6a059474c6bb0ef5f0c07944989087acd0/Amazon%20project%20Cases%20Study%20One.xlsx)

## Oluwatosin Moses Adebayo


