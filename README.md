# Pewlett-Hackard-Analysis
Resources Used
- Pyton 3.10
- PGadmin, PostgreSQL

## Overview of the analysis

The purpose of this analysis is to determine the amount of employees retiring from Pewlett Hackard based on their most recent job title as well as other employees who would be eligible for a mentorship program. By doing so, the company is then able to determine how many jobs will need to be filled when the eligable employees retire. 

## Results
- An entity relationship diagram was designed as an aid to joining the original 6 csv files into different tables to determine the eligible employees for retirement and mentorship. 
![ERD](https://github.com/rhiandoy/Pewlett-Hackard-Analysis/blob/da07a26be9a826fa41ee103df4c6a4889fa32945/Data/EmployeeDB.png)

### Retiring Employees
- Using this diagram as a reference, we joined the employee data into a table called "retirement titles" with information including:
  - employee number
  - first/last name
  - title
  - to/from date
  - birth date
 
- To get the head count of how many employees would be leaving each department, another table was created with just the count of employees per title. Based off of this data 72,458 employees are eligible to retire from Pewlett Hackard. 

![retiring titles](https://github.com/rhiandoy/Pewlett-Hackard-Analysis/blob/a25cca1217ee9282d089d918d14d312c5e3ab3a2/Data/retiring_titles.png)

### Mentorship Eligibility
- The second half of our analysis helped determine which employees would now be eligible for mentorship who were also born during the year 1965. For this table we also included the above bulleted columns used in the retirement titles table but used a smaller range of birth dates. 

![mentorship](https://github.com/rhiandoy/Pewlett-Hackard-Analysis/blob/a25cca1217ee9282d089d918d14d312c5e3ab3a2/Data/mentorship.png)

## Summary
Based on our findings in the retirement analysis, there are 72,458 roles needing to be filled during the "silver tsunami". This is assuming that every employee that is eligible for retirement will retire sooner rather than later. According to the csv file exported containing all employees elibible for mentorship, there are 1,549 employees that are qualified to move up in the company. I would suggest that based on the amount of retiring employees in higher up positions, they would be able to mentor the 1,549 employees. 
