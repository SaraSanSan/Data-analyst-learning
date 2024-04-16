
# IMPORTING DATA SETS #

### SUMMARY ###

In this module, you will learn how to understand data and learn about how to use the libraries in Python to help you import data from multiple sources. You will then learn how to perform some basic tasks to start exploring and analyzing the imported data set.
Learning Objectives

    - Access databases using Python database APIs
    - Analyze Python data using a dataset
    - Identify three Python libraries and describe their uses
    - Read data using Python's Pandas package
    - Demonstrate how to import and export data in Python


## COURSE INTRODUCTION ##

[MUSIC] Welcome.
I'm Joseph, your instructor.
Congratulations on taking your next step toward becoming a data scientist.
Python is a top language for data science.
Now that you know how to program with Python,
you're going to use Python to analyze data.
In this course, you will learn to use the most important libraries for
analyzing data in Python, including NumPy, Pandas, and Klearn.
These Python libraries are integral to becoming a data scientist and
used in industries such as healthcare, finance, insurance, all things Internet,
and many others.
In addition to analyzing data, you'll learn how to build data pipelines and
build your own machine learning model for making predictions on real world data set.
In module one, you'll learn how to understand the data set characteristics,
get an overview of Python packages for analyzing data, and
learn how to import data and start analyzing it.
In module two, I will teach you data wrangling preprocessing,
dealing with missing values, followed by data formatting and data normalization.
In module three, you'll be introduced to exploratory data analysis, descriptive
statistics GroupBy, correlation, and other important statistics.
In module four, you will learn linear regression, model evaluation,
polynomial regression, and pipelines measures for In-sample evaluation,
prediction and decision making.
In module five, you will discover model evaluation and refinement overfitting,
underfitting, model selection, ridge regression, and grid search.
Finally, you will practice your newly acquired skills with a Hands-On project
using a real world data set.
The only prerequisites for this course are programming with Python and
high school math.
Good luck and have fun. 



## UNDERSTANDING THE DATA ##

[MUSIC]
In this video, we'll be looking at the dataset on used car prices.
The data set used in this course is an open dataset by Jeffrey C Schlimmer.
This data set is in CSV format, which separates each of the values with commas,
making it very easy to import in most tools or applications.
Each line represents a row in the data set.
In the hands-on lab for this module, you'll be able to download and
use the CSV file.
Do you notice anything different about the first row?
Sometimes the first row is a header which contains a column name for
each of the 26 columns.
But in this example, it's just another row of data.
So here's the documentation on what each of the 26 columns represent.
There are a lot of columns, and I'll just go through a few of the column names.
But you can also check out the link at the bottom of the slide to go through
the descriptions yourself.
The first attribute,
symboling, corresponds to the insurance risk level of a car.
Cars are initially assigned a risk factor symbol associated with their price.
Then, if an automobile is more risky,
this symbol is adjusted by moving it up the scale.
A value of +3 indicates that the auto is risky, -3, that it's probably pretty safe.
The second attribute, normalized losses,
is the relative average loss payment per insured vehicle year.
This value is normalized for all autos within a particular size
classification two door small, station wagons, sports specialty,
etc, and represents the average loss per car per year.
The values range from 65 to 256.
The other attributes are easy to understand.
If you would like to check out more details,
refer to the link at the bottom of the slide.
Okay, after we understand the meaning of each feature,
we'll notice that the 26th attribute is price.
This is our target value or label.
In other words, this means price is the value that we want to predict from
the data set, and the predictors should be all the other variables listed,
like symboling, normalized losses, make, and so on.
Thus, the goal of this project is to predict price in terms of other car
features.
Just a quick note, this data set is actually from 1985, so
the car prices for the models may seem a little low.
But just bear in mind that the goal of this exercise is to learn how to analyze
the data.
[MUSIC] 



## PYTHON PACKAGES FOR DATA SCIENCE ##

