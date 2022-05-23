# Pewlett Hackard Analysis

## Overview
In this project, we helped Bobby, a Human Resources Analyst who works in Pewlett Hackard and need to answer the next questions: Who will be retiring in the next few years in the company?, and how many positions will Pewlett Hackard, need to fill?

Our **purpose** was to perform a database analysis for Pewlett Hackard with PostgreSQL and create a list of employees who are going to retire from their jobs shortly. The company also asks Bobby and us to develop a retirement package and prepare a mentorship program.

It's important to note Pewlett Hackards is a large company that is been around for a long time and because of it had a lot of future retirees from all departments.

To conduct this task, our **resources** were: six CSV files and PostgreSQL, pgAdmin, and QuickDBD.

## Results

The following image shows an Entity Relationship Diagrama that we used to understand and visualize the structure of our six CSV files. We made it to understand the analysis.

![Alt text](/Resources/EmployeeDB.png "imagen1") 

The table called "Retiring employees" has information of employee number, first_name, last_name, title, from_date, and to_date. This query results in 133,776 employees retiring soon.

![Alt text](/Resources/1_retirement.png "imagen2") 

However, in that table has not been removed the duplicate data, so in the following query, we corrected the "retiring employees" table, which shows that 90,398 employees meet the criteria for retiring soon.

![Alt text](/Resources/1_uniquetitles.png "imagen3") 

In the following table, we presented the number of employees due to retire according to their title:

![Alt text](/Resources/1_retiring_titles.png "imagen4") 

We can conclude that the positions where most employees are going to retire are Senior Engineer and Senior Staff.

Finally, the following table shows the employees eligible for the mentorship program. In this case, the query returns 1,548 rows and looks like this:

![Alt text](/Resources/mentonship.png "imagen5") 

## Summary

**How many roles will need to be filled as the "silver tsunami" begins to make an impact?** As we have seen in the respective table, a total of 90,398 employees are eligible to retire shortly. We can deduce that the **silver tsunami** represents a challenge for the company due to the large number of employees who are about to retire from their positions. According to our analysis, of 300,024 employees in the company, 90,398 are about to retire, which represents 30.13% of the total number of workers in the company. Also, the positions that are going to be vacated the most are Senior Staff and Senior Engineer.

**Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?** 
Regarding the Mentorship Program, the employees eligible to participate are only 1,549 workers, so, we can conclude that the number of candidates for the Mentorship Program is insufficient.
As we can see, there is a considerable representation of expected retirees in almost all departments, but there are about 59 apprentices for every mentor, which means that there will be a shortage of qualified mentors. A suggestion would be to study the skills that each mentor requires according to the department, in order to calculate how many people the mentor can help.

**Suggested tables**
We recommended to study not only the titles but also the departments separately for better organization, as shown in the following table:

###### Unique titles by Department
![Alt text](/Resources/title_and_depto.png "imagen6") 

Finally, we suggested to create a new query that counts the number of roles or positions per department.

###### Position to fill per deparment
![Alt text](/Resources/roles.png "imagen7")
