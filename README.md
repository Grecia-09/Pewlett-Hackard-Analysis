# Pewlett-Hackard-Analysis

## Overview of the analysis
An HR Analysit asked me to help him build an employee database with SQL by applying data modelling, engineering, and analysis skills for future-proofing the company by determining how many people will be retiring and, of those employees, who is eligible for a retirement package.
We had two specific assignments: 
- Determine the number of retiring employees per title.
- Identify employees who are eligible to participate in a mentorship program. 

## Results
Here are four major points from the two analysis deliverables:

- Taking in consideration all the titles of current employees who were born between January 1, 1952 and December 31, 1955, the number of retiring employees per title is 133,776.
- Some employees may have multiple titles in the database due to promotions throughout the life in the company, we eliminated duplicate rows from the result and now the number of retiring employees per title decreased to 90,398.
- The most recent job title with the highest number of employees who are about to retire is Senior Engineer. See image below for reference:

<img width="275" alt="Screen Shot 2020-11-01 at 2 24 45 PM" src="https://user-images.githubusercontent.com/70611325/97816937-0d3c1400-1c4e-11eb-9e18-af6d012651e2.png">

- After created a mentorship-eligibility table we obtained that 1,549 current employees are eligible to participate in the program.

## Summary 

***How many roles will need to be filled as the "silver tsunami" begins to make an impact?***

To retreive the total number of employees ready for retirement I used the following query:

SELECT COUNT(ri.emp_no)
FROM retirement_info as ri;

It seems that the roles that will need to be fill are a total number of 41,380.


***Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?***

The current employees eligible to participate in the program are 1,549. I've created a table where it shows the number of these employees by their current title:

<img width="274" alt="Screen Shot 2020-11-01 at 3 04 29 PM" src="https://user-images.githubusercontent.com/70611325/97817855-d7019300-1c53-11eb-8a4e-dcbfc2e92111.png">








