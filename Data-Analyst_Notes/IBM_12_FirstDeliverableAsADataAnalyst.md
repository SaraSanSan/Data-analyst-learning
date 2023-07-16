
# PART 1: CLEAN AND PREPARE THE DATA

The dataset used in this lab comes from the following source: https://data.montgomerycountymd.gov/Government/Fleet-Equipment-Inventory/93vc-wpdr under a Public Domain license.

In this final assigment, you will be following the scenario of a recently hired Junior Data Analyst in a local government office, who has been tasked with importing some data from another department which relates to inventory information about their fleet of vehicles. The data is in comma-separated value (CSV) format and the data also needs cleaning up before you can start to run any kind of analysis on it.

Download the file Montgomery_Fleet_Equipment_Inventory_FA_PART_1_START.CSV. Upload and open the file with Excel for the web and convert it to an .XLSX file. Then clean the data as detailed below.

Use the course videos from Module 3 and the lab ‘Hands-on Lab 5: Cleaning Data’ to help you complete these tasks.

Tasks to perform:

> Save the CSV file as an XLSX file: Change the ‘Viewing’ in the ToolTip to ‘Editing’inorder to save the file as an XLSX file. The file is converted when you click ‘Convert’ in the prompt.

Column widths: Sort out the widths of all columns so that the data is clearly visible in all cells.

Empty rows: Use the Filter feature to look for blanks and remove all empty rows from the data.

Duplicate records: Use either the Conditional Formatting or Remove Duplicates feature to look for and remove any duplicated records from the data.

Spelling: The original source file data has not been checked for errors in the spelling. Check for spelling mistakes in the data and fix them.

Whitespace: Use the Find and Replace feature to remove all double-spaces from the data.

Department names: When the data was converted from its data source, the department names (see correct list below) didn’t import correctly and they are now split over two columns in the data. Use Flash Fill to reduce the department names to just one column, and then remove any unnecessary columns.

Department	Department
Board of Elections	Economic Development
Circuit Court	Environmental Protection
Community Engagement Cluster	Finance
Community Use of Public Facilities	Fire and Rescue
Consumer Protection	General Services
Correction and Rehabilitation	Health and Human Services
County Executives Office	
Download your workbook: Use‘Save As’and select‘Download a copy’ to download your completed workbook as Montgomery_Fleet_Equipment_Inventory_FA_PART_1_END.XLSX.



# PART 2: ANALYZE THE DATA

Download and open the Montgomery_Fleet_Equipment_Inventory_FA_PART_2_START.XLSX file in Excel for the web.

Use the course videos from Module 4 and the lab ‘Hands-on Lab 7: Using Pivot Tables’ to help you complete these tasks.

Tasks to perform:

Format the data as a table: Use the Format as Table option to format the data as a table.

Use AutoSum to calculate values: Use AutoSum to find the following values for column ‘C’ and record each of the values:

SUM
AVERAGE
MIN
MAX
COUNT
Create a Pivot Table: Use the PivotTable feature to create a pivot table that displays the Department field in the Rows section, and the Equipment Count in the Values section, so that the pivot table displays the sum of equipment count by department.

Sort the pivot table data: Use the Sort By Value setting on the pivot table to sort it in descending order by the sum of equipment count.

Make two more pivot tables exactly the same as task 3: Follow the same steps you performed in Tasks 3 and 4 to create two more identical pivot tables so that you end up with 3 worksheets that contain identical pivot tables.

Analyze data in the pivot table: Use the PivotTable Fields pane to manipulate and analyze data in the two copied pivot table as follows:

In pivot table 2 add the Equipment Class field below the Department field so that the different vehicle types appear under each department with their respective counts.
Collapse all fields except the top one - Transportation
In pivot table 3 add the Equipment Class field above the Department field so that the different vehicle types appear first, with the different departments listed underneath each vehicle type with their respective counts.
Collapse all fields except the top one - CUV

Download your workbook: Use‘Save As’and select‘Download a copy’ to download your completed workbook as Montgomery_Fleet_Equipment_Inventory_FA_PART_2_END.XLSX.