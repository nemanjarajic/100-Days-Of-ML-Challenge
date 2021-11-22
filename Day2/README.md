# Linear Regression

### What is linear regression?
Assuming that two variables are linearly related, the goal of this method is to predict an dependent variable (Y) based on the independent variables (X).
Linear regression tries to find the best linear function(Best Fit Line) that predicts a value Y as a function of the feature.

The best fit line is finding the minimum sum of the residuals squared. Where a residual is the difference of Yi and Yp (predicted value).

### Step 1: Data Preprocessing
  - Import libraries: numpy, pandas, scikit-learn
  - Missing data?
  - Split data
    - X that is the independent values, Y is the dependent value
    - Split into test and training set for both the independent and dependent values
  - Feature scaling is completed by the sklearn library for LinearRegression

### Step 2: Fitting linear regression model to training dataset
  - This is done through the LinearRegression class in sklearn.linear_model as seen below
  ```
  regress = LinearRegression()
  regress = regress.fit(X_train, Y_train)
  ```

### Step 3: Result Prediction
  - Using the predict method in LinearRegression class we initialized with the training set we can predict the dependent value based on the independent. As see below we are putting in the test set for X and receiving its predictions for the Y values.
  ```
  Y_prediction = regress.predict(X_test)
  ```
### Step 4: Visualization
  - With the matplotlib library we want to create a scatter plot of the dataset then superimpose the best fit line over the scatter plot. This is how we can do that for the training dataset:
  
  ```
  plt.scatter(X_train, Y_train, color='red')
  plt.plot(X_train, regress.predict(X_train), color = 'blue')
  ```
