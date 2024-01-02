# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas

### Step2
Import linear model from sklearn

### Step3
Read the file cars.csv

### Step4
Assign the values x and y as required

### Step5
Create the linear regression model and predict the output

## Program:
```
#Program for implementation of Multivariate linear regression
#Developed by: Shehan Shajahan
#Register Number: 23008724
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
![Screenshot 2024-01-02 212729](https://github.com/shehanshajahan/Multivariate-Linear-Regression/assets/139317389/6efca62f-0978-4c97-b32a-fe9f506f4d7f)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
