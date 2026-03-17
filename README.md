# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1
Import required libraries and load the dataset.

### Step2
Define the feature matrix � and target vector �.

### Step3
Split the dataset into training and testing sets.

### Step4
Create a Linear Regression model and train it using training data.

### Step5
Predict outputs, evaluate the model, and plot the residual errors.

## Program:
```

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars.csv")
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

<img width="771" height="477" alt="Screenshot 2026-03-17 184800" src="https://github.com/user-attachments/assets/7abdf7c6-d7cd-4003-8a39-a58d7aa7d55c" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
