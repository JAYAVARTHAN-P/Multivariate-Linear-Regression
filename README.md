# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandaa as pd

### Step2
Read the csv

### Step3
Get the value of

### Step4
Create the linear regerssion model and fit

### Step5
Predict the CO2 emission of a car where the weight is 2300kg and the volume is 1300 cm3

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)

```
## Output:



![3e0daed6-eb7b-4d93-b048-02acd677984b](https://user-images.githubusercontent.com/121369281/214765639-5412c4b3-61ef-440b-8f2d-db3acdae294d.jpeg)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
