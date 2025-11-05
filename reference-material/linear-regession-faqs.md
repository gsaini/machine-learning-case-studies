# FAQ's - Linear Regession

**1. How to import a dataset in Jupyter Notebook?**

Loading data files in Jupyter Notebook slightly differs from Google Colab. Please refer to this link and follow the steps mentioned to load a dataset.

Note: To avoid errors, please ensure that the name of the dataset is correct - check for lower case and upper case, check for spaces, the name of the data set is like Sales.csv, etc

**2. What is the intercept in linear regression?**
The intercept in linear regression is the value at which the regression line crosses the y-axis. It is the expected value of the target when all the predictors are 0. However, the intercept is not always interpretable.

**3. Why should we use drop_first=True to drop one column while creating dummies?**
Consider the feature  'Gender' which has two categories 'Male' and 'Female'. The two columns 'Gender_Female' and 'Gender_Male' will be formed because of get_dummies() and the Gender column will be dropped. Now, because drop_first = True, one column of each category will be dropped. Suppose 'Gender_Female' is dropped

Dropping a column is logical because if the gender is not male, it will be female. That extra column (Gender_Female) adds no value.

Even if gender had three categories 'female', 'male', and 'other', then also dropping one makes sense, because if it's not 'male' or 'other', then it has to be 'female'.

The machine only understands numbers, and the feature name makes no sense to it. Whenever a nominal category column is there, the feature will have values 1 or 0, i.e., whether that particular row belongs to that particular feature or not.

Let us again consider 'Gender'. If the feature is 'Gender_Female' and the value is 1, then the machine only understands that the value for this particular row is 1. If we include the 'Gender_Male' feature as well, the value there will be zero. So adding that column is not significant.

**4. Why do we use .fit() and .predict()? What do .fit() and .predict() do?**
.fit(): Forms a mathematical equation with the help of a training dataset.
.predict(): Will use the mathematical expression obtained from fit() and give the output based on it.
Consider the linear regression equation y = a1x1 + a2x2 + a3x3, where x1, x2, and x3 are three different features. When we use .fit(), the values of all the coefficients are calculated, and when we use .predict(), the feature values for every particular row are used to calculate y for that row. So .predict() gives a Y value as output for each row.
