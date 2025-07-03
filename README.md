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
- [Author](#author)

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
  * Images (e.g., product or Amazon logo)
  * Color fills and consistent theme for a clean layout
 
 ## Insights Derived
 * Top-performing product categories
 * Price vs. Rating correlation
 * Products with highest discounts
 * Average customer satisfaction metrics
 


    