In order to do data analysis in Python,
we should first tell you a little bit about
the main packages relevant to analysis in Python.
A Python library is a collection of functions and methods
that allow you to perform lots of
actions without writing any code.
The libraries usually contain built-in modules
providing different functionalities
which you can use directly.
There are extensive libraries
offering a broad range of facilities.
We have divided the Python data
analysis libraries into three groups.
The first group is called Scientific Computing Libraries.
Pandas offers data structure and tools for
effective data manipulation and analysis.
It provides fast access to structured data.
The primary instrument of Pandas is
a two dimensional table
consisting of column and row labels,
which are called a data frame.
It is designed to provide easy indexing functionality.
The NumPy library uses arrays for its inputs and outputs.
It can be extended to objects for matrices,
and with minor coding changes,
developers can perform fast array processing.
SciPy includes functions for
some advanced math problems as listed on this slide,
as well as data visualization.
Using data visualization methods is the best way to
communicate with others, showing
the meaningful results of analysis.
These libraries enable you to create
graphs, charts, and maps.
The Matplotlib lib package is
the most well-known library for data visualization.
It is great for making graphs and plots.
The graphs are also highly customizable.
Another high-level visualization library is Seaborn.
It is based on Matplotlib.
It's very easy to generate various plots,
such as heat maps, time series, and violin plots.
With machine learning algorithms,
we're able to develop a model using
our data set and obtain predictions.
The algorithmic libraries tackle
some machine learning tasks from basic too complex.
Here we introduce two packages.
The Scikit-learn library contains tools,
for statistical modeling, including regression,
classification, clustering, and so on.
This library is built on NumPy,
SciPy, and Matplotlib.
Statsmodels is also
a Python module that allows users to explore data,
estimate statistical models,
and perform statistical tests. 



## IMPORTING AND EXPORTING DATA IN PYTHON ##

[MUSIC]
In this video, we'll look at how to read in data using Python's Pandas package.
Once we have our data in Python,
then we can perform all the subsequent data analysis procedures we need.
Data acquisition is a process of loading and
reading data into notebook from various sources.
To read any data using Python's Pandas package,
there are two important factors to consider: format and file path.
Format is the way data is encoded.
We can usually tell different encoding schemes by looking at
the ending of the file name.
Some common encodings are CSV, JSON, XLSX, HDF, and so forth.
The path tells us where the data is stored.
Usually it is stored either on the computer we are using, or
online on the internet.
In our case, we found a data set of used cars which was obtained from the web
address shown on the slide.
When Jerry entered the web address in his web browser, he saw something like this.
Each row is one data point.
A large number of properties are associated with each data point.
Because the properties are separated from each other by commas,
we can guess the data format is CSV, which stands for comma-separated values.
At this point, these are just numbers, and don't mean much to humans.
But once we read in this data, we can try to make more sense out of it.
In Pandas, the read_csv method can read in files
with columns separated by commas into a Pandas data frame.
Reading data in Pandas can be done quickly in three lines.
First, import Pandas, then define a variable with a file path.
And then use the read_csv method to import the data.
However, read_csv assumes the data contains a header.
Our data on used cars has no column headers.
So we need to specify read_csv to not assign headers by setting header to none.
After reading the data set, it is a good idea to look at the data frame to get
a better intuition and to ensure that everything occurred the way you expected.
Since printing the entire data set may take up too much time and resources, to save
time, we can just use dataframe.head to show the first n rows of the data frame.
Similarly, dataframe.tail shows the bottom n rows of data frame.
Here we printed out the first five rows of data.
It seems that the data set was read successfully.
We can see that Pandas automatically set the column header as a list of integers,
because we set header= none, when we read the data.
It is difficult to work with the data frame without having meaningful
column names.
However, we can assign column names in Pandas.
In our present case,
it turned out that we have the column names in a separate file online.
We first put the column names in a list called headers.
Then, we set df.columns=headers to replace the default integer headers by the list.
If we use the head method introduced in the last slide to check the data set,
we see the correct headers inserted at the top of each column.
At some point in time, after you've done operations on your data frame,
you may want to export your Pandas data frame to a new CSV file.
You can do this using the method to_csv.
To do this, specify the file path,
which includes the file name that you want to write to.
For example, if you would like to save data frame df,
as automobile.csv to your own computer,
you can use the syntax df.2_csv.
For this course, we will only read and save CSV files.
However, Pandas also supports importing and
exporting of most data file types with different data set formats.
The code syntax for reading and
saving other data formats is very similar to read or save CSV file.
Each column shows a different method to read and save files into a different format.
[MUSIC] 



