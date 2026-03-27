# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Import libraries and dataset
   Load required libraries (NumPy, Pandas, etc.) and read the dataset.
2. Prepare the data
   Preparate independent variables (X) and dependent variable (Y), and split into training and testing sets.
3. Train the model
   Apply multivariate linear regression using a suitable method (like Normal Equation or sklearn) and fit the model.
4. Predict and evaluate
   Use the trained model to predict outputs and check accuracy using error metrics (like MSE).

## Program:
**Developed by : Jeeva Nivas M**
**Referance no : 212225040148**
```python
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output:

![WhatsApp Image 2026-03-27 at 11 53 24 PM (1)](https://github.com/user-attachments/assets/41ed12f2-a4bb-479b-b493-7c068900df45)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
