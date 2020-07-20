# Pewlett_Hackard_Analysis
First step was to download the excel files from Pewlett Hackard and creat and ERB showing the relationships between the databases. 
Here is the code for the ERB:
Departments
-
dept_no varchar pk
dept_name varchar

Employees
-
emp_no pk int
birth_date date
first_name varchar
last_name varchar
gender varchar
hire_date date

Salaries
-
emp_no int pk fk - Employees.emp_no
salary int
from_date
to_date date

Managers
-
dept_no varchar pk fk >- Departments.dept_no
emp_no int fk - Employees.emp_no
from_date date
to_date date

Dept_Emp
-
dept_no varchar pk fk >- Departments.dept_no
emp_no int pk fk >- Employees.emp_no
from_date
to_date

Titles
-
emp_no int pk fk >- Employees.emp_no
title
from_date
to_date

Here is the image:
