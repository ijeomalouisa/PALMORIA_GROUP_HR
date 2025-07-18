## PALMORIA_GROUP_MANUFACTURING COMPANY


###  PROJECT TOPIC: PALMORIA GROUP HR ANALYSIS
The analysis is focused on issues bordering on gender inequality in the Palmoria Group HR manufacturing company and at its three (3) regions.

### PROJECT OVERVIEW
Palmoria Group is a manufacturing company based in Nigeria. The company is faced with the issues bordering on gender inequality in its three (3) regions within the country. Based on their ambitions to scale the business to other regions and even overseas, if the problems are not tackled, it can spriral downwards thereby jeopardize the company's image. To address the issues before they get out of hand, an HR Analyts needs to come in to identify key areas within the business that could give rise to issues, address them immediately and come up with recommendations for Management attention.


### SOURCE OF DATA:
The primary dataset to be used for this analysis is the "Palmoria Group Bonus Rules.xlsx" and the "Palmoria Group Emploment.CSV file. The dataset contains information such as; Staff name, gender, department, salary, location and ratings.

### TOOLS USED: 
- Power BI tool (https://www.microsoft.com), will be use to explore 
- Power BI query (for cleaning of the data)
- Analysis Dashboard (for Deep-Dive Metrics and Tables)
- Visualization Dashboard ( for excuting summary and high-level charts)

###  EXPLORATORY DATA ANALYSIS (EDA):
A comprehensive Exploratory Data Analysis (EDA) was deployed using appropriate analytical tools and techniques relevant to the context of each dataset; the Palmoria Group bonus Rules from Excel and the Palmoria Group Employment.Comma Seperated Values (csv) data are used to answer the key questions. 

##### CASE SCENARIO:
The analysis will be based on the use of Power BI to answer the following case scenario and pointers from Mr.Gamma:
To analyze the company data and generate insights that the Palmoria management team would need to address and the analysis is to be visualized using appropriate charts. Focuse should be on gender related issues within the organization and its regions, Insight required  from the Analyst are based on discretion. Generally, there are two genders in the organization but some employees refused to disclose their gender, so, a generic gender status is required. Some staff are without a salary, reason been that they are no longer with the company, they need to be out. lastly, some departments are indicated as "NULL" the departments also need to be taken out.

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
 
  ### DATA WRANGLING/PREPARATION (POWER BI)
In view of the preparation task concerning the above case scnario and pointers from Mr. Gamma, the analyst used the Power BI query to get the overall structure thus:
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



#### Step-by-Step Data Cleaning of Palmoria Group emp.csv

* From "HOME" Bar "GET DATA", "Text/CSV", select "Palmoria Group emp.csv"
* Transform the data to load into power query (wrangling)
* Remove the "NULL" as instructed in the case scenario (Click of the "Department" drop down arrow and uncheck the null)
* Go to "Salary" column and uncheck the NULL
* Go to "Gender" column, right click and replace values (value to find "BlanK", replace with "Unknown") then click OK
* Go to "HOME" Click on "Merge queries": click on department and click on the Bonus department too, Press and hold down Ctrl. key, then click on "Rating" in the emp., click on "Bonus" rating too Then OK.
* Go to Bonus column, click on teh arrow opposite each other to uncheck "select all columns", then select and check on bonus, right click on the Bonus to replace values
* Replace value (value to find "NULL" replaced with "0", then check the data type to percentage
* to to "ADD COLUMN" bar (Custom Column), name it BONUS, = clcik on Salary * Bonus Rules, OK
* Go to Add column again, Rename as "New Salary" = Salary + Bonus then OK
* Go to "VIEW" to check the coloumn quality
* Go to bonus rule.bonus column (right click), replace values (NOTE: do not make mistake of writing capital letter because it is case sensitive),  value to find "null", replaced with "0"
* Change the data type to percentage(%)
* Highlight the BONUS and NEW SALARY at the same time, change the data type to "Whole Number"
* Add a "CONDITIONAL COLUMN" from the Add column bar and name as "SALARY BAND" (to know how many employees fall into a band,) and do the calculation thus;
  1. If salary, is less than or equal to 1000, THEN 0-10,000, ADD CLAUSE...
  2. If salary, is less than or equal to 20000, THEN 10001-20000, ADD CLAUSE
  3. If salary, is less than or equal to 30000, THEN 20001-30000, ADD CLAUSE
  4. If salary, is less than or equal to 40000, THEN 30001-40000, ADD CLAUSE
  5. If salary, is less than or equal to 50000, THEN 40001-50000, ADD CLAUSE
  6. If salary, is less than or equal to 60000, THEN 50001-60000, ADD CLAUSE
  7. If salary, is less than or equal to 70000, THEN 60001-70000, ADD CLAUSE
  8. If salary, is less than or equal to 80000, THEN 70001-80000, ADD CLAUSE
  9. If salary, is less than or equal to 90000, THEN 80001-90000, ELSE
  10. 100 001 & Above

Below is the Power BI query of the Employee's data wrangling and the steps.....






<img width="904" alt="Palmoria Employee Query" src="https://github.com/user-attachments/assets/4cd5179b-c52a-4d47-a97d-a7788f8436da" />




This is the concluding part of the "BONUS RULES" and "EMPLOYEE" data wrangling as shown in the two power query tables above.



### VIZUALIZATION DASHBOARD

#### Pointer 1: Gender Distribution in the Organization
In this overall distribution across genders, location and department, A total of 946 employees are working under the company. The male are 465 (49.15%) of the count, female 441 (46.62%) while the unknown genders are 40 (4.23%). This shows that the company tend to employ male than female counterpart as evidenced in the visual below:


<img width="466" alt="Overall Gender Distribution in Palmoria HR1" src="https://github.com/user-attachments/assets/dea7334e-9bff-4a56-bbfc-b407c57e3e8f" />



The visual simply shows that male gender dominates the other genders  


#### Pointer 2: Show Insights on Ratings Based on Gender


<img width="235" alt="Insights on Ratings based on Gender " src="https://github.com/user-attachments/assets/fce49381-61e7-4551-8daf-934915533cc6" />


The above insight indicates how employee rating varies across gender. Male has the average rating of 212, female 190 while unknown has 18. More female employee are rated "Good" and "Very Good" as identify in the matrix than male. Some male are rated "Very Poor".  


#### Pointer 3: Analyze Salary and Identify Gender Pay Gap

In this, the overall salary structure will be showcased; to detect the gender-based salary disparities and highlight departments and regions needing management focus.





<img width="419" alt="Salary Structure and Gender Pay Gap" src="https://github.com/user-attachments/assets/3b1783b4-cb07-408d-960e-b6734791f8fb" />








The overall salary pay gap per gender shows that unknown gender has the highest average as evidenced in the 78367.50 followed by the male gender with 74789.53 and female having the lowest average of 72135.69. Lagos has the highest average pay as indicated in the gender pay per location as unknow genders has 86860.00, male 76680.65 and female 74163.47. looking at the average salary pay gap by gender per department, unknown genders earn more in the Marketing and Accounting department but receive less average pay in the Business Development and product Management as shown in the 49956.67and 36480.00 respectively.



#### Compliance & Pay Distribution Analysis:

The aim here is to check if company complies with the $90,000 minimum salary for Manufacturing employees as well, know the overall salary distribution in $10,000 Bands.





<img width="304" height="260" alt="SALARY BAND BY LOCATION2" src="https://github.com/user-attachments/assets/b9cbd119-e7b4-45f8-9648-52144fa3944c" />

DISTRIBUTION OF SALARY BAND PER LOCATION



<img width="455" height="221" alt="SALARY BAND PER DEPARTMENT" src="https://github.com/user-attachments/assets/752580ec-4746-4d36-94f5-1d495b58026f" />

DISTRIBUTION OF SALARY BAND PER DEPARTMENT

In the list of manufacturing employees <$90000 above, 202 workers falls into salary band of 100000 & above distribution across the organization, 90 employees falls into 90001-100000, 28 workers falls into 20001-30000 and 101 employees into the band of 30001-40001.
Legal department is the highest in the distribution across the department with the salary  band of 20001-30001 with the total of of seven(7) employees. Training Department with the 13 employees in the salary band of 90001-100000 and 50001-60000 respectively with the count of 16 employees. Production Management earn highest in 60001-70001 as well as in 100000 and above. Kaduna has the highest salary band in the salary distribution across Region.


#### Pointer 5: Bonus Allocation Using Bonus Rules 

BONUS CALCULATIONS: This calculation is achieved using conditional columns thus
* Unpivot and merge Bonus Rules and Employee Table
* Calculate Bonus Amount = Salary * Bonus %
* Calculate Totapy Pay = Salary + Bonus

FIND BELOW THE EXECUTIONS:

<img width="599" height="347" alt="BONUS ALLOCATION USING BONUS RULES " src="https://github.com/user-attachments/assets/1fdb96e6-4f71-4295-941b-fed4feb8443f" />


TOTAL BONUS AND PAY BY REGION AND DEPARTMENT



<img width="212" height="141" alt="TOTAL BONUS AND PAY BY REGION AND DEPARTMENT" src="https://github.com/user-attachments/assets/8e990759-e26e-48af-bdb7-49b273d33cf8" />


### FINDINGS 
* Palmora Group has a nearly even male-to-female workforce,
* Unknown genders has the highest average salary pay
* Kaduna is the highest salary band distribution across the region
* Lagos has the highest salary concentration, management should focused on that region
* Business Development leads the pack.
* Many employees are rated as "Good", but a notable portion are “Not Rated” — this may require HR intervention.
* Salaries between genders are relatively balanced but could benefit from further drill-down by role.

### CONCLUSION
Polmoria Group of Company has male to female workforce of 946, there is no disparity because some workers did not disclose their gender, relatively, some employees earn salary greater than of equal to $90,000 and above taking cognizance of the the salary band. A good number of workers are rated "Good" while few "Not Rated". The company needs to review Abuja location to know what is not working in that area. More female employee should be deployed in the company. Finaly, The company meet the requirement of the 90,000 salary distribution 




