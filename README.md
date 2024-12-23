# sql-challenge
Module 9 Assignment

# Files in the repository and their functions
- In the data folder, there are CSV files that are the only remaining records of the employees, departments, and managers of a company called Pewlett Hackard.
    - <ins>departments.csv</ins> - contains department numbers and department names
    - <ins>dept_emp.ssv</ins> - cross references employee numbers and department numbers
    - <ins>dept_manager.csv</ins> - contains department numbers and department manager IDs
    - <ins>employees.csv</ins> - contains employee numbers, employee title ID, birth date, first name, last name, sex, and hire date
    - <ins>salaries.csv</ins> - contains employee ID number and the salary they get
    - <ins>titles.csv</ins> - contains the ID number associated with each position title name

- In the main folder, there is a <ins>TableSchema.sql0</ins> which creates and initiates table schema with the proper columns, primary keys, composite keys, and foreign keys to establish proper relationships

- Also in the main folder, an image file displaying the above information in a graphical / diagram format exists as well.  This is the ERD (entity relationship diagram).  

![Entity Relationship Diagram](https://github.com/user-attachments/assets/8b0e9a26-cf1d-492a-80d0-f594b34e8bb1)

- The main code file <ins>PewlettHackwardEmployeeQuery.sql</ins> performs the below operations
    - Deletes the 6 tables if they exist to make sure we are starting with fresh data
    - Creates tables named dept_manager, employees, departments, salaries, titles, and dept_emp with columns matching the CSV file columns with appropriate data types
    - Using pgAdmin, I used the Import function to insert the data from CSV files in the data folder into the tables created above
    - Use the select function and proper arguments to list the employee number, last name, first name, sex, and salary of each employee

  ![image](https://github.com/user-attachments/assets/3a071418-4f52-4735-9994-00f141d5e865)

    - Use the select function and proper arguments to list the first name, last name, and hire date for the employees who were hired in 1986

  ![2](https://github.com/user-attachments/assets/4538b898-7a8a-475b-9d44-1d6ea32558b6)

   - Use the select function and proper arguments to list the manager of each department along with their department number, department name, employee number, last name, and first name
 
    ![dept_manager](https://github.com/user-attachments/assets/be7e2e48-4005-4b59-ba28-6d04a06cce29)

  - Use the select function and proper arguments to list the department number for each employee along with that employee’s employee number, last name, first name, and department name
 
  ![4](https://github.com/user-attachments/assets/c09b2f8f-920d-4ab7-aa1b-cf768e15e979)

  - Use the select function and proper arguments to list first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.

  ![5](https://github.com/user-attachments/assets/fcda5b06-04d9-4aca-945a-a9ebba539734)

  - Use nested select functions and proper arguments to list each employee in the Sales department, including their employee number, last name, and first name.

  ![6](https://github.com/user-attachments/assets/c96a2643-d6ba-4e52-8380-3e9b6022716d)

  - Use inner joins to combine data from multiple tables in order to extract information to list each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.

  ![7](https://github.com/user-attachments/assets/6e39d054-658a-472e-ad2d-d2945e6b7af8)

  - Use the select function, group by function, and order by function to properly capture, order, and display a list of the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

  ![8](https://github.com/user-attachments/assets/8d3ae6ba-06f9-44a5-9efa-a4445843da82)
