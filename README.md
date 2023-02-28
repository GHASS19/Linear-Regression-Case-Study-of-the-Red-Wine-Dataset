# Linear Regression
# Wine Study

## 1. Sourcing and loading

- Import relevant libraries

-Load the data

-Exploring the data

There are: 1599 rows.
There are: 12 columns.

- Choosing a dependent variable, Fixed Acidity for our regression analysis.

## 2. Cleaning, transforming, and visualizing

- Visualizing correlations

![image](https://user-images.githubusercontent.com/86930309/221759145-4096c811-7035-45ee-9604-6d717c5d5ac1.png)

![image](https://user-images.githubusercontent.com/86930309/221759205-22298928-e8d6-4b54-bc8f-b2668cc99e74.png)

## 3. Modeling

Train/Test split
- Making a Linear regression model: first model

 This model's R-Squared coefficient score explained only about 45% of the variation from the mean.

- Second model: Ordinary Least Squares (OLS)

For this model we added a constant to the X variable and we got an R2 score of 45.5%.

- Third model: multiple linear regression

This model had the highest R2 score of 87.1%.

- Fourth model: avoiding redundancy

We can also see from our early heat map that volatile.acidity and citric.acid are both correlated with pH. We can make a model that ignores those two variables and just uses pH, in an attempt to remove redundancy from our model. This mode got a R2 score of 74.2%. The lower R2 score means the columns were important to predicting the fixed acidity.


## 4. Evaluating and concluding

While our most predictively powerful model was the multiple linear regression, this model had explanatory variables that were correlated with one another, which made some redundancy. Our most elegant and economical model was the last and fourth one. It used fewer predictors to get a good result.
