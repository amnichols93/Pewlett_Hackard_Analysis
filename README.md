# Pewlett Hackard Analysis

Pewlett Hackard provided several datasets so we could execute different analyses and determine the number of employees who will likely be retiring soon and which departments will be losing staff and/or managers. Additionally, after the initialy analysis was performed, the company requested a list of people who qualified for a mentorship program based on their date of birth. I was provided data on current departments and employees, including hiring dates, retirement/termination dates, salaries, and job titles, via six .csv files.

To provide Pewlett Hackard with the analysis they were looking for, I built a Postgres database and used SQL to analyze the .csv files. Before performing any analysis, I built an ERD (see below) to represent the relationships between the data in the individual datasets. Once the ERD was saved, I used SQL to physically establish the relationships that I had mapped out in the ERD. I used prompts like CREATE TABLE, FOREIGN KEY / REFERENCES, and PRIMARY KEY to load the given .csv files into their databases and connect them. Once the given .csv files were loaded, I used the SELECT / INTO commands to parce out the pertinent information for new databases that provided deeper analysis based on the information Pewlett Hackard needed. 

![ERD](EmployeeDB.png)

Figure: ERD


The analysis indicates that the following number of employees will likely retire soon from each department: 2,199 from Marketing; 1,908 from Finance; 1,953 from Human Resources; 8,174 from Production; 9,281 from Development; 2,234 from Quality Management; 5,860 from Sales; 2,413 from Research; and 2,597 from Customer Service. A little over 1500 employees qualify for the mentorship program. The limitations I found in performing this analysis were solely related to my proficiency with SQL. Everything the company asked of me was possible, so long as I knew the commands to perform the analysis. If the company had asked for the comprehensive analysis of upcoming retirees and mentees, then it would have been much more helpful if the company provided the exact criteria for which employees fall into those categories. For example, age may not be the only factor in determining when someone retires. If this were a public service profession, many employees retire after twenty years of service, regardless of age.
