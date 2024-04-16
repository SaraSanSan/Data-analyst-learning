
# EXPLORATORY DATA ANALYSIS #

### SUMMARY ###

In this module, you will learn what is meant by exploratory data analysis, and you will learn how to perform computations on the data to calculate basic descriptive statistical information, such as mean, median, mode, and quartile values, and use that information to better understand the distribution of the data. You will learn about putting your data into groups to help you visualize the data better, you will learn how to use the Pearson correlation method to compare two continuous numerical variables, and you will learn how to use the Chi-square test to find the association between two categorical variables and how to interpret them.

Learning Objectives:

    - Implement descriptive statistics
    - Demonstrate the basics of grouping
    - Describe data correlation processes


## EXPLORATORY DATA ANALYSIS ##

In this module,
we're going to cover the basics of exploratory data analysis using Python.
Exploratory data analysis or in short, EDA, is an approach to analyze
data in order to summarize main characteristics of the data,
gain better understanding of the data set,
uncover relationships between different variables and
extract important variables for the problem we're trying to solve.
The main question we are trying to answer in this module is,
what are the characteristics that have the most impact on the car price?
We will be going through a couple of different useful exploratory data
analysis techniques in order to answer this question.
In this module, you will learn about, descriptive statistics,
which describe basic features of a data set and
obtains a short summary about the sample and measures of the data.
Basic of grouping data using GroupBy and
how this can help to transform our data set.
ANOVA, the analysis of variance a statistical method in which the variation
in a set of observations is divided into distinct components.
The correlation between different variables.
And lastly, advanced correlation, where we'll introduce you to various correlation
statistical methods, namely Pearson correlation and correlation heatmaps. 



## DESCRIPTIVE STATISTICS ##

In this video, we'll be
talking about descriptive statistics.
When you begin to analyze data,
it's important to first explore your data
before you spend time building complicated models.
One easy way to do so is to
calculate some descriptive statistics for your data.
Descriptive statistical analysis helps
to describe basic features of
a dataset and obtains
a short summary about
the sample and measures of the data.
Let's show you a couple different useful methods.
One way in which we can do this is
by using the describe function in pandas.
Using the describe function and
applying it on your data frame,
a describe function automatically
computes basic statistics for all numerical variables.
It shows the mean, the total number of data points,
the standard deviation, the quartiles,
and the extreme values.
Any NaN values are
automatically skipped in these statistics.
This function will give you a clearer idea of
the distribution of your different variables.
You could have also categorical
variables in your dataset.
These are variables that can be divided up into
different categories or groups and have discrete values.
For example, in our dataset,
we have the drive system as a categorical variable,
which consists of the categories forward wheel-drive,
rear wheel-drive, and four wheel-drive.
One way you can summarize the categorical data is by
using the function value_counts.
We can change the name of
the column to make it easier to read.
We see that we have 118 cars
in the front wheel-drive category,
75 cars in the rear wheel-drive category,
and eight cars in the four wheel-drive category.
Box plots are a great way to visualize numeric data,
since you can visualize
the various distributions of the data.
The main features that the box plot shows are the median
of the data which
represents where the middle data point is,
the upper quartile shows where the 75th percentile is,
the lower quartile shows where the 25th percentile is.
The data between the upper and lower quartile
represents the inter-quartile range.
Next, you have the lower and upper extremes.
These are calculated as 1.5 times
the inter-quartile range above the 75th percentile,
and as 1.5 times the IQR below the 25th percentile.
Finally, box plots also display outliers
as individual dots that occur
outside the upper and lower extremes.
With box plots, you can easily spot
outliers and also see
the distribution and skewness of the data.
Box plots make it easy to compare between groups.
In this example, using box plot,
we can see the distribution of different categories
of the drive-wheels feature over price feature.
We can see that the distribution of price between
the rear wheel-drive and
the other categories are distinct.
But the price for front wheel-drive and
four wheel-drive are almost indistinguishable.
Oftentimes, we tend to see
continuous variables in our data.
These data points are numbers contained in some range.
For example, in our dataset,
price and engine size are continuous variables.
What if we want to understand
the relationship between engine size and price?
Could engine size possibly predict the price of a car?
One good way to visualize this is using a scatter plot.
Each observation in a scatter plot
is represented as a point.
This plot shows the relationship between two variables.
The predictor variable is
the variable that you are using to predict an outcome.
In this case, our predictor variable is the engine size.
The target variable is
the variable that you are trying to predict.
In this case, our target variable
is the price since this would be the outcome.
In a scatter plot, we typically set
the predictor variable on the x-axis or horizontal axis,
and we set the target variable on
the y-axis or vertical axis.
In this case, we will thus plot the engine size on
the x-axis and the price on the y-axis.
We are using the Matplotlib function scatter here,
taking in x and a y variable.
Something to note is that it's
always important to label your axes
and write a general plot title
so that you know what you're looking at.
Now, how is the variable engine size related to price?
From the scatter plot, we see that
as the engine size goes up,
the price of the car also goes up.
This is giving us an initial indication that there is
a positive linear relationship
between these two variables. 



