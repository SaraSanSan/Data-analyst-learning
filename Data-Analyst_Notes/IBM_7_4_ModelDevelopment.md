
# MODEL DEVELOPMENT #

### SUMMARY ###

In this module, you will learn how to define the explanatory variable and the response variable and understand the differences between the simple linear regression and multiple linear regression models. You will learn how to evaluate a model using visualization and learn about polynomial regression and pipelines. You will also learn how to interpret and use the R-squared and the mean square error measures to perform in-sample evaluations to numerically evaluate our model. And lastly, you will learn about prediction and decision making when determining if our model is correct.

Learning Objectives:

    - Evaluate model using visualizationtechniques in Python
    - Apply polynomial regression techniques using Python
    - Transform data into a polynomial, then use linear regression to fit the parameter
    - Apply model evaluation using visualization in Python
    - Apply polynomial regression techniques to Python
    - Predict and make decisions based on to Python data models
    - Describe the use of R-squared and MSE for in-sample evaluation
    - Define the term "curvilinear relationship"


## MODEL DEVELOPMENT ##

In this video, we will examine
model development by trying to
predict the price of a car using our dataset.
In this module, you will learn about
simple and multiple linear regression,
model evaluation using visualization,
polynomial regression and pipelines,
R-squared and MSE for in-sample evaluation,
prediction and decision making,
and how you can determine a fair value for a used car.
A model or estimator can be thought of as
a mathematical equation used to predict
a value given one or more other values,
relating one or more independent variables
or features to dependent variables.
For example, you input a car models
highway miles per gallon as
the independent variable or feature.
The output of the model or
dependent variable is the price.
Usually the more relevant data you have,
the more accurate your model is.
For example, you input
multiple independent variables or features to your model.
Therefore, your model may
predict a more accurate price for the car.
To understand why more data is
important consider the following situation.
You have two almost identical cars.
Pink cars sell for significantly less.
You want to use your model to
determine the price of two cars,
one pink, one red.
If your model's independent variables
or features do not include color,
your model will predict the same price
for cars that may sell for much less.
In addition to getting more data,
you can try different types of models.
In this course you will learn
about simple linear regression,
multiple linear regression, and polynomial regression. 



## LINEAR REGRESSION AND MULTIPLE LINEAR REGRESSION ##

[MUSIC]
In this video, we'll be talking about simple linear regression and
multiple linear regression.
Linear regression will refer to one independent variable to make a prediction.
Multiple linear regression will refer to multiple independent variables to make
a prediction.
Simple linear regression, or SLR,
is a method to help us understand the relationship between two variables:
the predictor (independent variable x) and the target (dependent variable y).
We would like to come up with a linear relationship between the variables
shown here.
The parameter b0 is the intercept, the parameter b1 is the slope.
When we fit or train the model we will come up with these parameters.
This step requires lots of math, so we will not focus on this part.
Let's clarify the prediction step.
It's hard to figure out how much a car costs, but
the highway miles per gallon is in the owner's manual.
If we assume there is a linear relationship between these variables,
we can use this relationship to formulate a model to determine the price of the car.
If the highway miles per gallon is 20,
we can input this value into the model to obtain a prediction of $22,000.
In order to determine the line,
we take data points from our data set marked in red here.
We then use these training points to fit our model.
The results of the training points are the parameters.
We usually store the data points in two data frame or NumPy arrays.
The value we would like to predict is called the target that we store in
the array y.
We store the dependent variable in the data frame or array x.
Each sample corresponds to a different row in each data frame or array.
In many cases, many factors influence how much people paid for a car,
for example, make or how old the car is.
In this model, this uncertainty is taken into account by assuming
a small random value is added to the point on the line. This is called noise.
The figure on the left shows the distribution of the noise.
The vertical axis shows the value added and
the horizontal axis illustrates the probability that the value will be added.
Usually a small positive value is added or a small negative value. 



## MODEL EVALUATION USING VISUALIZATION ##

