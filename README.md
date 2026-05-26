# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1
Import required libraries

Step2
Load the dataset

Step3
Split the dataset and Create the Linear Regression model

Step4
Train the model and Evaluate the model

Step5
Visualize residual errors and Interpret results

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv(r"D:\hack11\caremission.csv")
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

<img width="1034" height="299" alt="WhatsApp Image 2026-05-26 at 8 09 23 PM" src="https://github.com/user-attachments/assets/31bb9444-c4f9-4be5-8e48-3a249ad8ff71" />





## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
