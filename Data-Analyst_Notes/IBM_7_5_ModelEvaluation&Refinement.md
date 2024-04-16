
# MODEL EVALUATION & REFINEMENT #

### SUMMARY ###

In this module, you will learn about the importance of model evaluation and discuss different data model refinement techniques. You will learn about model selection and how to identify overfitting and underfitting in a predictive model. You will also learn about using Ridge Regression to regularize and reduce standard errors to prevent overfitting a regression model and how to use the Grid Search method to tune the hyperparameters of an estimator.

Learning Objectives:

    - Describe data model refinement techniques
    - Explain overfitting, underfitting, and model selection
    - Apply ridge regression to regularize and reduce the standard errors to avoid overfitting a regression model
    - Apply grid search techniques using Python
    - Explain how grid searches work
    - Describe how ridge regression works to avoid overfitting a model


## MODEL EVALUATION AND REFINEMENT ##

Model evaluation tells us
how our model performs in the real world.
In the previous module,
we talked about in-sample evaluation.
In-sample evaluation tells us how
well our model fits the data already given to train it.
It does not give us an estimate of how
well the trained model can predict new data.
The solution is to split our data up,
use the in-sample data
or training data to train the model.
The rest of the data, called test data,
is used as out-of-sample data.
This data is then used to approximate
how the model performs in the real world.
Separating data into training and
testing sets is an important part of model evaluation.
We use the test data to get an idea
how our model will perform in the real world.
When we split a dataset,
usually the larger portion of data is used for
training and a smaller part is used for testing.
For example, we can use 70% of the data for training.
We then use 30% for testing.
We use training set to build
a model and discover predictive relationships.
We then use a testing set to evaluate model performance.
When we have completed testing our model,
we should use all the data to train the model.
A popular function in the Scikit-learn package for
splitting datasets is the train_test_split function.
This function randomly splits a dataset into training and
testing subsets from the example code snippet.
This method is imported from sklearn.cross validation.
The input parameters y_data is the target variable.
In the car appraisal example it would be the price,
and x_data, the list of predictor variables.
In this case, it would be all the other variables in
the car dataset that we are
using to try to predict the price.
The output is an array, x_train and y_train.
The subsets for training x_test,
and y_test the subsets for testing.
In this case, the test size is
a percentage of the data for the testing set.
Here it is 30%.
The random state is a random seed
for random data set splitting.
Generalization error is a measure of how well
our data does a predicting previously unseen data.
The error we obtain using
our testing data is an approximation of this error.
This figure shows the distribution
of the actual values in
red compared to the predicted values
from a linear regression in blue.
We see the distributions are somewhat similar.
If we generate the same plot using the test data,
we see the distributions are relatively different.
The difference is due to
a generalization error and
represents what we see in the real world.
Using a lot of data for training gives us
an accurate means of determining how
well our model will perform in the real world,
but the precision of the performance will be low.
Let's clarify this with an example.
The center of this bull's eye
represents the correct generalization error.
Let's say we take a random sample of the data using
90% of the data for training and 10% for testing.
The first time we experiment,
we get a good estimate of the training data.
If we experiment again,
training the model with a
different combination of samples,
we also get a good result,
but the results will be
different relative to the
first time we run the experiment.
Repeating the experiment again with
a different combination of training and testing samples,
the results are relatively
close to the generalization error,
but distinct from each other.
Repeating the process, we get
good approximation of the generalization error,
but the precision is poor, i.e.
all the results were
extremely different from one another.
If we use fewer data points to
train the model and more to test the model,
the accuracy of the generalization
performance will be less,
but the model will have good precision.
The figure above demonstrates this.
All our error estimates are relatively close together,
but they are further away from
the true generalization performance.
To overcome this problem,
we use cross validation.
One of the most common out-of-sample evaluation metrics
is cross validation.
In this method, the dataset is split into k equal groups.
Each group is referred to as a fold,
for example, four folds.
Some of the folds can be used as
a training set which we use to train the model,
and the remaining parts are used as
a test set which we use to test the model.
For example, we can use three folds for training,
then use one fold for testing.
This is repeated until
each partition is used for both training and testing.
At the end, we use
the average results as
the estimate of out-of-sample error.
The evaluation metric depends on the model.
For example, the R^2.
The simplest way to apply
cross validation is to call the cross_val_score,
function which performs
multiple out-of-sample evaluations.
This method is imported from
sklearns model selection package.
We then use the function cross_val_score.
The first input parameter is the type of
model we are using to do the cross validation.
In this example, we initialize
the linear regression model or object lr,
which we passed the cross_val_score function.
The other parameters are x_data,
the predictor variable data,
and y_data, the target variable data.
We can manage the number of
partitions with the cv parameter.
Here, cv=3,
which means the data set is
split into three equal partitions.
The function returns an array of scores,
one for each partition that
was chosen as the testing set.
We can average the result together to estimate
out-of-sample R^2 using the mean function in NumPy.
Let's see an animation.
Let's see the result of the
score array in the last slide.
First we split the data into three folds.
We use two folds for
training the remaining fold for testing.
The model will produce an output,
we will use the output to calculate a score.
In the case of the R^2, i.e.
coefficient of determination,
we will store that value in an array,
we will repeat the process using
two folds for training and one fold for testing,
save the score, then use
a different combination for
training and the remaining fold for testing.
We store the final result.
The cross_val_score function returns
the score value to tell us the cross validation result.
What if we want a little more information?
What if we want to know the actual predicted values
supplied by our model before
the R^2 values are calculated?
To do this, we use the cross_val_predict function.
The input parameters are exactly the same
as the cross_val_score function,
but the output is a prediction.
Let's illustrate the process.
First, we split the data into three folds.
We use two folds for training,
the remaining fold for testing.
The model will produce an output
and we will store it in an array.
We will repeat the process using
two folds for training, one for testing.
The model produces an output again.
Finally, we use the last two folds for training,
then we use the testing data.
This final testing fold produces an output.
These predictions are stored in an array. 