In this video, we'll look at model evaluation using visualization.
Regression plots are a good estimate of the relationship between two variables,
the strength of the correlation and the direction of the relationship,
positive or negative.
The horizontal axis is the independent variable.
The vertical axis is the dependent variable.
Each point represents a different target point.
The fitted line represents the predicted value.
There are several ways to plot a regression plot.
A simple way is to use regplot from the Seaborn library.
First, import Seaborn, then use the regplot function.
The parameter x is the name of the column that contains the independent variable or
feature.
The parameter y contains the name of the column that contains the name
of the dependent variable or target.
The parameter data is the name of the dataframe.
The result is given by the plot.
The residual plot represents the error between the actual value.
Examining the predicted value and actual value, we see a difference.
We obtained that value by subtracting the predicted value and
the actual target value.
We then plot that value on the vertical axis with the dependent variable as
the horizontal axis.
Similarly, for the second sample, we repeat the process, subtracting
the target value from the predicted value, then plotting the value accordingly.
Looking at the plot gives us some insight into our data.
We expect to see the results to have zero mean distributed evenly around
the x-axis with similar variance.
There is no curvature.
This type of residual plot suggests a linear plot is appropriate.
In this residual plot, there is a curvature.
The values of the error change with x.
For example, in the region all the residual errors are positive.
In this area, the residuals are negative.
In the final location, the error is large.
The residuals are not randomly separated.
This suggests the linear assumption is incorrect.
This plot suggests a nonlinear function.
We will deal with this in the next section.
In this plot, we see that variance of the residuals increases with x.
Therefore, our model is incorrect.
We can use Seaborn to create a residual plot.
First, import Seaborn, we use the residplot function. 



## POLYNOMINAL REGRESSION AND PIPELINES ##

[MUSIC]
In this video, we will cover polynomial regression and pipelines.
What do we do when a linear model is not the best fit for our data?
Let's look into another type of regression model, the polynomial regression.
We transform our data into a polynomial,
then use linear regression regression to fit the parameter.
Then we will discuss pipelines.
Pipelines are a way to simplify your code.
Polynomial regression is a special case of the general linear regression.
This method is beneficial for describing curvilinear relationships.
What is a curvilinear relationship?
It's what you get by squaring or setting higher-order terms of the predictor
variables in the model transforming the data.
The model can be quadratic,
which means that the predictor variable in the model is squared.
We use a bracket to indicate it as an exponent.
This is a 2nd order polynomial regression with a figure representing the function.
The model can be cubic, which means that the predictor variable is cubed.
This is a 3rd order polynomial regression.
We see by examining the figure that the function has more variation.
There also exists higher-order polynomial regressions
when a good fit hasn't been achieved by 2nd or 3rd order.
We can see in figures how much the graphs change when we change the order
of the polynomial regression.
The degree of the regression makes a big difference and
can result in a better fit if you pick the right value.
In all cases, the relationship between the variable and
the parameter is always linear.
Let's look at an example from our data where we generate a polynomial
regression model.
In Python, we do this by using the polyfit function.
In this example, we develop a 3rd order polynomial regression model base.
We can print out the model.
The symbolic form for the model is given by the following expression:
-1.557 (x_1) cubed + 204.8 (x_1) squared + 8965 x_1 + 1.37 times 10 to the power of 5.
We can also have multidimensional polynomial linear regression.
The expression can get complicated.
Here are just some of the terms for a two-dimensional 2nd order polynomial.
NumPy's polyfit function cannot perform this type of regression.
We use the preprocessing library in scikit-learn
to create a polynomial feature object.
The constructor takes the degree of the polynomial as a parameter.
Then we transform the features into a polynomial feature
with the fit_transform method.
Let's do a more intuitive example.
Consider the features shown here.
Applying the method, we transform the data.
We now have a new set of features that are a transformed version of our original features.
As the dimension of the data gets larger,
we may want to normalize multiple features in scikit-learn.
Instead, we can use the preprocessing module to simplify many tasks.
For example, we can standardize each feature simultaneously.
We import standard scalar.
We train the object, fit the scale object,
then transform the data into a new data frame on array x_scale.
There are more normalization methods available in the preprocessing library
as well as other transformations.
We can simplify our code by using a pipeline library.
There are many steps to getting a prediction.
For example, polynomial transform, normalization, and linear regression.
We simplify the process using a pipeline.
Pipelines sequentially perform a series of transformations.
The last step carries out a prediction.
First, we import all the modules we need.
Then we import the library pipeline.
We create a list of tuples.
The first element in the tuple contains the name of the estimator, model.
The second element contains model constructor.
We input the list in the pipeline constructor.
We now have a pipeline object.
We can train the pipeline by applying the train method to the pipeline object.
We can also produce a prediction as well.
The method normalizes the data, performs a polynomial transform,
then outputs a prediction.
[MUSIC] 


