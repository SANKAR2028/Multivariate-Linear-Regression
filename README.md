# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1: Import the required libraries — pandas for data handling and linear_model from sklearn for regression.
<br>

### Step2: Read the dataset from the CSV file using pd.read_csv() and store it in a DataFrame.
<br>

### Step3: Assign independent variables (Volume, Weight) to x and the dependent variable (CO2) to y.
<br>

### Step4: Create a LinearRegression() object and fit it using reg.fit(x, y) to find the regression coefficients and intercept.
<br>

### Step5: Use reg.predict([[3300,1300]]) to predict CO₂ emission for the given input values and display the results
<br>

## Program:
```


import pandas as pd
from sklearn import linear_model
df = pd.read_csv("/content/car.csv")
x = df[["Volume","Weight"]]
y = df ["CO2"]
reg = linear_model.LinearRegression()
reg.fit(x,y)
print("Coefficience",reg.coef_)
print("Intercept", reg.intercept_)
print("Predicting the CO2",reg.predict([[3300,1300]]))



```
## Output:

![alt text](<Screenshot 2025-11-13 112613.png>)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
