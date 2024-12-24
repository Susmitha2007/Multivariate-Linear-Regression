# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

Import pandas.


### Step2

Import linear model from sklearn

### Step3

Read the files cars.csv

### Step4

Assign the values for x and y as requried.

### Step5

Create the LinearRegression model and predict the output

## Program:
```

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:\\Users\\admin\\Downloads\\car.csv")
x=df[['Volume','Weight']]
y=df['CO2']
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("Coeffient",regression.coef_)
print("Intercept",regression.intercept_)
print("CO2 required is",regression.predict([[3300,1300]]))




```
## Output:

![output](<Screenshot 2024-12-24 163714.png>)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.