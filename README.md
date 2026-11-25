# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
   
### Algorithm :  Implementation of Multivariate Linear Regression
### Step 1:  Start the program and import the required libraries such as NumPy, Pandas, and Scikit-learn.
### Step 2:  Load the dataset and separate the independent variables (X) and dependent variable (Y).
### Step 3:  Split the dataset into training and testing data using the train_test_split() function.
### Step 4:  Create and train the Multivariate Linear Regression model using the LinearRegression() function and fit() method.
### Step 5:  Predict the output using the predict() method and display the predicted results.
### Step 6:  Stop the program.

## Program:
```
## Developed By: ESAIYA E
## Reference number: 26014140

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
<img width="1920" height="1080" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/6e1e37dc-053c-4b4f-9aea-ec7424a1ef90" />



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
