## HR DATA ANALYSIS with EXCEL

### OVERVIEW
---

HR datasets consist of information related to various aspects of workforce within an organisation.

For the purpose of this project, the type of HR data used focused on employees demographic and job information in an organisation. Microsoft Excel was the tool used to carry out this task and using Pivot Table feature for exploratory data analysis. 


### PROCESS
---

The HR dataset used for this project is gotten from data.world, it is available via this [link](https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Human+Resources.csv). It has total of 22214 rows and 13 columns. It was downloaded in a .csv format.

The dataset was loaded into Excel sheet as seen below:

![1](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/50d3770b-2b36-4349-8aa2-ad63400c61bc)

Checking the dataset, it needs claning. Inconsistencies, blanks, wrong datatypes were noticed. Starting with, the ‘birth_date’, ‘hire_date’ and ‘termdate’ columns were changed to Date datatypes, the ‘termdate’ column has blanks in it cells which were replaced with ‘unknown’ using the ‘Go to special’ feature in the Find & Select tab to fill the blanks.

For the adequate result of the analysis, four additional columns were created as follows:

* Full name

![4](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/50a039fc-0716-4039-8663-a635ab8d961d)

The CONCATENATE function used to combine the first_name and last_name together.


*	Tenure

![5](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/4e41b6da-13d9-4aa6-9426-9ca9d6f1ea50)

The YEARFRAC function used to calculate the years difference between the hire_date and termdate and using the IFERROR function to replace the blanks with ‘unknown’.


*	Age

![6](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/97e48874-c9ad-4e26-b405-e0d5a3f2bfd0)

Using the YEARFRAC function also to calculate the years difference between the birth_date and hire_date to get the age of each employee.


*	Age group

![7](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/3afc8297-7bf0-4072-a623-6b21b66b6495)

The IF function used as a conditional formula to create age range for the employees. Age group were classified into young, adult and old.

![3](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/2dca10c2-1ca2-4dae-ab3c-388d3e50a13a)


The dataset is now cleaned and good to go for analysis.

![2](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/3740260e-259e-4ef8-b45f-52e0cecd821c)


### ANALYSIS
---

The exploratory data analysis were segmented into five (5).

i.	Primary Analysis

ii.	Employee Analysis

iii.	Job Analysis

iv.	Department Analysis

v.	Location Analysis

#### Primary Analysis
This analysis to get the descriptive statistics of every employee i.e the frequency of employee demographics in the organization. These were as follows:

**1. Gender**

![8](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/8e90b880-d684-4386-a484-de00cd9a23ba)

There are 3 Gender types.


**2. Race**

![9](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/41d88209-b13d-48e0-abed-93eea1fef638)

There are 7 Races.


**3. Department**

![10](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/2d94b97a-0e74-4052-9327-f8d4e61b98e7)

There are 13 departments in the organisation.


**4. Job Title**

![11](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/660b5c68-85f0-4626-a656-2d30eccbb3c1)

There are 185 Job Titles in the organisation.


**5.	Work Location**

![12](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/bec757d2-c603-44d0-aaa3-fa33c6f892c9)

There are 2 types of work location.



### Employee Analysis

**1.	What is the distribution of employees gender, race, age group and work location in the organisation?**

![13](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/78f3f19b-d2b8-448a-aa47-946a66e8ccd6)

![14](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/d4542cc9-b2aa-4f78-a5e5-e5f319a01010)

![16](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/1a7b5ca1-9ae2-4971-bf7a-7d40e1331646)

![15](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/351ad36f-215e-4955-b6fa-4ba5825b9190)


**2.	What is the calculation of average age and average tenure of employees?**

![17](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/de8a3565-7d0e-4c9c-9e32-358cdd8e2f2a)

![18](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/4edca650-d40e-402c-b918-ee4f3c3d8bbc)


**3.	Identify the employees with the longest tenure in the organisation?**

![20](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/913c3224-16de-4db0-b428-acedc94b7695)

There are 3 employees with longest tenure in the organisation.


**4.	Identify the employees with the shortest tenure in the organisation?**

![21](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/45e64d24-2f3f-4ecf-a24b-0001784d646f)

Total of 18362 employees had shortest tenure with less than a year in the organisation.


**5.	What is the distribution of age group in the organisation by gender?**

![19](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/fb3847e7-9ea6-47a7-81f1-cea1c878592d)



### Job Analysis

**1.	Each job titles has how many employees?**

![22](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/9afd3339-3507-43ef-a17b-dc2982e947ee)


**2.	How is the distribution of gender in each job title?**

![23](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/8ddbae74-07c5-4d5d-b687-9c627cdbe510)



### Department Analysis

**1.	Identify the department with the highest and lowest number of employees.**

![26](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/af308243-0067-4fc5-a6c0-6a982465f67d)

Department of Engineering has the highest number of employees while Auditing department has the lowest.


**2.	What is the distribution of gender in each department?**

![27](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/f19c4fae-d08b-4830-9c27-24b483cfec65)


**3.	Analyze the average age and average tenure of employees from each departments.**

![28](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/45e54a08-6f65-40ba-bfa7-22f6e8f17f3a)



### Location Analysis

**1.	Determine which state has the highest number of employees.**

![24](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/81691fcc-7d97-4056-b640-206a32b73000)


**2.	Identify the number of employees from each city.**

![25](https://github.com/Dparagon/hr-data-analysis-with-excel/assets/128928568/d56a66d2-97cf-4647-aee7-ec17a9ccde11)

There are total of 77 cities with Cleveland city having the highest number of employees.


### CONCLUSION
---

Microsoft Excel provides powerful tools for data manipulation and analysis, including pivot table and other in-built functions to help you explore your data effectively.

**The Excel sheet can be seen via this link.**

https://4g56xz-my.sharepoint.com/:x:/g/personal/atollyguy_4g56xz_onmicrosoft_com/Ec3_hsbxoJVOo1LIEcgjBekBUy_QvzBfxHQsUqjEHe-eUg?e=3TZq65