## OVERFITTING, UNDERFITTING AND MODEL SLECTION ##

If you recall, in the last module,
we discussed polynomial regression.
In this section, we will discuss how to pick
the best polynomial order and problems
that arise when selecting the wrong order polynomial.
Consider the following function.
We assume the training points come from
a polynomial function plus some noise.
The goal of model selection is to determine the order of
the polynomial to provide
the best estimate of the function y(x).
If we try and fit the function with a linear function,
the line is not complex enough to fit the data.
As a result, there are many errors.
This is called underfitting,
where the model is too simple to fit the data.
If we increase the order of
the polynomial, the model fits better.
But the model is still not
flexible enough and exhibits underfitting.
This is an example of the eighth order polynomial
used to fit the data.
We see the model does well at fitting the data and
estimating the function, even at the inflection points.
Increasing it to a 16th order polynomial,
the model does extremely
well at tracking the training point,
but performs poorly at estimating the function.
This is especially apparent
where there is little training data.
The estimated function oscillates,
not tracking the function.
This is called overfitting,
where the model is too flexible and
fits the noise rather than the function.
Let's look at a plot of the mean square error for
the training and testing set
of different order polynomials.
The horizontal axis represents
the order of the polynomial.
The vertical axis is the mean square error.
The training error decreases
with the order of the polynomial.
The test error is a better means
of estimating the error of a polynomial.
The error decreases till
the best order of the polynomial is determined.
Then the error begins to increase.
We select the order that minimizes the test error.
In this case, it was eight.
Anything on the left would be considered underfitting.
Anything on the right is overfitting.
If we select the best order of the polynomial,
we will still have some errors.
If you recall the original
expression for the training points,
we see a noise term.
This term is one reason for the error.
This is because the noise is
random and we can't predict it.
This is sometimes referred to as an irreducible error.
There are other sources of errors as well.
For example, our polynomial assumption may be wrong.
Our sample points may
have come from a different function.
For example, in this plot,
the data is generated from a sine wave.
The polynomial function does not
do a good job of fitting the sine wave.
For real data, the model may be too difficult to
fit or we may not have
the correct type of data to estimate the function.
Let's try different order polynomials
on the real data using horsepower.
The red points represent the training data,
the green points represent the test data.
If we just use the mean of the data,
our model does not perform well.
A linear function does fit the data better.
A second order model
looks similar to the linear function.
A third order function also appears to increase,
like the previous two orders.
Here we see a fourth order polynomial.
At around 200 horsepower
the predicted price suddenly decreases.
This seems erroneous.
Let's use R^2 to see if our assumption is correct.
The following is a plot of the R^2 value.
The horizontal axis represents
the order of polynomial models.
The closer the R^2 is to one,
the more accurate the model is.
Here we see the R^2 is
optimal when the order of the polynomial is three.
The R^2 drastically decreases
when the order is increased to four,
validating our initial assumption.
We can calculate different R^2 values as follows.
First, we create an empty list to store the values.
We create a list containing different polynomial orders.
We then iterate through the list using a loop.
We create a polynomial feature object with
the order of the polynomial as a parameter.
We transform the training and test data into
a polynomial using the fit transform method.
We fit the regression model using the transformed data.
We then calculate the R^2
using the test data and store it in the array. 



