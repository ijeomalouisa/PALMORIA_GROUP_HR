## PALMORIA_GROUP_MANUFACTURING COMPANY


###  PROJECT TOPIC: PALMORIA GROUP HR ANALYSIS
Amazon is a company that provides E-commerce sales. They deals with different kinds of accessories ranging from electronics, computer/accessories, car and motor bikes accessories, helath and personal care medical equipments, musical instrument, office products, toys and games etc. This project will allow me to generate insight that can guide the company on product improvement,marketing strategies and customer engagement.

### DATA SOURCE:
**Amazon Sales Data:** The primary dataset used for this analysis is the "Amazon_Case_Study.xlsx" file. The dataset contains information from each sales which includes;
* Product details: name, category, price, discount and ratings
* Customer engagement: user reviews, titles, an contents.

### TOOLS USED: 
- Microsoft Excel (https://www.microsoft.com), other tools I used to explore are;
- Excel Power query (for cleaning of the data)
- Calculated columns (for creating new metrics of KPIs)
- Pivot Charts ( for visualizing of the summarized data)
- Pivot tables (to analyze the data from different angles to identify trends and patterns so as to make informed decision)

###  EXPLORATORY DATA ANALYSIS (EDA):
An Exploratory Data (EDA) was deployed using Excel tools and relevant techniques to the context of each analysis. I will explore the Amazon sales data to answer these key questions. 

##### Task Question 1:

The analysis will be based on the use of Pivot tables and calculated columns where necessary to answer the following;
  1. Find the average discount percentages by Product category
  2. Check how many products that are listed under each category
  3. Calculate the total number of review per category
  4. show product that has the highest average ratings
  5. Acertain the average actual prices Vs the discounted prices by category
  6. To List the products that have the highest number of reveiws
  7. Find how  many products that have a discount of 50% or more
  8. To show the distribution of product ratings i.e. how many products that are rated 3.0, 4.0 etc
  9. calculate the total potential revenue of actual price * rating count by category
  10. Find out the number of unique products per price range bucket e.g. <200, <200-500, >500
  11. To show how the rating relates to the level of discount
  12. Check how many products have fewer than 1,000 reviews
  13. Find out which categories have product with the highest discounts
  14. To identify the top 5 products in terms of rating and number of reviews combined
  
#### Task Question 2: Dashboard Creation
I will use the clean dataset with the pivot outputs and build an Excel dashboard to unleash beautiful creativity

### DATA CLEANING/PREPARATION (EXCEL)
In view of the preparation task concerning this product, I performed the followings: we have 2 options for the cleaning. We can go by writing functions/formular or use Excel power query, I choosed Power query instead. 
1. To "DATA" menu, "from get and transform data", click the table/range,
2. The data was loaded to the Excel power querry,
3. I viewed it to see the column quality, going through it, I observed that there was "NULL" and "ERROR" in the rating count. as far as am concerned the data is dirty.
4. I shortened the "category" aspect of the dataset to make it look good, if not, in the course of the analysis it may be too long.
5. Highlight and Right click on the category to choose split column by delimiter i.e. "left most delimiter", Ok, it splited it into two, in the computer and accessories writing together
7. Right click again to replace values i.e value to find "&" then replace with "space" (it will be divided into two)
8. HomeImprovement, MusicalIstrument and OfficeProduct are still together and they are the three arguments I added space
9. I Go to add column, "Conditional column", HomeImprovement, category 1, then HomeImprovement writing in space e.g. replace Home Improvement
10. add clause to repeat the remaining two i.e. MusicalInstrument and OfficeProduct, Else Category 1
11. In the product name, count the number of character, I counted and stoped at 25 character including the spaces,
12. split the column again BUT not by delimiter, Split by number of character "once as far left as posible"
13. add the 25 and check on "once as far left as possible
14. Right Click and remove the splited right column
15. change the data types
16. I removed columns that are not needed. i.e. the img link, user-name, review content and product link etc because they are not necessary.
17. Close and Load my query.