## GROUP-BY in Python ##

In this video, we'll cover the basics of
grouping and how this can help to transform our data set.
Assume you want to know, is there
any relationship between
the different types of drive system,
forward, rear, and four-wheel drive,
and the price of the vehicles.
If so, which type of
drive system adds the most value to a vehicle?
It would be nice if we could
group all the data by the different types of
drive wheels and compare
the results of these different
drive wheels against each other.
In Pandas, this can be done using the groupby method.
The groupby method is used on categorical variables,
groups the data into subsets according
to the different categories of that variable,
you can group by a single variable,
or you can group by multiple variables
by passing in multiple variable names.
As an example, let's say we are
interested in finding the average price of vehicles
and observe how they differ between different types of
body styles and drive wheels variables.
To do this, we first pick out
the three data columns we are interested in,
which is done in the first line of code.
We then group the reduced data according to
drive wheels and body style in the second line.
Since we are interested in knowing how
the average price differs across the board,
we can take the mean of each group and
append at this bit at the very end of the Line 2.
The data is now grouped into subcategories,
and only the average price of each subcategory is shown.
We can see that according to our data,
rear-wheel drive convertibles and
rear-wheel drive hardtops have the highest value,
while four-wheel drive hatchbacks have the lowest value.
A table of this form isn't the easiest to
read and also not very easy to visualize.
To make it easier to understand,
we can transform this table to
a pivot table by using the pivot method.
In the previous table,
both drive wheels and body style were listed in columns.
A pivot table has one variable displayed along
the columns and the other variable
displayed along the rows.
Just with one line of code
and by using the Pandas pivot method,
we can pivot the body style variable
so it is displayed along the columns,
and the drive wheels will be displayed along the rows.
The price data now becomes a rectangular grid,
which is easier to visualize.
This is similar to what is
usually done in Excel spreadsheets.
Another way to represent the pivot table
is using a heat map plot.
Heat map takes a rectangular grid of data and assigns
a color intensity based on
the data value at the grid points.
It is a great way to plot
the target variable over multiple variables,
and through this, get visual clues of
the relationship between these variables and the target.
In this example, we use Pyplot's pcolor method to plot
heat map and convert
the previous pivot table into a graphical form.
We specified the red-blue color scheme.
In the output plot,
each type of body style is numbered along the x-axis,
and each type of drive wheels
is numbered along the y-axis.
The average prices are plotted with
varying colors based on
their values according to the color bar.
We see that the top section of the heat map
seems to have higher prices in the bottom section. 



## CREATING DIFFERENT TYPES OF PLOTS in Python ##

Visualizations play a key role in data analysis. In this reading, you'll be introduced to various forms of graphs and plots that you can create with your data in Python that help you in visualising your data for better analysis.