## GETTING STARTED ANALYZING DATA IN PYTHON ##

In this video, we introduce
some simple Pandas methods that
all data scientists and
analysis should know when using Python,
Pandas, and data.
At this point, we assume that the data has been loaded.
It's time for us to explore the dataset.
Pandas has several built in
methods that can be used to understand
the data type of features or to
look at the distribution of data within the dataset.
Using these methods gives an overview
of the dataset and also points out
potential issues such as the wrong data type of
features which may need to be resolved later on.
Data has a variety of types.
The main types stored in Pandas objects are object,
float, int, and date time.
The data type names are somewhat
different from those in native Python.
This table shows the difference
and similarities between them.
Some are very similar,
such as the numeric data types int and float.
The object pandas type functions
similar to string in Python,
save for the change in name.
While the date time Pandas type is
a very useful type for handling time series data,
there are two reasons to check data types in a dataset.
Pandas automatically assigns types based
on the encoding it detects from the original data table.
For a number of reasons,
this assignment may be incorrect.
For example, it would be awkward if the car price column,
which we should expect contain
continuous numeric numbers,
is assigned the data type of object.
It would be more natural for it to have the float type.
Jerry may need to manually change the data type to float.
The second reason is it allows
an experienced data scientist to see which
Python functions can be applied to a specific column.
For example, some math functions
can only be applied to numerical data.
If these functions are applied to non numerical data,
an error may result.
When the data type method is applied to the dataset.
The data type of each column is returned in a series.
A good data scientist's intuition tells us that
most of the data types make sense.
They make of cars,
for examples are names.
This information should be of type object.
The last one on the list would be an issue.
As bore is a dimension of an engine,
we should expect a numerical data type to be used.
Instead, the object type is used.
In later sections, Jerry will have to
correct these types of mismatches.
Now we would like to check the statistical summary of
each column to learn about
the distribution of data in each column.
The statistical metrics can tell
the data scientist if there
are mathematical issues that may exist,
such as extreme outliers and large deviations,
the data scientists may
have to address these issues later.
To get the quick statistics,
we use the described method.
It returns the number of terms in the column as count,
average column value as mean,
column standard deviation as STD,
and maximum minimum values,
as well as the boundary of each of the quartiles.
By default, the data frame described
functions skips rows and
columns that do not contain numbers.
It is possible to make the described method
work for object type columns as well.
To enable a summary of all the columns,
we could add an argument,
include equals, all inside
the described function bracket.
Now the outcome shows the summary of
all 26 columns including object type attributes.
We see that for the object type columns,
a different set of statistics is
evaluated like unique, top, and frequency.
Unique is the number of distinct objects in the column,
top is most frequently occurring object,
and frequent is the number of
times the top object appears in the column.
Some values in the table are shown here as NaN,
which stands for not a number.
This is because that particular
statistical metric cannot be
calculated for that specific column data type.
Another method you can use to check
your dataset is the dataframe.info function.
This function gives a concise summary of the data frame.
This method prints information
about a data frame including
the index D type and
columns non-null values, and memory usage. 



## ACCESSING DATABASES WITH PYTHON ##

