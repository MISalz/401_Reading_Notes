# Class13 Reading Notes

### Reading
[How to Run Linear Regression in Python](http://bigdata-madesimple.com/how-to-run-linear-regression-in-python-scikit-learn/)

*NOTE: Since this demo was published scikit-learn has been updated. The train_test_split function is now imported from sklearn.model_selection*

Scikit-learn is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction.

DESCR = give info on data set

Important functions to keep in mind while fitting a linear regression model are:

lm.fit() -> fits a linear model

lm.predict() -> Predict Y using the linear model with estimated coefficients

lm.score() -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.
You can also explore the functions inside lm 

object by pressing lm.\<tab>

.coef_ gives the coefficients and .intercept_ gives the estimated intercepts.

Two other parameters that you can pass to linear regression object are fit_intercept and normalize.

 to calculate the predicted prices (Y^i) using lm.predict.

**Training and validation data sets**
In practice you wont implement linear regression on the entire data set, you will have to split the data sets into training and test data sets. So that you train your model on training data and see how well it performed on test data.

Input:
print “Fit a model X_train, and calculate MSE with Y_train:”, np.mean((Y_train – lm.predict(X_train)) ** 2)

print “Fit a model X_train, and calculate MSE with X_test, Y_test:”, np.mean((Y_test – lm.predict(X_test)) ** 2)

Output:
Fit a model X_train, and calculate MSE with Y_train: 19.5467584735 Fit a model X_train, and calculate MSE with X_test, Y_test: 28.5413672756

### Additional Resources
[Linear Regression in Python](https://realpython.com/linear-regression-in-python/)


### Videos

[Introduction to Simple Linear Regressions](https://www.youtube.com/watch?v=KsVBBJRb9TE)


### Bookmark and Review
[Train & Test Splits](https://towardsdatascience.com/train-test-split-and-cross-validation-in-python-80b61beca4b6)

[What is Linear Regression](https://www.statisticssolutions.com/what-is-linear-regression/)


----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)