The two major libraries used to create plots are matplotlib and seaborn. We will learn the prominent plotting functions of both these libraries as applicable to Data Analysis.
Importing libraries

You can import the above mentioned libraries as shown below.

a. matplotlib

    1    from matplotlib import pyplot as plt

Alternatively, the command can also be written as:

    1    import matplotlib.pyplot as plt

Note that most of the plots that are of interest to us in this library are contained in the pyplot subfolder of the package.

matplotlib functions return a plot object which requires additional statements to display. While using matplotlib in Jupyter Notebooks, we require the graph to be displayed inside the notebook interface itself. It is, therefore, essential to add the following 'magic' statement after loading the library.

    1    %matplotlib inline

b. seaborn
Seaborn is usually imported in a code using the following statement:

    1    import seaborn as sns


## Matplotlib functions

### 1. Standard Line Plot

The simplest and most fundamental plot is a standard line plot. The function expects two arrays as input, x and y, both of the same size. x is treated as an independent variable and y as the dependent one. The graph is plotted as shortest line segments joining the x,y point pairs ordered in terms of the variable x.

Syntax:

    1    plt.plot(x,y)

A sample plot is shown in the image below.

Plot example.

### 2. Scatter plot

Scatter plots are graphs that present the relationship between two variables in a data set. It represents data points on a two-dimensional plane. The independent variable or attribute is plotted on the X-axis, while the dependent variable is plotted on the Y-axis.

Scatter plots are used in either of the following situations:

    When we have paired numerical data
    When there are multiple values of the dependent variable for a unique value of an independent variable
    In determining the relationship between variables in some scenarios

Syntax:

    1    plt.scatter(x,y)

Here, x contains the independent variable, and y contains the dependent variable. You have the option to change the size, color, and shape of the markers with additional attributes in the function.
A sample scatter plot is shared below.
Sample scatter plot.

### 3. Histogram

A histogram is an important visual representation of data in categorical form. To view the data in a "Binned" form, we may use the histogram plot with a number of bins required or even with the data points that mark the bin edges. The x-axis represents the data bins, and the y-axis represents the number of elements in each of the bins.

Syntax:

    1    plt.hist(x,bins)

An example of a histogram plot is shown below. Use an additional argument, edgecolor, for better clarity of plot.
Consider the graph shown below. The left graph is the histogram plot for a data set, plotted without setting the edgecolor. The right one is the same graph but has the edgecolor argument set as the color black.

Histogram plot example.

### 4. Bar plot

A bar plot is used for visualizing catogorical data. The y-axis represents the average value of data points belonging to a particular category, while the x-axis represents the number of elements in the different categories.

Syntax:

    1    plt.bar(x,height)

Here, x is the categorical variable, and height is the number of values belonging to the category. You can adjust the width of each bin using an additional width argument in the function.

A sample graph is shown below.

Sample bar plot graph.

### 5. Pseudo Color Plot

A pseudocolor plot displays matrix data as an array of colored cells (known as faces). This plot is created as a flat surface in the x-y plane. The surface is defined by a grid of x and y coordinates that correspond to the corners (or vertices) of the faces. Matrix C specifies the colors at the vertices. The color of each face depends on the color of one of its four surrounding vertices. Of the four vertices, the one that comes first in the x-y grid determines the color of the face.

In this course, you use the pcolor plot for visualizing the contents of a pivot table that has been grouped on the basis of 2 parameters. Those parameters then represent the x and y-axis components that create the grid. The values in the pivot table are the average values of a third parameter. These values act as the code for the color the cell is going to take.

Syntax:

    1    plt.pcolor(C)

You can define an additional cmap argument to specify the color scheme of the plot.

Two sample pcolor plots are shown below, created for same data but for different color schemes.

Sample pcolor plots.


## Seaborn functions

### 6. Regression plot