## RIDGE REGRESSION ##

For models with multiple independent features and ones with polynomial feature extrapolation, it is common to have colinear combinations of features. Left unchecked, this multicollinearity of features can lead the model to overfit the training data. To control this, the feature sets are typically regularized using hyperparameters.

Ridge regression is the process of regularizing the feature set using the hyperparameter alpha. The upcoming video shows how Ridge regression can be utilized to regularize and reduce standard errors and avoid over-fitting while using a regression model. 

In this video, we'll discuss ridge regression.
Ridge regression prevents overfitting.
In this video, we will focus on
polynomial regression for visualization.
But overfitting is also a big problem when
you have multiple independent variables or features.
Consider the following fourth order polynomial in orange.
The blue points are generated from this function.
We can use a 10th order polynomial to fit the data.
The estimated function in blue does
a good job at approximating the true function.
In many cases, real data has outliers.
For example, this point shown
here does not appear to come from the function in orange.
If we use a 10th order
polynomial function to fit the data,
the estimated function in blue is incorrect and
is not a good estimate of the actual function in orange.
If we examine the expression for the estimated function,
we see the estimated polynomial coefficients
have a very large magnitude.
This is especially evident
for the higher order polynomials.
Ridge regression controls the magnitude of
these polynomial coefficients by
introducing the parameter Alpha.
Alpha is a parameter we
select before fitting or training the model.
Each row in the following table
represents an increasing value of Alpha.
Let's see how different values of Alpha change the model.
This table represents the polynomial coefficients
for different values of Alpha.
The column corresponds to
the different polynomial coefficients,
and the rows correspond to the different values of Alpha.
As Alpha increases, the parameters get smaller.
This is most evident for
the higher order polynomial features.
But Alpha must be selected carefully.
If Alpha is too large,
the coefficients will approach
zero and underfit the data.
If Alpha is zero,
the overfitting is evident.
For Alpha equal to
0.001 the overfitting begins to subside.
For Alpha equal to
0.01 the estimated function tracks the actual function.
When Alpha equals one,
we see the first signs of underfitting.
The estimated function does not have enough flexibility.
At Alpha equals to 10,
we see extreme underfitting.
It does not even track the two points.
In order to select Alpha,
we use cross validation.
To make a prediction using
ridge regression import ridge from sklearn linear models.
Create a ridge object using the constructor.
The parameter Alpha is one
of the arguments of the constructor.
We train the model using the fit method.
To make a prediction we use the predict method.
In order to determine
the parameter Alpha we use some data for training.
We use a second set called validation data.
This is similar to test data,
but it is used to select parameters like Alpha.
We start with a small value of Alpha.
We train the model, make
a prediction using the validation data,
then calculate the R^2 and store the values.
Repeat the value for a larger value of Alpha.
We train the model again,
make a prediction using the validation data,
then calculate the R^2 and store the values of R^2.
We repeat the process for a different Alpha value,
training the model and making a prediction.
We select the value of Alpha that maximizes the R^2.
Note that we can use other metrics
to select the value of Alpha,
like mean squared error.
The overfitting problem is
even worse if we have lots of features.
The following plot shows
the different values of R^2 on the vertical axis.
The horizontal axis represents
different values for Alpha.
We use several features from
our used car data set and a
second order polynomial function.
The training data is in
red and validation data is in blue.
We see as the value of Alpha increases,
the value of R^2 increases and
converges at approximately 0.75.
In this case, we
select the maximum value of Alpha because
running the experiment for
higher values of Alpha have little impact.
Conversely, as Alpha increases,
the R^2 on the test data decreases.
This is because the term Alpha prevents overfitting.
This may improve the results in the unseen data,
but the model has worse performance on the test data.
See the lab on how to generate this plot. 



