
# GETTING STARTED WITH SQL #

### SUMMARY ###

In this module, you will be introduced to databases. You will learn how to use basic SQL statements like SELECT, INSERT, UPDATE and DELETE. You will also get an understanding of how to refine your query results with the WHERE clause as well as using COUNT, LIMIT and DISTINCT.


# WELCOMO TO SQL #

## COURSE INTRODUCTION ##

In this data-centric era, the role of data and the structures used to support its use become increasingly essential to humankind and the world at large.
Data science is a multi-billion dollar industry, and only poised to grow as we continue to identify its applications in the sciences, politics, business, and almost every other sector of our lives.

Analysts estimate the industry will grow to over 500 billion by the end of this decade.
As a data scientist, you can make $124,000 annually on average.
Exciting, isn’t it?
We generate and store trillions of gigabytes of data every day.
With that being said, the need to analyze, manipulate, and, more importantly, manage this information has become a daunting task.
And so, the importance of data science in today's world cannot be overstated.
As we move towards a data-centric world, the value of data science is rising to new heights.

In the rapidly evolving digital landscape, databases are vast data repositories.
SQL, or Structured Query Language, is the key that unlocks these treasure troves, enabling us to query, update, and manipulate data efficiently.
SQL plays a vital role in the data science workflow, enabling professionals to extract valuable insights from large, intricate datasets.
SQL is powerful, globally relevant (in industry and academia), and widely used by most data scientists today.
A very versatile language called Python is used to connect to various databases, execute SQL queries, and retrieve results in a format conducive to further data analysis.
It offers a wide array of libraries that simplify the connecting process.
This course aims to equip you with the knowledge and skills to harness the power of databases and SQL in your data science endeavors effectively.

In module 1 of this course, you will learn simple SQL for data manipulation in a database table.
In module 2, you will learn about data definition statements and how to create our database tables.
In module 3, you learn about built-in functions, sub-queries, and working with multiple tables.
In module 4, you explore Python for accessing databases using Jupyter Notebooks. Module 5 primarily focuses on a project based on real-world data designed to test what you have learned from the course.
An additional module, 6, covers advanced concepts like Stored Procedures, Views, ACID Transactions, Inner & Outer JOINs.

Additionally, integrated hands-on labs and evaluations allow you to apply the theoretical knowledge to real-world scenarios, enhancing your understanding and retention of the concepts.
These are designed with the sole purpose of maximizing your learning efficacy.
All this will make your journey from learning to mastering SQL for Data Science interactive, engaging, and, most importantly, effective.

So, what are you waiting for?
Let's embrace this exciting journey together! 



## COURSE OVERVIEW ##

The course is structured into 6 weeks, each focusing on a specific topic. 


Week 1: Getting started with SQL 

This week will let you learn the basics of SQL and databases. You will also learn how to query tables in a database. 


Week 2: Introduction to relational Databases and Tables 

This week is all about relational databases, creating tables, and modifying their contents. 


Week 3: Intermediate SQL 

In this module, you will learn more about different types of SQL queries, functions, string patterns, grouping, and sorting. 


Week 4: Accessing databases with Python 

This week, you will learn the nuances of accessing databases using Python libraries and SQL magic in Jupyter Notebooks. 


Week 5: Course Assignment 

This week is designed to give you an understanding of how to deal with real-world datasets and complete an assignment which tests your skills acquired throughout the course.  


Week 6: Bonus Module: Advanced SQL for Data Engineers (Honors) 

In this additional module, you will learn how to apply advanced queries in SQL, like Views, Stored Procedures, and ACID transactions. 



This course can be applied to multiple specializations or Professional Certificates programs. Completing this course will count towards your learning in any of the following programs: 

Data Engineering Foundations Specialization 

IBM Data Analyst Professional Certificate 

Data Science Fundamentals with Python and SQL Specialization 

IBM Data Engineering Professional Certificate 

Introduction to Data Science Specialization 

IBM Data Science Professional Certificate 


Upon completion of the course, you will receive a shareable certificate that you can add to your LinkedIn profile. 




# BASIC SQL #

## INTRODUCTION TO DATABASES ##

