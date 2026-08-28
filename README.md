# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the required libraries such as Pandas and LinearRegression from Scikit-learn.
### Step2
Read the dataset carsemission.csv using Pandas and store it in a DataFrame.
### Step3
Select Weight and Volume as the independent variables and CO2 as the dependent variable.
### Step4
Create a Linear Regression model and train the model using the selected input and output data.
### Step5
Provide new values for Weight and Volume, predict the corresponding CO2 emission, and display the coefficients, intercept, and predicted output.
## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
```
## Output:

### Insert your output
<img width="1027" height="502" alt="image" src="https://github.com/user-attachments/assets/d3bf201f-c35e-431c-a38c-b7b789dca16e" />



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
