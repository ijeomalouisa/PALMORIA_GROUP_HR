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
A comprehensive Exploratory Data Analysis (EDA) was deployed using appropriate analytical tools and techniques relevant to the context of each dataset; the Palmoria Group bonus Rules from Excel and the Palmoria Group Employment.Comma Seperated Values (csv) data are used to answer these key questions. 

##### CASE SCENARIO:
The analysis will be based on the use of Power BI to answer the following case scenario and pointers from Mr.Gamma:
To analyze the company data and generate insights that the Palmoria management team would need to address and the analysis is to be visualized using appropriate charts. Focuse should be on gender related issues within the organization and its regions, Insight required  from the Analyst are based on discretion. Generally, there are two genders in the organization but some employees refused to disclose their gender, so, a generic gender status is required. Some staff are without a salary reason is that they are no longer with the company, they need to be out. lastly, some departments are indicated as "NULL" the departments also need to be taken out.

#### CASE QUESTIONS: POINTERS FROM MR. GAMMA

1. What is the gender distribution in the organization? distil to regions and departments.
2. Show insights on ratings based on gender.
3. Analyze the company's alary structure. Tdentify if there is a gender pay gap. If there is, Identify the department and regions that should be the focus of management.
4. A recent regulation was adopted which reuires manufacturing companies to pay employees a minimum of $90,000. Does Palmoria meet this requirement? (b) Show the pay distribution of employees grouped by a band of $10,000-$20,000, $20,000 - $30,000 etc (c) also visualize this by regions.
5. Allocate the annual bonus pay to employees based on the performance rating.
6. Use the Bonus Payment Rules to:
   a). Calculate the amount to be paid as a bonus to individual employees
   b). Calculate teh total amount to be paid to individual employees (salary inclusive of Bonus)
   c). Total amount to be paid out per region and company wide.
 
  ### DATA WRANGLING/PREPARATION (EXCEL)
In view of the preparation task concerning the above case scnario and pointers from Mr. Gamma, I used  the Power BI, to get the overall structure thus:
* Analysis Dashboard (for Deep-Drive Metrics & Tables)
* Visualization Dashboard (for Executive summary, High-level charts)

#### Step-by-Step Data Wrangling:
* Lunch the Power BI
* From "HOME" Bar "GET DATA", "Excel.xlsx", select "Palmoria Group Bonus Rules"
* Transform data to do the cleaning
* Unpivot the department column (choose unpivot other columns)
* Change the column to (a) Rating (b) Bonus %.
* Change Data type for Bonus to percentage. Done

Below is the Power BI query of the Bonus Rule's data wrangling and the steps.....



<img width="785" alt="Palmoria Bonus Rules" src="https://github.com/user-attachments/assets/5405f794-0824-4abd-866c-669520749644" />



#### Step-by-Step Data Cleaning of Palmoria Groupemp.csv

* From "HOME" Bar "GET DATA", "Text/CSV", select "Palmoria Group emp.csv"
* Transform the data to load into power query (wrangling
* 

Below is the Power BI query of the Bonus Rule's data wrangling and the steps.....