## GRID SEARCH ##

[MUSIC] Grid Search allows us to scan through
multiple free parameters with few lines of code.
Parameters like the alpha term discussed in the previous video are not part of
the fitting or training process, these values are called hyperparameters.
Scikit-learn has a means of automatically iterating over these hyperparameters
using cross-validation.
This method is called Grid Search.
Grid Search takes the model or objects you would like to train and
different values of the hyperparameters.
It then calculates the mean square error or r squared for
various hyperparameter values, allowing you to choose the best values.
Let the small circles represent different hyperparameters.
We start off with one value for hyperparameters and train the model.
We use different hyperparameters to train the model.
We continue the process until we have exhausted the different free parameter
values.
Each model produces an error,
we select the hyperparameter that minimizes the error.
To select the hyperparameter, we split our data set into three parts,
the training set, validation set and test set.
We train the model for different hyperparameters, we use the r squared or
mean squared error for each model.
We select the hyperparameter that minimizes the mean squared error or
maximizes the r squared on the validation set.
We finally test our model performance using the test data.
This is the Scikit-learn webpage where the object constructor parameters are given.
It should be noted that the attributes of an object are also called parameters.
We will not make the distinction even though some of the options are not
hyperparameters per se.
In this module, we will focus on the hyperparameter alpha and
the normalization parameter.
The value of your grid search is a Python list that contains a Python dictionary,
the key is the name of the free parameter.
The value of the dictionary is the different values of the free parameter.
This can be viewed as a table with various free parameter values,
we also have the object or model.
The Grid Search takes on the scoring method, in this case r squared,
the number of folds, the model or object, and the free parameter values.
Some of the outputs include the different scores for
different free parameter values.
In this case,
the r squared along with the free parameter values that have the best score.
First, we import the libraries we need, including Grid Search CV,
the dictionary of parameter values.
We create a ridge regression object or model,
we then create a GridSearchCV object.
The inputs are the ridge regression object,
the parameter values and the number of folds.
We will use r squared, this is the default scoring method.
We fit the object, we can find the best values for
the free parameters using the attribute best estimator.
We can also get information like the mean score on the validation data using
the attribute CV result.
One of the advantages of Grid Search is how quickly we can test multiple
parameters. 


## LESSON SUMMARY ##

At this point in the course, you know: 

    - How to split your data using the train_test_split() method into training and test sets. You use the training set to train a model, discover possible predictive relationships, and then use the test set to test your model to evaluate its performance.

    - How to use the generalization error to measure how well your data does at predicting previously unseen data.

    - How to use cross-validation by splitting the data into folds where you use some of the folds as a training set, which we use to train the model, and the remaining parts are used as a test set, which we use to test the model. You iterate through the folds until you use each partition for training and testing. At the end, you average results as the estimate of out-of-sample error.

    - How to pick the best polynomial order and problems that arise when selecting the wrong order polynomial by analyzing models that underfit and overfit your data.

    - Select the best order of a polynomial to fit your data by minimizing the test error using a graph comparing the mean square error to the order of the fitted polynomials.

    - You should use ridge regression when there is a strong relationship among the independent variables.  

    - That ridge regression prevents overfitting.

    - Ridge regression controls the magnitude of polynomial coefficients by introducing a hyperparameter, alpha. 

    - To determine alpha, you divide your data into training  and validation data. Starting with a small value for alpha, you train the model, make a prediction using the validation data, then calculate the R-squared and store the values. You repeat the value for a larger value of alpha. You repeat the process for different alpha values, training the model, and making a prediction. You select the value of alpha that maximizes R-squared.

    - That grid search allows you to scan through multiple hyperparameters using the Scikit-learn library, which iterates over these parameters using cross-validation. Based on the results of the grid search method, you select optimum hyperparameter values.

    - The GridSearchCV() method takes in a dictionary as its argument where the key is the name of the hyperparameter, and the values are the hyperparameter values you wish to iterate over.
    