What is SQL? SQL is a language used for
relational databases to query
or get data out of a database.
SQL is also referred to
as SQL and is short for its original name,
Structured Query Language.
SQL Is a language used for a database to query data.
But what is data and what is a database?
Data is a collection of facts in the form of words,
numbers, or even pictures.
Data is one of the most critical assets of any business.
It is used and collected practically everywhere.
Your bank stores data about you, your name,
address, phone number, account numbers, etc.
Your credit card company and
your PayPal accounts also store data about you.
Data is important so it needs to be
secure and it needs to be stored and access quickly.
The answer is a database.
What is a database?
Databases are everywhere and used every day,
but they are largely taken for granted.
A database is a repository of data,
it is a program that stores data.
A database also provides the functionality for adding,
modifying, and querying that data.
There are different kinds of databases
of different requirements.
The data can be stored in various forms.
When data is stored in tabular form,
the data is organized in tables like in a spreadsheet,
which is columns and rows, that's relational database.
The columns contain properties
about the item such as LastName,
FirstName, e-mail address, city.
A table is a collection of related things,
like a list of employees or a list of book authors.
In a relational database,
you can form relationships between tables.
A database is a repository of data.
A set of software tools for the data in
the database is called a database management system,
or DBMS, for short.
The terms database, database server, database system,
data server and database
management systems are often used interchangeably.
For relational databases, it's called
a relational database management system or RDBMS.
RDBMS is a set of software tools that controls the data,
such as access, organization, and storage.
RDBMS serves as the backbone
of applications in many industries,
including banking, transportation, health, and so on.
Examples of relational database
management systems are MySQL,
Oracle database, DB2 warehouse,
and DB2 on Cloud.
For the majority of people using a database,
there are five simple commands to create a table,
Insert data to populate the table,
Select data from the table,
Update data in the table,
Delete data from the table.
You can now describe what is SQL,
what is data, what is a database,
and what is a relational database.
You know, the RDBMS stands for
Relational Database Management System
and you can list
five basic SQL commands to create a table,
Insert data to populate the table,
Select data from the table,
Update data in the table,
and Delete data from the table.
Thanks for watching this video. 



## SELECT statement ##

Hello and welcome to retrieving data with a SELECT statement.
In this video, we will learn about retrieving data from
a relational database table by selecting columns of a table.
At the end of this lesson,
you will be able to retrieve data from a relational database table,
to find the use of a predicate,
identify the syntax of the SELECT statement using the WHERE clause, and
list the comparison operators supported by a relational database management system.
The main purpose of a database management system,
is not just to store the data but also facilitate retrieval of the data.
So, after creating a relational database table and inserting data into the table,
we want to see the data.
To see the data, we use the SELECT statement.
The SELECT statement is a data manipulation language statement.
Data Manipulation Language statements or DML statements are used to read and modify data.
The SELECT statement is called a query,
and the output we get from executing this query is called a result set or a result table.
In its simplest form, a SELECT statement is select star from table name.
Based on the book entity example,
we would create the table using
the entity name book and the entity attributes as the columns of the table.
The data would be added to the book table by adding
rows to the table using the insert statement.
In the book entity example, select star from book gives the result set of four rows.
All the data rows for all columns in the table book are displayed.
In addition, you can also retrieve all the rows for all columns by
specifying the column names individually in the SELECT statement.
You don't always have to retrieve all the columns in a table.
You can retrieve just a subset of columns.
If you want, you can retrieve just two columns from the table book.
For example book_id and title.
In this case, the select statement is select book_id, title from book.
In this case, only the two columns display for each of the four rows.
Also notice that the order of the columns displayed
always matches the order in the SELECT statement.
However, what if we want to know the title of the book whose book_id is B1.
Relational operation helps us in restricting
the result set by allowing us to use the clause WHERE.
The WHERE clause always requires a predicate.
A predicate is conditioned evaluates to true, false or unknown.
Predicates are used in the search condition of the WHERE clause.
So, if we need to know the title of the book whose book_id is B1,
we use the WHERE clause with the predicate book_id equals B1.
Select book_id title from book where book_id equals B1.
Notice the result set is now restricted to
just one row whose condition evaluates to true.
The previous example used comparison operator equal to in the WHERE clause.
There are other comparison operators supported by
a relational database management system: equal to,
greater than, less than,
greater than or equal to,
less than or equal to, and not equal to.
Now you can retrieve data and select columns from a relational database table,
define the use of a predicate,
identify the syntax of the SELECT statement using the WHERE clause, and
list the comparison operators supported by a relational database management system.
Thanks for watching this video. 


### SELECT statement examples ###  - Cheat Sheets folder


## COUNT, DISTINCT, LIMIT ##

Hello and welcome.
In this video, we'll briefly present a few useful expressions that
are used with select statements.
The first one is COUNT, COUNT is a built-in database function that
retrieves the number of rows that match the query criteria.
For example, get the total number of rows in a given table,
select COUNT(*) from tablename.
Let's say you create a table called MEDALS which has a column called COUNTRY, and
you want to retrieve the number of rows where the medal recipient is from Canada.
You can issue a query like this:
Select COUNT(COUNTRY) from MEDALS where COUNTRY='CANADA.'
The second expression is DISTINCT.
DISTINCT is used to remove duplicate values from a result set.
Example, to retrieve unique values in a column,
select DISTINCT columnname from tablename.
In the MEDALS table mentioned earlier,
a country may have received a gold medal multiple times.
Example, retrieve the list of unique countries that received gold medals.
That is, removing all duplicate values of the same country.
Select DISTINCT COUNTRY from MEDALS where MEDALTYPE = 'GOLD'.
The third expression is LIMIT, LIMIT is used for
restricting the number of rows retrieved from the database.
Example, retrieve just the first 10 rows in a table.
Select * from tablename LIMIT 10.
This can be very useful to examine the results set by looking at just a few
rows instead of retrieving the entire result set which may be very large.
Example, retrieve just a few rows in the MEDALS table for a particular year.
Select * from MEDALS where YEAR = 2018 LIMIT 5.
In this video we looked at some useful expressions that are used with select
statements, namely the COUNT, DISTINCT, and LIMIT built-in functions.
Thanks for watching this video.



