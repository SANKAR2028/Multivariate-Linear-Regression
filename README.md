# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>

### Step2
<br>

### Step3
<br>

### Step4
<br>

### Step5
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