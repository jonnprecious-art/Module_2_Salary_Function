# Module_2_Salary_Function: Data Processing & Integration
SF Salary Analysis System

Project Overview
This project demonstrates a hybrid data processing pipeline using Python and R. It processes the San Francisco City Employee Salary dataset, allows for specific employee record retrieval via a custom function, and handles data exporting and compression.

File Structure
Salary_Analysis.ipynb: The main Jupyter Notebook containing all code.

Salaries.csv: The input dataset.

Employee_Profile.zip: The generated output containing individual employee CSVs.

README.md: Project documentation.

Technical Requirements
To run this notebook, i will need the following installed in my Python environment:

- Python 3.x
- Pandas: For data manipulation.
- rpy2: To execute R code within the Jupyter cells.
- R Environment: Installed on your local machine and linked to Jupyter.

How to Use the Code
1. Data Import & Dictionary Mapping
The notebook first loads the Salaries.csv. To optimize lookup speeds, the data is mapped into a Python dictionary where the EmployeeName serves as the unique key.

2. The Employee Function
I can retrieve any employee's details by calling:

Python
get_employee_details("NAME OF EMPLOYEE")
Error Handling: If the name is misspelled or missing from the dataset, the function will return a friendly error message instead of crashing the program.

3. Exporting Data
To export an employee's profile to the zipped folder:
Run the export_employee_to_zip("Employee Name") function.

This creates a directory named Employee_Profile, saves a CSV, and compresses it into Employee_Profile.zip.

4. R Integration
The final cell uses R magic commands to:

Unzip the folder.
Read the CSV back into an R data frame.
Display the results to the console.

Author
[Precious Donald] Module 2: Python Data Structures and Error Handling