## MEASURES FOR IN-SAMPLE EVALUATION ##

Now that we've seen how we can evaluate a model by using visualization,
we want to numerically evaluate our models.
Let's look at some of the measures that we use for in-sample evaluation.
These measures are a way to numerically determine how good the model fits on
our data.
Two important measures that we often use to determine the fit of
a model are mean squared, error, MSE and R-squared.
To measure the MSE, we find the difference between the actual value y and
the predicted value y Hat then square it.
In this case, the actual value is 150.
The predicted value is 50.
Subtracting these points, we get 100.
We then square the number.
We then take the mean or average of all the errors by adding them all together and
dividing by the number of samples.
To find the MSE in Python, we can import
the mean_squared_error from sk.learn.metrics.
The mean_squared_error function gets two inputs,
the actual value of target variable and the predicted value of target variable.
R squared is also called the coefficient of determination.
It's a measure to determine how close the data is to the fitted regression line.
So how close is our actual data to our estimated model?
Think about it as comparing a regression model to a simple model,
i.e., the mean of the data points.
If the variable x is a good predictor,
our model should perform much better than just the mean.
In this example, the average of the data points y bar is six.
Coefficient of determination R squared is one minus the ratio of
the MSE of the regression line divided by the MSE of the average of the data points.
For the most part, it takes values between zero and one.
Let's look at a case where the line provides a relatively good fit.
The blue line represents the regression line.
The blue squares represent the MSE of the regression line.
The red line represents the average value of the data points.
The red squares represent the MSE of the red line.
We see the area of the blue squares is much smaller than the area of the red
squares.
In this case, because the line is a good fit, the mean squared error is small.
Therefore the numerator is small.
The mean squared error of the average of the data is large as
the denominator is large.
A small number divided by a larger number is an even smaller number.
Taken to an extreme, this value tends to zero.
If we plug in this value from the previous slide for R squared,
we get a value near one.
This means the line is a good fit for the data.
Here is an example of a line that does not fit the data well.
If we just examine the area of the red squares compared to the blue squares,
we see the area is almost identical.
The ratio of the areas is close to one.
In this case, the R squared is near zero.
This line performs about the same as just using the average of the data points.
Therefore, this line did not perform well.
We find the R squared value in Python by using the score method in the linear
regression object.
From the value that we get from this example, we can say that approximately
49.659% of the variation of price is explained by this simple linear model.
Your R squared value is usually between zero and one.
If your r square is negative,
it can be due to overfitting that we will discuss in the next module.
[MUSIC] 


## PREDICTION AND DECISION MAKING ##

In this video, our final topic
will be on prediction and decision making.
How can we determine if our model is correct?
The first thing you should do is make
sure your model results make sense.
You should always use visualization,
numerical measures for evaluation
and comparing between different models.
Let's look at an example of prediction.
If you recall, we train the model using the fit method.
Now we want to find out what the price would be for
a car that has a highway miles per gallon of 30.
Plugging this value into the predict method gives us
a resulting price of $13,771.30.
This seems to make sense for example,
the value is not negative,
extremely high, or extremely low.
We can look at the coefficients by
examining the coef_ attribute.
If you recall,
the expression for the simple linear model
that predicts price from highway miles per gallon,
this value corresponds to the multiple
of the highway miles per gallon feature.
As such, an increase of
one unit in highway miles per gallon,
the value of the car decreases approximately $821.
This value also seems reasonable.
Sometimes your model will
produce values that don't make sense.
For example, if we plot the model out for
highway miles per gallon in the ranges of 0-100,
we get negative values for the price.
This could be because the values
in that range are not realistic.
The linear assumption is incorrect,
or we don't have data for cars in that range.
In this case, it is unlikely that
a car will have fuel mileage in that range,
so our model seems valid.
To generate a sequence of values in a specified range,
import NumPy, then use
the NumPy a range function to generate the sequence.
The sequence starts at
one and increments by one until we reach 100.
The first parameter is
the starting point of the sequence.
The second parameter is
the end point plus one of the sequence.
The final parameter is
the step size between elements in the sequence.
In this case, it's one.
We increment the sequence one step at a time,
from 1 to 2 and so on.
We can use the output to predict new values.
The output is a NumPy array,
many of the values are negative.
Using a regression plot to
visualize your data is the first method you should try.
See the labs for examples of
how to plot polynomial regression.
For this example, the effect of
the independent variable is evident in this case.
The data trends down as the dependent variable increases.
The plot also shows some non linear behavior.
Examining the residual plot, we see in this case,
the residuals have a curvature,
suggesting non linear behavior.
A distribution plot is
a good method for multiple linear regression.
For example, we see the predicted values for prices in
the range from 30,000-50,000 are inaccurate.
This suggests a non linear model may be more
suitable or we need more data in this range.
The mean square error is perhaps
the most intuitive numerical measure
for determining if a model is good or not.
Let's see how different measures of
mean square error impact the model.
The figure shows an example of
a mean square error of 3,495.
This example has a mean square error of 3,652.
The final plot has a mean square error of 12,870.
As the square error increases,
the targets get further from the predicted points.
As we discussed, R^2
is another popular method to evaluate your model.
In this plot, we see
the target points in red and the predicted line in blue,
and R^2 of 0.9986.
The model appears to be a good fit.
This model has an R^2 of 0.9226,
there still is a strong linear relationship.
R^2 of 0.806, the data is a lot more messy,
but the linear relation is evident.
R^2 of 0.61,
the linear function is harder to see,
but on closer inspection,
we see the data is increasing
with the independent variable.
An acceptable value for
R^2 depends on what field you're studying.
Some authors suggest a value should be
equal to or greater than 0.10.
Comparing MLR and SLR is a lower MSE,
always implying a better fit?
Not necessarily.
MSE for an MLR model will be smaller than the MSE for
an SLR model since the errors of
the data will decrease when
more variables are included in the model.
Polynomial regression will also have
a smaller MSE than regular regression.
A similar inverse relationship holds for R^2.
In the next section, we'll look
at better ways to evaluate the model. 