A regression plot draws a scatter plot of two variables, x and y, and then fits the regression model and plots the resulting regression line along with a 95% confidence interval for that regression. The x and y parameters can be shared as the dataframe headers to be used, and the data frame itself is passed to the function as well.

Syntax:

    1    sns.regplot(x = 'header_1',y = 'header_2',data= df)

A sample regression plot is shared below.

Sample regression plot.

### 7. Box and whisker plot

A box plot (or box-and-whisker plot) shows the distribution of quantitative data in a way that facilitates comparisons between variables or across levels of a categorical variable. The box shows the quartiles of the dataset while the whiskers extend to show the rest of the distribution, except for points that are determined to be "outliers".

Consider the Box and whisker plot interpretation figure shown below.
Box and whisker plot example.

The plot uses whiskers to represent Minimum value to 25% quartile data and 75% quartile to Maximum value data. The range between 25% quartile and 75% quartile is considered as the Inter-Quartile Range. Outliers are generally classified as being outside 1.5 times the interquartile range.

A sample box plot is shown below
Box plot example.

### 8. Residual Plot

A residual plot is used to display the quality of polynomial regression. This function will regress y on x as a polynomial regression and then draw a scatterplot of the residuals.
Residuals are the differences between the observed values of the dependent variable and the predicted values obtained from the regression model. In other words, a residual is a measure of how much a regression line vertically misses a data point, meaning how far off the predictions are from the actual data points.

Syntax:

    1    sns.residplot(data=df,x='header_1', y='header_2')

Alternatively:

    1    sns.residplot(x=df['header_1'], y=df['header_2'])

A sample plot is shown below.

Residual plot example.

### 9. KDE plot

A Kernel Density Estimate (KDE) plot is a graph that creates a probability distribution curve for the data based upon its likelihood of occurrence on a specific value. This is created for a single vector of information. It is used in the course in order to compare the likely curves of the actual data with that of the predicted data.

Syntax:

    1    sns.kdeplot(X)

A sample graph made for a random set of values is shown below.

KDE plot examplke.

### 10. Distribution Plot

This plot has the capacity to combine the histogram and the KDE plots. This plot creates the distribution curve using the bins of the histogram as a reference for estimation. You can optionally keep or discard the histogram from being displayed. In the context of the course, this plot can be used interchangeably with the KDE plot.

Syntax:

    1    sns.distplot(X,hist=False)

Here, keeping the argument hist as True would plot the histogram along with the distribution plot. Both variations are shown in the image below.

Histogram and KDE sample plots.



## CORRELATION ##

In this video, we'll talk about the correlation between different variables.
Correlation is a statistical metric for
measuring to what extent different variables are interdependent.
In other words, when we look at two variables over time,
if one variable changes, how does this affect change in the other variable?
For example, smoking is known to be correlated to lung cancer,
since you have a higher chance of getting lung cancer if you smoke.
In another example, there is a correlation between umbrella and rain variables,
where more precipitation means more people use umbrellas.
Also, if it doesn't rain, people would not carry umbrellas.
Therefore, we can say that umbrellas and rain are interdependent and
by definition they are correlated.
It is important to know that correlation doesn't imply causation.
In fact, we can say that umbrella and rain are correlated, but we would not have
enough information to say whether the umbrella caused the rain or
the rain caused the umbrella.
In data science, we usually deal more with correlation.
Let's look at the correlation between engine size and price.
This time we'll visualize these two variables using a scatter plot and
an added linear line called a regression line,
which indicates the relationship between the two.
The main goal of this plot is to see whether the engine size has
any impact on the price.
In this example,
you can see that the straight line through the data points is very steep, which shows
that there is a positive linear relationship between the two variables.
With increase in values of engine size, values of price go up as well, and
the slope of the line is positive.
So there is a positive correlation between engine size and price.
We can use seaborne reg plot to create the scatter plot.
As another example, now let's look at the relationship between highway miles per
gallon to see its impact on the car price.
As we can see in this plot, when highway miles per gallon value goes up,
the value of price goes down.
Therefore, there is a negative linear relationship between highway miles per
gallon and price.
Although this relationship is negative, the slope of the line is steep,
which means that the highway miles per gallon is still a good predictor of price.
These two variables are said to have a negative correlation.
Finally, we have an example of a weak correlation.
For example, both low peak RPM and
high values of peak RPM have low and high prices.
Therefore, we cannot use RPM to predict the values. 