## INSERT statement ##

Hello, and welcome to the INSERT statement.
In this video, we will learn about populating a relational database table.
At the end of this video, you'll be able to identify the syntax of
the INSERT statement and explain two methods to add rows to a table.
After table is created,
the table needs to be populated with data.
To insert data into a table,
we use the INSERT statement.
The INSERT statement is used to add new rows to a table.
The INSERT statement is one of the data manipulation language statements.
Data manipulation language statements or DML statements are used to read and modify data.
Based on the author entity example,
we created the table using the entity name author,
and the entity attributes as the columns of the table.
Now we will add the data to the author table by adding rows to the table.
To add the data to the author table,
we use the INSERT statement.
The syntax of the INSERT statement looks like this,
insert into table name, column name, values.
In this statement, table name identifies the table,
the column name list identifies each column in the table,
and the values clause specifies the data values to be added to the columns in the table.
To add a row with the data for Raul Chong,
we insert a row with an author underscore ID of A one,
the last name is Chong,
the first name as Raul,
the email as RFC@IBM.com,
the city is Toronto,
and the country as CA for Canada.
The author table has six columns,
so the INSERT statement lists the six column names separated by commas,
followed by a value for each of the columns also separated by commas.
It is important that the number of values provided in the values clause
is equal to the number of column names specified in the column name list.
This ensures that each column has a value.
Tables do not need to be populated one row at a time,
multiple rows can be inserted by specifying each row in the values clause.
In the values clause,
each row is separated by a comma.
For example, in this INSERT statement we are inserting two rows,
one for Raul Chong and one for Rav Ahuja.
Now you can identify the syntax of the INSERT statement,
and explain the two methods to add rows to a table.
One row at a time or multiple rows.
Thanks for watching this video. 



## UPDATE & DELETE statements ##

Hello and welcome to the UPDATE statement and the DELETE statement.
In this video, we will learn about altering and
deleting data in a relational database table.
At the end of this lesson,
you will be able to identify the syntax of the UPDATE statement and
DELETE statement and explain the importance of the WHERE clause in these statements.
After a table is created and populated with data,
the data in a table can be altered with the UPDATE statement.
The UPDATE statement is one of the data manipulation language or DML statements.
DML statements are used to read and modify data.
Based on the author entity example,
we created the table using the entity name
Author and the entity attributes as the columns of the table.
Rows were added to the Author table to populate the table.
Sometime later, you want to alter the data in the table.
To alter or modify the data in the Author table,
we use the UPDATE statement.
The syntax of the UPDATE statement looks like this,
UPDATE [TableName] SET [ColumnName] = [Value] ]> WHERE [Condition] .
In the statement, TableName identifies the table.
The ColumnName identifies the column value to be changed,
as specified in the WHERE [Condition] .
Let's look at an example.
In this example, you want to update the FIRSTNAME and LASTNAME of
the author with AUTHOR_ID A2 from Rav Ahuja to Lakshmi Katta.
In this example, to see the UPDATE statement in action,
we start by selecting all rows from the author table to see the values.
To change the first name and last name to Lakshmi Katta where the AUTHOR_ID = A2,
enter the UPDATE statement as follows.
UPDATE AUTHOR SET LAST NAME = KATTA,
FIRST NAME = LAKSHMI WHERE AUTHOR_ID = A2.
Now, to see the result of the update,
select all rows again from the Author table and you will see that in row
2 the name changed from Rav Ahuja to Lakshmi Katta.
Note that if you do not specify the WHERE clause,
all the rows in the table will be updated.
In this example, without specifying the WHERE clause all rows in
the table would have changed the first and last names to Lakshmi Katta.
Sometime later, there might be a need to remove one or more rows from a table.
The rows are removed with the DELETE statement.
The DELETE statement is one of
the data manipulation language statements used to read and modify data.
The syntax of the DELETE statement looks like this,
DELETE FROM [TABLEName] WHERE [Condition].
The rows to be removed are specified in the WHERE condition.
Based on the author entity example,
we want to delete the rows for AUTHOR_ID A2 and A3.
Let's look at an example.
DELETE FROM AUTHOR WHERE AUTHOR_ID IN ('A2','A3').
Note that if you do not specify the WHERE clause,
all the rows in the table will be removed.
Now you can identify the syntax of the UPDATE statement and
DELETE statement and explain the importance of the WHERE clause in these statements.
Thanks for watching this video.



## SUMMARY ##

Congratulations! You have completed this lesson. At this point in the course, you know: 

    The Data Manipulation Language (DML) statements read and modify data. 

    The search condition of the WHERE clause uses a predicate to refine the search.

    The SQL retrieves specific data from databases.

    The COUNT, DISTINCT, and LIMIT are expressions used with SELECT statements. 

    The real-world applications of SELECT statements.

    The INSERT, UPDATE, and DELETE are DML statements for populating and changing tables. 


### SQL CHEAT SHEET: Basics ###

