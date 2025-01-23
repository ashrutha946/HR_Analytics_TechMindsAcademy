# HR_Analytics_TechMindsAcademy

HR ANALYTICS : POWER BI DASHBOARD PRJECT


OVERVIEW



The data provides various data points to do analyses of a company. Using this data, build a dashboard which will highlight the key performance indicators(KPIs) related to attrition in the company.



The dashboard should help in understanding the attrition by department, job role, age group, years at company, job satisfaction etc. Build the dashboard using the following KPIs:



Data Transformation:




Calculate a column: AttritionCount, conditional column (1 if attrition=Yes, else 0)


Visuals:



Build a visual to highlight total employee in the company



Build a visual to show Total attrition in the company 



Build a visual to show attrition rate in the company( new measure(AttritionRate = sum(AttritionCount)/sum(EmployeeCount)



Build a visual to show average age of employee in the company


Build a visual to show average salary of employee in the company



Build a visual to show average years of employee in the company



Build a visual to show attrition by Education field



Build a visual to show attrition by Age



Build a visual to show Job satisfaction by role



Build a visual to show attrition by salary slab



Build a visual to show attrition by role



Build a visual to attrition by years at company



Build a visual to show attrition by gender



Build a slicer to enable filter by department





Add Title of Project to the dashboard











1. Data Cleaning Procedure




Before building the dashboard, it’s crucial to clean and transform the data to ensure accuracy and usability.




Data Cleaning Steps:




Import Data:




Load the dataset into Power BI from the desired source (Excel, CSV, SQL database, etc.).




Inspect Data:





Navigate to the “Data View” in Power BI to review the data fields, missing values, and inconsistencies.




Handle Missing Values:



Identify columns with missing data and decide how to handle them (e.g., replacing with averages, medians, or removing rows).




Rename Columns:




Rename columns to user-friendly names for better visualization (e.g., “Emp_ID” → “Employee ID”).



Remove Duplicates:



Ensure there are no duplicate records in the dataset.



Create New Columns:




Attrition Count: Create a calculated column in Power BI using the DAX formula:



AttritionCount = IF(Table[Attrition] = "Yes", 1, 0)



Total Employee Count: Use DAX to create a measure for the total number of employees:



TotalEmployees = COUNT(Table[Employee ID])



Calculate Attrition Rate:



AttritionRate = DIVIDE(SUM(Table[AttritionCount]), TotalEmployees, 0)



Categorize Salary Slabs (Optional):




Create a conditional column to group salaries into slabs (e.g., Low, Medium, High).



Normalize Data:





Ensure categorical fields like "Job Role," "Department," or "Education Field" are consistent (e.g., correct typos or standardize labels).****




2. Dashboard Building Procedure


Once the data is clean, follow these steps to create the dashboard:





Visualizations and Layout:




Title and Overview:




Add a clear title to the dashboard: "HR Analytics Dashboard: Employee Attrition Insights".



KPI Cards:




Create individual KPI cards for:


Total Employees


Total Attrition


Attrition Rate


Average Age


Average Salary


Average Years at Company



Attrition Visuals:

Use bar charts or column charts for:



Attrition by Department: Department-wise attrition trends.



Attrition by Job Role: Highlight job roles with high attrition.



Attrition by Education Field: Breakdown by education.




Demographic Analysis:





Use a pie or donut chart for:




Attrition by Gender: Show male vs. female attrition rates.



Use a line chart or histogram for:




Attrition by Age: Age group analysis.




Satisfaction Analysis:



Create bar charts for:



Job Satisfaction by Role: Visualize satisfaction levels for each role.




Use slicers to filter satisfaction by department or gender.




Tenure Analysis:




Use a clustered bar chart:




Attrition by Years at Company: Show trends by employee tenure.




Interactive Slicers:





Add slicers for:




Department




Job Role




Gender




Design the Layout:




Group similar visuals (e.g., demographic visuals in one section, job-related in another).





Use consistent colors (e.g., green for low attrition, red for high attrition).



Interactivity:




Enable filters for all visuals to interact dynamically.




Use drill-through functionality to dive deeper into specific departments or roles.





3. Finalizing and Publishing



Validate the Dashboard:





Cross-check calculations and verify data consistency in visuals.





Test Filters:






Ensure all slicers and filters work as expected.





Publish to Power BI Service:






Upload the dashboard to the Power BI Service for sharing with stakeholders.








