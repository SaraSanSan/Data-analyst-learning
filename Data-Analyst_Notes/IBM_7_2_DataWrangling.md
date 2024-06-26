
# DATA WRANGLING #

### SUMMARY ###

In this module, you will learn how to perform some fundamental data wrangling tasks that, together, form the pre-processing phase of data analysis. These tasks include handling missing values in data, formatting data to standardize it and make it consistent, normalizing data, grouping data values into bins, and converting categorical variables into numerical quantitative variables.
Learning Objectives

    - Describe how to handle missing values
    - Describe data formatting techniques
    - Describe data normalization and standardization
    - Demonstrate the use of binning
    - Demonstrate the use of categotical variables


## PRE-PROCESSING DATA in Python ##

In this video, we'll be going through
some data pre-processing techniques.
If you're unfamiliar with the term,
data pre-processing is a necessary step in data analysis.
It is the process of converting or mapping data from
one raw form into
another format to make it ready for further analysis.
Data pre processing is often called
data cleaning or data wrangling,
and there are likely other terms.
Here are the topics that we'll
be covering in this module.
First, we'll show you how to
identify and handle missing values.
A missing value condition occurs
whenever a data entry is left empty.
Then we'll cover data formats.
Data from different sources may be in various formats,
in different units, or in various conventions.
We will introduce some methods in
Python Pandas that can
standardize the values into the same format,
or unit, or convention.
After that, we'll cover data normalization.
Different columns of numerical data
may have very different ranges,
and direct comparison is often not meaningful.
Normalization is a way to bring all data into
a similar range for more useful comparison.
Specifically, we'll focus on
the techniques of centering and scaling,
and then we'll introduce data binning.
Binning creates bigger categories
from a set of numerical values.
It is particularly useful for
comparison between groups of data.
Lastly, we'll talk about categorical variables,
and show you how to convert categorical values
into numeric variables to
make statistical modeling easier.
In Python, we usually perform operations along columns.
Each row of the column represents a sample i.e,
a different used car in the database.
You access a column by specifying the name of the column.
For example, you can access symboling and body style.
Each of these columns is a Panda series.
There are many ways to manipulate data frames in Python.
For example, you can add
a value to each entry of a column.
To add one to each symboling entry, use this command.
This changes each value of
the data frame column by adding one to the current value. 



## DEALING WITH MISSING VALUES in Python ##

[MUSIC]
In this video, we will introduce the pervasive problem of missing values
as well as strategies on what to do when you encounter missing values in your data.
When no data value is stored for feature for a particular observation,
we say this feature has a missing value.
Usually, missing value in dataset appears as question mark,
N/A, zero or just a blank cell.
In the example here, the normalized losses feature has a missing value
which is represented with NaN.
But how can you deal with missing data?
There are many ways to deal with missing values and
this is regardless of Python, R or whatever tool you use.
Of course, each situation is different and should be judged differently.
However, these are the typical options you can consider.
The first is to check if the person or
group that collected the data can go back and find what the actual value should be.
Another possibility is just to remove the data where that missing value is found.
When you drop data, you could either drop the whole variable or
just the single data entry with the missing value.
If you don't have a lot of observations with missing data,
usually dropping the particular entry is the best.
If you're removing data,
you want to look to do something that has the least amount of impact.
Replacing data is better since no data is wasted.
However, it's less accurate since we need to replace missing data with
a guess of what the data should be.
One standard replacement technique is to replace missing values by
the average value of the entire variable.
As an example, suppose we have some entries that have missing values for
the normalized losses column and the column average for
entries with data is 4,500.
While there is no way for us to get an accurate guess of what the missing values
under the normalized losses column should have been,
you can approximate their values using the average value of the column, 4,500.
But what if the values cannot be averaged as with categorical variables?
For a variable like fuel type,
there isn't an average fuel type since the variable values are not numbers.
In this case, one possibility is to try using the mode the most common,
like gasoline.
Finally, sometimes we may find another way to guess the missing data.
This is usually because the data gatherer knows something
additional about the missing data.
For example, he may know that the missing values tend to be old cars and
the normalized losses of old cars are significantly higher than
the average vehicle.
And of course,
finally in some cases you may simply want to leave the missing data as missing data.
For one reason or another it may be useful to keep that observation even if
some features are missing.
Now, let's go into how to drop missing values or
replace missing values in Python.
To remove data that contains missing values,
Pandas library has a built in method called dropna.
Essentially, with the dropna method, you can choose to drop rows or
columns that contain missing values like NaN.
So you'll need to specify axis = 0 to drop the rows,
or axis = 1 to drop the columns that contain the missing values.
In this example, there is a missing value in the price column.
Since the price of used cars is what we're trying to predict in our upcoming
analysis, we'd have to remove the cars, the rows that don't have a listed price.
It can simply be done in one line of code using dataframe.dropna.
Setting the argument in place to True allows
the modification to be done on the data set directly,
inplace = True just writes the result back into the data frame.
This is equivalent to this line of code.
Don't forget that this line of code does not change the data frame but
it's a good way to make sure that you are performing the correct operation.
To modify the data frame, you have to set the parameter inplace = True.
You should always check the documentation if you are not familiar with a function or
method.
The Pandas webpage has lots of useful resources.
To replace missing values like NaNs with actual values,
Pandas library has a built in method called Replace,
which can be used to fill in the missing values with the newly calculated values.
As an example, assume that we want to replace the missing values of
the variable normalized losses by the mean value of the variable.
Therefore, the missing value should be replaced by the average of the entries
within that column.
In Python, first we calculate the mean of the column.
Then we use the method Replace to specify the value we would like to
be replaced as the first parameter, in this case NaN.
The second parameter is the value we would like to replace it with i.e,
the mean in this example.
This is a fairly simplified way of replacing missing values.
There are, of course, other techniques such as replacing missing values for
the average of the group instead of the entire data set. 



