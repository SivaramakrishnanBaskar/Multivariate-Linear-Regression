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


## Insert your output
Coefficient [0.00755095 0.00780526]
Intercept 79.69471929115939
predicted CO2 for the corresponding weight and volumes  [114.75968007]
/usr/local/lib/python3.10/dist-packages/sklearn/base.py:439: UserWarning: X does not have valid feature names, but LinearRegression was fitted with feature names
  warnings.warn(
  
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
