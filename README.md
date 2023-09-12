Project Documentation: Data Transformation with Power Query and DAX

Objective:
The objective of this project is to transform and prepare data from multiple sheets within an Excel workbook using Power Query in Power BI. The transformed data is then used to create a dynamic dashboard with calculated measures using DAX (Data Analysis Expressions). This documentation outlines the steps taken to achieve this goal.


Step 1: Data Transformation with Power Query

Opening the CSV File in Power Query Editor:

The Power Query Editor is opened, and the Excel workbook is loaded as a data source.
Removing Unnecessary Columns:

Unnecessary columns are removed from all sheets using Power Query. This step ensures that only relevant data is retained for further processing.
Selecting Data from One Sheet:

One sheet is selected to serve as a template. Power Query automatically applies the necessary modifications made to this sheet to all other sheets in the workbook. This step optimizes the data transformation process.
Changing Header Columns:

Header columns are modified to ensure consistency and data clarity. The top row is deleted as it typically contains header information.
Using Unpivot Function:

The Unpivot function is applied to bring all dates from multiple columns into a single column. This step simplifies data structure for analysis.
Changing Column Data Types:

Column data types are adjusted to match the desired format for analysis.
Dynamic Column Handling:

The transformation process is designed to handle new columns dynamically. If new columns are added to the source data, the existing Power Query template will automatically incorporate them.
Step 2: Creating a Function

Encapsulation into a Function:
All the data transformation actions are encapsulated into a function. This function allows for reusability and can be applied to similar Excel workbooks with minimal changes.
Step 3: DAX Calculations

Total Working Days:

A DAX measure named "Total Working Days" is created to calculate the total working days. It counts the number of working days based on the "Value" column in the transformed data. Non-working days ("WO" for Work Off and "HO" for Holiday) are excluded from the count.
Work_from_home_count:

Another DAX measure, "Work_from_home_count," is created. It assigns values based on the "Value" column to quantify the nature of work (e.g., full work from home, half work from home, or none).
Step 4: Dashboard Creation

Dashboard Design:
The transformed and calculated data is used to create a dynamic dashboard within Power BI. Visualizations, such as charts and tables, are added to present insights effectively.


Conclusion:
This project successfully transformed and prepared attendance data from multiple sheets within an Excel workbook using Power Query in Power BI. The use of DAX measures enhanced the data analysis capabilities, allowing for the calculation of working days and quantifying work-from-home patterns. The encapsulated function and dynamic column handling ensure the project's scalability and reusability for future Excel workbooks with similar data structures.