## DATA FORMATTING in Python ##

In this video, we'll look at
the problem of data with different formats,
units, and conventions and
the Pandas methods that help us deal with these issues.
Data is usually collected from different places,
by different people,
which may be stored in different formats.
Data formatting means bringing
data into a common standard of
expression that allows users
to make meaningful comparisons.
As a part of dataset cleaning,
data formatting ensures that data
is consistent and easily understandable.
For example, people may use
different expressions to represent New York City,
such as N.Y.,
Ny, NY, and New York.
Sometimes this unclean data is a good thing to see.
For example, if you're looking at
the different ways people tend to write New York,
then this is exactly the data that you want.
Or if you're looking for ways to spot fraud,
perhaps writing N.Y. is more likely
to predict an anomaly than if
someone wrote out New York in full.
But perhaps, more often than not,
we just simply want to treat them all as the same entity
or format to make
statistical analysis easier down the road.
Referring to our used car dataset,
there's a feature named city-miles
per gallon in the dataset,
which refers to a car fuel consumption
in miles per gallon unit.
However, you may be someone who
lives in a country that uses metric units,
so you would want to convert those values to liters
per 100 kilometers, the metric version.
To transform miles per
gallon to liters per 100 kilometers,
we need to divide 235 by
each value in the city miles per gallon column.
In Python, this can easily be done in one line of code.
You take the column and set it to equal to
235 divided by the entire column.
In the second line of code,
rename column name from city-miles per gallon to
city-liters per 100 kilometers
using the data frame rename method.
For a number of reasons,
including when you imported dataset into Python,
the data type may be incorrectly established.
For example, here we notice that
the assigned data type to the price feature is
object although the expected data type
should really be an integer or float type.
It is important for later analysis to explore
the feature's data type and
convert them to the correct data types.
Otherwise, the developed models later on may behave
strangely and totally valid data
may end up being treated like missing data.
There are many data types in Pandas.
Objects can be letters or words.
Int64 are integers,
and floats are real numbers.
There are many others that we will not discuss.
To identify a feature's data type in Python,
we can use the dataframe.dtypes method
and check the data type of each variable in a data frame.
In the case of wrong data types,
the method dataframe.astype can be
used to convert a data type from one format to another.
For example, using astype("int") for the price column,
you can convert the object column
into an integer type variable. 



## DATA NORMALIZATION in Python ##

[MUSIC]
In this video we'll be talking about data normalization,
an important technique to understand in data preprocessing.
When we take a look at the used car data set,
we notice in the data that the feature length ranges from 150 to 250,
while feature width and height ranges from 50 to 100.
We may want to normalize these variables so
that the range of the values is consistent.
This normalization can make some statistical analyses easier down the road.
By making the ranges consistent between variables.
Normalization enables a fairer comparison between the different features,
making sure they have the same impact.
It is also important for computational reasons.
Here is another example that will help you understand why normalization is important.
Consider a data set containing two features: age and
income, where age ranges from 0 to 100,
while income ranges from 0 to 20,000 and
higher. Income is about 1,000 times larger than age and
ranges from 20,000 to 500,000.
So these two features are in very different ranges.
When we do further analysis, like linear regression, for example, the attribute
"income" will intrinsically influence the result more due to its larger value.
But this doesn't necessarily mean it is more important as a predictor.
So the nature of the data biases the linear regression model to weigh
income more heavily than age.
To avoid this,
we can normalize these two variables into values that range from 0 to 1.
Compare the two tables at the right.
After normalization, both variables now have a similar influence on the models we
will build later.
There are several ways to normalize data.
I will just outline three techniques.
The first method, called simple feature scaling,
just divides each value by the maximum value for that feature.
This makes the new values range between 0 and 1.
The second method, called min max, takes each value x underscore old,
subtracts it from the minimum value of that feature,
then divides by the range of that feature. Again,
the resulting new values range between 0 and 1.
The third method is called Z-score, or standard score.
In this formula, for each value, you subtract the mu, which is the average
of the feature and then divide by the standard deviation sigma.
The resulting values hover around zero and typically range between negative three and
positive three, but can be higher or lower.
Following our earlier example,
we can apply the normalization method on the length feature.
First, we use the simple feature scaling method,
where we divide it by the maximum value in the feature. Using the Pandas method max(),
This can be done in just one line of code.
Here's the min max method on the length feature.
We subtract each value by the minimum of that column,
then divide it by the range of that column the max minus the min.
Finally, we apply the Z-score method on length feature to normalize the values.
Here we apply the mean and STD method on the length feature.
Mean method will return the average value of the feature in the data set and
STD method will return the standard deviation of the features in the data set.
[MUSIC] 


