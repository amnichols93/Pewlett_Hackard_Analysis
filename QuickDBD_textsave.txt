departments
-
dept_no varchar pk
dept_name varchar

employees
-
emp_no int pk
birth_date date
first_name varchar
last_name varchar
gender varchar
hire_date date

dept_emp
-
emp_no int pk fk -< employees.emp_no
dept_no varchar fk -< departments.dept_no
from_date date
to_date date

dept_manager
-
dept_no varchar pk fk -< departments.dept_no
emp_no int fk - employees.emp_no
from_date date
to_date date

salaries
-
emp_no int pk fk - employees.emp_no
salary int
from_date date
to_date date

titles
-
emp_no int pk fk -< employees.emp_no
title varchar
from_date date
to_date date