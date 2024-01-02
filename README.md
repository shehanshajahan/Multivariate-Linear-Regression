# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import pandas

### Step2
<br>
Import linear model from sklearn

### Step3
<br>
Read the file cars.csv

### Step4
<br>
Assign the values x and y as required

### Step5
<br>
Create the linear regression model and predict the output

## Program:
```
import pandas as pd
from sklearn import linear_model

df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:
### Insert your output
![Screenshot 2024-01-02 212017](https://github.com/shehanshajahan/Multivariate-Linear-Regression/assets/139317389/ee75893d-46eb-411f-a48e-f4ae36135593)
<br>
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