## BINNING in Python ##

In this video,
we'll be talking about binning as a method of data preprocessing.
Binning is when you group values together into bins.
For example, you can bin age into 0-5, 6-10, 11-15 and so on.
Sometimes binning can improve accuracy of the predictive models.
In addition, sometimes we use data binning to group a set of numerical values into
a smaller number of bins to have a better understanding of the data distribution.
As example, "price" here is an attribute range from 5,000 to 45,500.
Using binning, we categorize the price into three bins: low price,
medium price and high prices.
In the actual car dataset, price is a numerical variable ranging
from 5,188 to 45,400. It has 201 unique values.
We can categorize them into three bins, low, medium and high price cars.
In Python, we can easily implement the binning.
We would like three bins of equal bin width, so
we need four numbers as dividers that are equal distance apart.
First, we use the NumPy function linspace to return the array bins that contains
four equally spaced numbers over the specified interval of the price.
We create a list group underscore names that contains the different bin names.
We use the Pandas function cut to segment and sort the data values into bins.
You can then use histograms to visualize the distribution of the data after they've
been divided into bins.
This is the histogram that we plotted based on the binning
that we applied in the price feature.
From the plot, it is clear that most cars have a low price and
only very few cars have high price.
[MUSIC] 


## TURNING CATEGORICAL VARIABLES INTO QUANTITATIVE VARIABLES in Python ##

In this video, we'll discuss how to turn
categorical variables into
quantitative variables in Python.
Most statistical models cannot take
in objects or strings as input,
and for model training,
only take the numbers as inputs.
In the car data set,
the fuel type feature as
a categorical variable has two values;
gas or diesel which are in string format.
For further analysis, Jerry has to
convert these variables into some form of numeric format.
We encode the values by
adding new features corresponding to
each unique element in
the original feature we would like to encode.
In the case where the feature fuel has two unique values,
gas and diesel, we create
two new features, gas and diesel.
When a value occurs in the original feature,
we set the corresponding value to one in the new feature,
the rest of the features are set to zero.
In the fuel example for car B,
the fuel value is diesel.
Therefore, we set the feature diesel equal
to one and the gas feature to zero.
Similarly for car D,
the fuel value is gas.
Therefore, we set the feature gas equal to
one and the feature diesel equal to zero.
This technique is often called one hot encoding.
In pandas, we can use get_dummies
method to convert
categorical variables to dummy variables.
In Python, transforming categorical variables
to dummy variables is simple.
Following the example pd.get_dummies method
gets the fuel type column and creates
the data frame dummy_variable_one.
The get_dummies method automatically
generates a list of numbers,
each one corresponding to
a particular category of the variable. 


## LESSON SUMMARY ##

At this point in the course, you know:

    - Data formatting is critical for making data from various sources consistent and comparable.

    - Master the techniques in Python to convert units of measurement, like transforming "city miles per gallon" to "city-liters per 100 kilometers" for ease of comparison and analysis.

    - Acquire skills to identify and correct data types in Python, ensuring the data is accurately represented for subsequent statistical analyses.

    - Data normalization helps make variables comparable and helps eliminate inherent biases in statistical models.

    - You can apply Feature Scaling, Min-Max, and Z-Score to normalize data and apply each technique in Python using pandas’ methods.

    - Binning is a method of data pre-processing to improve model accuracy and data visualization.

    - Run binning techniques in Python using numpy's "linspace" and pandas' "cut" methods, particularly for numerical variables like "price."

    - Utilize histograms to visualize the distribution of binned data and gain insights into feature distributions.

    - Statistical models generally require numerical inputs, making it necessary to convert categorical variables like "fuel type" into numerical formats.

    - You can implement the one-hot encoding technique in Python using pandas’ get_dummies method to transform categorical variables into a format suitable for machine learning models.
    
