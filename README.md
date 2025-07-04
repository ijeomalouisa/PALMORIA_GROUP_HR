## PALMORIA_GROUP_MANUFACTURING COMPANY


###  PROJECT TOPIC: PALMORIA GROUP HR ANALYSIS
The analysis is to look for the issues bordering on gender inequality of the Palmoria Group HR manufacturing company in its three (3) regions, the company is based in Nigeria and an HR analytics experts is needed to analyze the company's data and come up with recommendations for Management attention.

### PROJECT OVERVIEW
Palmoria Group is a manufacturing company based in Nigeria. The company is faced with the issues bordering on gender inequality in its three (3) regions with the country. Based on their ambitions to scale the business to other regions and even overseas, if the problems are not tackled, it can spriral downwards thereby jeopardize the company's image. To address the issues before they get out of hand, an HR Analyts needs to come in to identify key areas within the business that could give rise to issues and address them immediately.

### SOURCE OF DATA:
The primary dataset to be used for this analysis is the "Palmoria Group Bonus Rules.xlsx" and the "Palmoria Group Emploment.CSV file. The dataset contains information such as; Staff name, gender, department, salary, location and ratings.

### TOOLS USED: 
- Power BI tool (https://www.microsoft.com), will be use to explore, overall structure is 
- Power BI query (for cleaning of the data)
- Analysis Dashboard (for Deep-Dive Metrics and Tables)
- Visualization Dashboard ( for excuting summary and high-level charts)

###  EXPLORATORY DATA ANALYSIS (EDA):
A comprehensive Exploratory Data Analysis (EDA) was deployed using appropriate analytical tools and techniques relevant to the context of each dataset; the Palmoria Group bonus Rules from Excel and the Palmoria Group Employment.Comma Seperated Values data are used to answer these key questions. 

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
