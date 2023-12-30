
# COURSE ASSIGNMENT - Databases & SQL for Data Science with Python #

### SUMMARY ###

In this module, you will be working with multiple real-world datasets for the city of Chicago. You will be asked questions that will help you understand the data just as you would in the real world. You will be assessed on the correctness of your SQL queries and results.

Learning Objectives:

    · Discuss real-world datasets
    · Analyze table details and properties
    · Interpret and translate data analysis questions into SQL queries
    · Run SQL queries on real world datasets



# ASSIGNMENT PREPARATION: WORKING WITH REAL-WORLD DATASETS & BUILT-IN SQL FUNCTIONS #



## WORKING WITH REAL-WORLD DATASETS ##

Hello and welcome.
In this video, we'll give you a few hints and tips for
working with real-world datasets.
What you will learn.
At the end of this video,
you will be able to discuss the format of data in databases.
Explain how to load data in databases.
Many of the real-world data sets are made available as CSV files.
These are text files that contain data values typically separated by commas.
In some cases, a different separator such as a semicolon may be used.
For this video, we will use an example of a file called DOGS.csv.
Although this is a fictional dataset that contains names of dogs and their breeds,
we will use it to illustrate concepts that you will then apply to real datasets. 

Sample contents of the DOGS.csv file are shown here.
The first row in the table in many cases contain
attribute labels which map to column names in a table.
In DOGS.csv, the first row contains names of three attributes.
ID is the name of the first attribute, and
the subsequent rows contain ID values of 1, 2, and 3.
The name of dog is the second attribute.
In this case, it has values Wolfie, Fluffy, and Huggy, and
the third attribute is called breed, dominant breed, if not a pure breed,
it has values German, Shepherd, Pomeranian, and Labrador.
As we saw in the DOGS.csv file, CSV files can have the first or
a header row that contains the names of the attributes.

If you are loading the data into databases using the phpMyAdmin tool while
importing the CSV file to your database, browse to the file to upload it. 
And then, select CSV from the dropdown under the Format section.
This will generate a section named Format Specific Options.
At the bottom, you will observe a checkbox specifying that the first line of
the file contains the table column names.
For a CSV with headers,
you can select this checkbox before clicking the Go button.
MySQL will auto-detect the header names as column names and process appropriate,
create, and insert statements to populate the data in the table.
The default name of the table is kept as the name of the file in lowercase.
As is evident from the example being discussed, the column names can often have
spaces and optionally, special characters in the column names of the data.
To query such columns,
it is often an accepted practice to use backticks around the column name.
Note that use of any other form of quotes, like single quotes or double quotes,
will not work with column names.
If you have very long queries such as join queries or nested queries,
it may be useful to split the query into multiple lines for improved readability.
In Python notebooks, you can use the backslash character to indicate
continuation to the next row, as shown in this example, using line magic.
You might get an error if you split the query into multiple lines in a Python
notebook without the backslash.
When using SQL cell magic, the content of the cell is interpreted as an SQL code.
This makes the use of backslash at the end of each line redundant.
In Python, you can also query the tables in a database using
read_sql method from the Pandas library.
This function will be easier to use if you have the query saved in a specific
variable say query_statement.
In such cases, if your query contains double quotes,
possibly to specify a column name with spaces or special characters,
you could differentiate the quote by using single quotes for the Python variable
to enclose the SQL query and double quotes for the column names.
What if you need to specify single quotes within the query, for
example, to specify a value in the where clause?
In this case, you can use backslash as the escape character before the quote.
How would you restrict the number of rows retrieved?
A table may contain thousands or millions of rows,
but you may only want to just sample some data sample or
look at just a few rows to see what kind of data the table contains.
You may be tempted to just do select star from table name to retrieve
the results in a Pandas data frame and do a head on it.
But doing so may take a long time for a query to run.
Instead, you can restrict the results set by using the LIMIT clause.
For example, use the following query to retrieve just the first three rows
in a table called census data, select asterisk from census_data LIMIT 3.
Now you know that datasets are basically CSVs,
which are text files containing data values separated by commas. 

Use the phpMyAdmin tool statement to load data in the database.
To query columns in a table, backticks are used around the column name.
Refrain from using single or double quotes.
Long queries, join queries, or
nested queries need to be split into multiple lines for improved readability.
In Python, the tables can be queried in the database using
the read_sql method from the Pandas library.
Use the LIMIT clause to restrict the result set.



## GETTING TABLE & COLUMN DETAILS ##

Hello and welcome.
In this video we'll look at how to get information about tables and
their columns in a database.
What you will learn at the end of this video,
you will be able to, discuss how to get a list of tables in a database,
discuss how to get a list of tables in an SQLite3 database.
Now, how do you get a list of tables in the database?
Sometimes your database may contain several tables and
you may not remember the correct name.
For example, you may wonder whether the table is called dog, dogs,
or four-legged mammals.
Database systems typically contain system or catalog tables from where you can
query the list of tables and get their properties.
In DB2, this catalog is called SYSCAT.TABLES, in SQL Server,
it's information_Schema.tables, in SQLite3,
it is sqlite_master, and in MySQL, it is SHOW TABLES.
To get a list of tables in an SQLite3 database, you can run the following query.
SELECT name FROM sqlite_master WHERE type='table'.
The same can be done in a MySQL interface using the statement, SHOW TABLES.
To extract the attributes or column headers of the dataset tables you can make
use of specific commands in each type of servers.
For instance, in SQLite3 you can use the command PRAGMA table_info.
In MySQL, the command can be used for this is, DESCRIBE table_name.
Know you know that, database systems typically contain system or catalog tables
from where you can query the list of tables and get their properties.
To get a list of tables in SQLite3 database,
use SELECT name FROM sqlite_master WHERE type="table".
To extract the attributes in SQLite3,
use PRAGMA table_info(table_name).



## SUMMARY & HIGHLIGHTS ##

Congratulations! You have completed this lesson. At this point in the course, you know:  

    How to work with real-world datasets, gaining practical experience in handling and analyzing data. 

    The process of obtaining table and column details from databases, which is essential for understanding database structures and designing effective queries.



# USING IBM Db2 #

# FINAL ASSIGNMENT #
