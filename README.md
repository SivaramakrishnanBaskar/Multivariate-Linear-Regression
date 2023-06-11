# Implementation of Multivariate Linear Regression

## Aim
To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:

### Step1

Import pandas as pd

### Step2

Read the csv file

### Step3

Read the csv file

### Step4

Create the linear regression model and fit

### Step5

Predict the CO2 emission of a car where the weight is 2300kg and the volume is 1300cm^3

### Step6
rint the predicted output


## Program:
```
Developed By: Sivaramakrishnan B
Register Number: 212222110044

import pandas as pd 
from sklearn import linear_model
df = pd.read_csv("/content/cars (1).csv")
x = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(x,y)

print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)

predictedCO2 = regr.predict([[3300,1300]])
print("predicted CO2 for the corresponding weight and volumes ",predictedCO2)

```
## Output:
![python exp](https://github.com/SivaramakrishnanBaskar/Multivariate-Linear-Regression/assets/119476322/e41f757f-9062-4e88-b038-f664dd05bfea)
  
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