## CORRELATION - STATISTICS ##

In this video, we'll introduce you
to various correlation statistical methods.
One way to measure the strength
of the correlation between
continuous numerical variables is by
using a method called Pearson Correlation.
Pearson Correlation method will give you two values;
the correlation coefficient and the p-value.
How do we interpret these values?
For the correlation coefficient,
a value close to one
implies a large positive correlation,
while a value close to -1
implies a large negative correlation,
and a value close to zero
implies no correlation between the variables.
Next, the p-value will tell us how
certain we are about the correlation that we calculated.
For the p-value,
a value less than 0.001 gives us
a strong certainty about
the correlation coefficient that we calculated,
a value between 0.001
and 0.05 gives us moderate certainty,
a value between 0.05
and 0.1 will give us a weak certainty,
and a p-value larger than
0.1 will give us no certainty of correlation at all.
We can say that there is a strong correlation
when the correlation coefficient is
close to one or -1 and the p-value is less than 0.001.
The following plot shows data
with different correlation values.
In this example, we want to look at the correlation
between the variables horsepower and car price.
See how easy you can calculate
the Pearson Correlation using the Scipy stats package?
We can see that the correlation coefficient is
approximately 0.8 and this is close to one,
so there's a strong positive correlation.
We can also see that the p-value is very small,
much smaller than 0.001,
and so we can conclude that we are
certain about the strong positive correlation.
Taking all variables into account,
we can now create a heat map that indicates
the correlation between each
of the variables with one another.
The color scheme indicates
the Pearson correlation coefficient,
indicating the strength of
the correlation between two variables.
We can see a diagonal line with a dark red color
indicating that all the values on
this diagonal are highly correlated.
This makes sense because when you look closer,
the values on the diagonal are
the correlation of all variables with themselves,
which will be always one.
This correlation heat map gives us
a good overview of how
the different variables are related to one another,
and most importantly,
how these variables are related to price. 


## LESSON SUMMARY ##

At this point in the course, you know: 

    - Tools like the 'describe' function in pandas can quickly calculate key statistical measures like mean, standard deviation, and quartiles for all numerical variables in your data frame. 

    - Use the 'value_counts' function to summarize data into different categories for categorical data. 

    - Box plots offer a more visual representation of the data's distribution for numerical data, indicating features like the median, quartiles, and outliers.

    - Scatter plots are excellent for exploring relationships between continuous variables, like engine size and price, in a car data set.

    - Use Pandas' 'groupby' method to explore relationships between categorical variables.

    - Use pivot tables and heat maps for better data visualizations.

    - Correlation between variables is a statistical measure that indicates how the changes in one variable might be associated with changes in another variable.

    - When exploring correlation, use scatter plots combined with a regression line to visualize relationships between variables.

    - Visualization functions like regplot, from the seaborn library, are especially useful for exploring correlation.

    - The Pearson correlation, a key method for assessing the correlation between continuous numerical variables, provides two critical values—the coefficient, which indicates the strength and direction of the correlation, and the P-value, which assesses the certainty of the correlation.

    - A correlation coefficient close to 1 or -1 indicates a strong positive or negative correlation, respectively, while one close to zero suggests no correlation.

    - For P-values, values less than .001 indicate strong certainty in the correlation, while larger values indicate less certainty. Both the coefficient and P-value are important for confirming a strong correlation.

    - Heatmaps provide a comprehensive visual summary of the strength and direction of correlations among multiple variables.