## LESSON SUMMARY ##

At this point in the course, you know: 

    - Linear regression refers to using one independent variable to make a prediction.

    - You can use multiple linear regression to explain the relationship between one continuous target y variable and two or more predictor x variables.

    - Simple linear regression, or SLR, is a method used to understand the relationship between two variables, the predictor independent variable x and the target dependent variable y.

    - Use the regplot and residplot functions in the Seaborn library to create regression and residual plots, which help you identify the strength, direction, and linearity of the relationship between your independent and dependent variables.

    - When using residual plots for model evaluation, residuals should ideally have zero mean, appear evenly distributed around the x-axis, and have consistent variance. If these conditions are not met, consider adjusting your model.

    - Use distribution plots for models with multiple features: Learn to construct distribution plots to compare predicted and actual values, particularly when your model includes more than one independent variable. Know that this can offer deeper insights into the accuracy of your model across different ranges of values.

    - The order of the polynomials affects the fit of the model to your data. Apply Python's polyfit function to develop polynomial regression models that suit your specific dataset.

    - To prepare your data for more accurate modeling, use feature transformation techniques, particularly using the preprocessing library in scikit-learn, transform your data using polynomial features, and use the modules like StandardScaler to normalize the data.

    - Pipelines allow you to simplify how you perform transformations and predictions sequentially, and you can use pipelines in scikit-learn to streamline your modeling process.

    - You can construct and train a pipeline to automate tasks such as normalization, polynomial transformation, and making predictions.

    - To determine the fit of your model, you can perform sample evaluations by using the Mean Square Error (MSE), using Python’s mean_squared_error function from scikit-learn, and using the score method to obtain the R-squared value.

    - A model with a high R-squared value close to 1 and a low MSE is generally a good fit, whereas a model with a low R-squared and a high MSE may not be useful.

    - Be alert to situations where your R-squared value might be negative, which can indicate overfitting. 

    - When evaluating models, use visualization and numerical measures and compare different models.

    - The mean square error is perhaps the most intuitive numerical measure for determining whether a model is good.

    - A distribution plot is a suitable method for multiple linear regression.

    - An acceptable r-squared value depends on what you are studying and your use case.

    - To evaluate your model’s fit, apply visualization, methods like regression and residual plots, and numerical measures such as the model's coefficients for sensibility: 

    - Use Mean Square Error (MSE) to measure the average of the squares of the errors between actual and predicted values and examine R-squared to understand the proportion of the variance in the dependent variable that is predictable from the independent variables.

    - When analyzing residual plots, residuals should be randomly distributed around zero for a good model. In contrast, a residual plot curve or inaccuracies in certain ranges suggest non-linear behavior or the need for more data.
