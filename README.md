# Pewlett-Hackard-Analysis

## Overview of the analysis

The leadership of Pewlett Hackard wants to be prepared for the future and don't have any surprises in their upcoming retirement wave. Due to that reason the following analysis of the Pewlett Hackard employees structure was performed to give more insights about the following key questions. 

This analysis consists of two technical analysis deliverables and a written report. 

Deliverable 1: The Number of Retiring Employees by Title
Deliverable 2: The Employees Eligible for the Mentorship Program
Deliverable 3: A written report on the employee database analysis (README.md)


## Results

- Pewlett Hackard has a workforce of 300.024 employees 
- Depending on how we set the filters with birth_data and hire_date we get different numbers for Pewlett Hackard employees eligible for retirement. 
The table below shows the employees eligible for retirement sorted by titles. 


- A large percentage of this eligible for retirement employees are either senior or leadership level. That means Pewlett Hackard will loose a lot of knowledge in that retirement wave. 
- Especially in the 



- There are in total 1549 employees eligible for the mentorship program, which can help to buffer the retirement wave, but still there have to new hires and a knowledge transfer as soon as possible. 
- There are only 275 Senior Engineers and 77 Technique Leaders eligible for the mentorship program. 
- Out of 25916 Senior Engineers and 3603 Technique Leaders going in retirement this number is not sufficient enough to buffer the retirement wave with mentorship program. 


## Summary

### How many roles will need to be filled as the "silver tsunami" begins to make an impact?
- The numbers are varying depending on the filters and are between 41380 and 133.000 employees. 
- In the worst case filter scenario nearly half of the workforce is retiring of PH. 


### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

There are not enough employees eligible for the mentorship program to mentor the next generation of PH employees. As already mentioned in above the results PH has to start hiring as soon as possible. 

Query for Count of mentors by title. 

SELECT COUNT(mt.title),
		mt.title
FROM mentorship_eligibility as mt
GROUP BY mt.title
ORDER BY mt.count DESC;


