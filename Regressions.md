# Linear Regressions

Linear regression is a statistical method used to model the relationship between a dependent variable (target variable) and one or more independent variables (predictor variables) by fitting a linear equation to the data. The goal of linear regression is to find the line of best fit that minimizes the distance between the predicted values and actual values.

Linear regression is widely used in data analysis and machine learning because it is simple, interpretable, and can be used to make predictions based on input variables. In machine learning, linear regression is often used as a baseline model to compare against more complex models.

## Implementing Linear Regression in Python using Scikit Learn
Scikit Learn is a popular machine learning library in Python that provides various tools for regression analysis. The following steps are necessary to implement a linear regression model using Scikit Learn:

1. Import the necessary libraries: numpy, pandas, and sklearn.

```
import numpy as np
import pandas as pd
from sklearn.linear_model import LinearRegression

```

2. Load the dataset using pandas.

```
data = pd.read_csv('dataset.csv')

```

3. Prepare the data by splitting it into the dependent and independent variables.

```
X = data['independent_variable'].values.reshape(-1,1)
y = data['dependent_variable'].values.reshape(-1,1)

```

4. Split the dataset into training and testing sets using the train_test_split function from Scikit Learn.

```
from sklearn.model_selection import train_test_split

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=0)

```

5. Create an instance of the LinearRegression class and fit the training data to the model.

```
regressor = LinearRegression()  
regressor.fit(X_train, y_train)

```
6. Predict the values using the test set.

```
y_pred = regressor.predict(X_test)

```

7. Evaluate the performance of the model using metrics such as Mean Squared Error (MSE) or R-Squared (R2).

```
from sklearn.metrics import mean_squared_error, r2_score

print('Mean squared error: %.2f'
      % mean_squared_error(y_test, y_pred))

print('Coefficient of determination: %.2f'
      % r2_score(y_test, y_pred))

```

## Train and Test Splits
Splitting the dataset into training and testing sets is a crucial step in evaluating the performance of a machine learning model. The purpose of this step is to evaluate the model on unseen data to ensure that it generalizes well and is not overfitting to the training data.

By splitting the dataset into training and testing sets, we can train the model on the training set and evaluate its performance on the testing set. This helps us to estimate the performance of the model on new data.

In Scikit Learn, we can use the train_test_split function to split the dataset randomly into training and testing sets. We can specify the size of the testing set using the test_size parameter, which is typically set to 20% or 30% of the total dataset.

## Things I want to know more about
* How can we handle missing values in linear regression?
* What is the difference between simple linear regression and multiple linear regression?
* What are some real-world applications of linear regression?

