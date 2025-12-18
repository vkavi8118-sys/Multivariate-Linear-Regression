# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd
### Step2
Read the csv file
### Step3
Get the value of X and Y variables
### Step4
Create the linear regression model and fit
### Step5
predict the CO2 emission of a car where the weight is 2300kg and volume is 1300 cm cube

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
Register number:25017974
Developed by:Kavinaya V
```
## Output:
![Screenshot 2025-12-09 224151png](https://github.com/user-attachments/assets/db8d07b6-cef7-4a83-b2e3-612484328743)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