Hello, in this video,
you will learn how to access databases using Python.
Databases are powerful tools for data scientists.
After completing this module,
you will be able to explain the basic concepts
related to using Python to connect to databases.
This is how a typical user accesses
databases using Python code
written on a Jupiter Notebook,
a web-based editor.
There is a mechanism by which
the Python program communicates with the DBMS.
The Python code connects to the database using API calls.
We will explain the basics of
SQL API's and Python DB APIs.
An application programming interface is a set of
functions that you can call to get
access to some type of service.
A SQL API consists of library
function calls as an application programming interface (API)
for the DBMS. To pass SQL statements to the DBMS,
an application program calls functions in the API,
and it calls other functions to retrieve
query results and status information from the DBMS.
The basic operation of
a typical SQL API is illustrated in the figure.
The application program begins
its database access with one
or more API calls that connect the program to the DBMS.
To send a SQL statement to the DBMS,
the program builds the statement as
a text string in a buffer and then
makes an API call to pass
the buffer contents to the DBMS.
The application program makes API calls to check
the status of its DBMS request and to handle errors.
The application program ends its database access
with an API call that disconnects it from the database.
DB API is Python standard
API for accessing relational databases.
It is a standard that allows you to
write a single program that works with
multiple kinds of relational databases
instead of writing a separate program for each one.
If you learn the DB API functions,
then you can apply that knowledge
to use any database with Python.
The two main concepts in
the Python DB API are
connection objects and query objects.
You use connection objects to connect to
a database and manage your transactions.
Cursor objects are used to run queries.
You open a cursor object and then run queries.
The cursor works similar to
a cursor in a text processing system,
where you scroll down in your result
set and get your data into the application.
Cursors are used to scan
through the results of a database.
Here are the methods used with connection objects.
The cursor method returns
a new cursor object using the connection.
The commit method is used to commit
any pending transaction to the database.
The rollback method causes the database to
roll back to the start of any pending transaction.
The closed method is used to close a database connection.
Let's walk through a Python application that
uses the DB API to query a database.
First, you import your database module
by using the connect API from that module.
To open a connection to the database,
you use the connection function
and pass in the parameters.
That is, the database name, username, and password.
The connect function returns a connection object.
After this, you create
a cursor object on the connection object.
The cursor is used to run queries and fetch results.
After running the queries using the cursor,
we also use the cursor to fetch the results of the query.
Finally, when the system is done running the queries,
it frees all resources by closing the connection.
Remember that it is always important to close
connections to avoid unused connections
taking up resources.
Thanks for watching this video. 




## LESSON SUMMARY ##

At this point in the course, you know: 

    - Each line in a dataset is a row, and commas separate the values.

    - To understand the data, you must analyze the attributes for each column of data.

    - Python libraries are collections of functions and methods that facilitate various functionalities without writing code from scratch and are categorized into Scientific Computing, Data Visualization, and Machine Learning Algorithms.

    - Many data science libraries are interconnected; for instance, Scikit-learn is built on top of NumPy, SciPy, and Matplotlib.

    - The data format and the file path are two key factors for reading data with Pandas.

    - The read_CSV method in Pandas can read files in CSV format into a Pandas DataFrame.

    - Pandas has unique data types like object, float, Int, and datetime.

    - Use the dtype method to check each column’s data type; misclassified data types might need manual correction.

    - Knowing the correct data types helps apply appropriate Python functions to specific columns.

    - Using Statistical Summary with describe() provides count, mean, standard deviation, min, max, and quartile ranges for numerical columns.

    - You can also use include='all' as an argument to get summaries for object-type columns.

    - The statistical summary helps identify potential issues like outliers needing further attention.

    - Using the info() Method gives an overview of the top and bottom 30 rows of the DataFrame, useful for quick visual inspection.

    - Some statistical metrics may return "NaN," indicating missing values, and the program can’t calculate statistics for that specific data type.

    - Python can connect to databases through specialized code, often written in Jupyter notebooks.

    - SQL Application Programming Interfaces (APIs) and Python DB APIs (most often used) facilitate the interaction between Python and the DBMS.

    - SQL APIs connect to DBMS with one or more API calls, build SQL statements as a text string, and use API calls to send SQL statements to the DBMS and retrieve results and statuses.

    - DB-API, Python's standard for interacting with relational databases, uses connection objects to establish and manage database connections and cursor objects to run queries and scroll through the results.

    - Connection Object methods include the cursor(), commit(), rollback(), and close() commands.

    - You can import the database module, use the Connect API to open a connection, and then create a cursor object to run queries and fetch results. 

    - Remember to close the database connection to free up resources.
