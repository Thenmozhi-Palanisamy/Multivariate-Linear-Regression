# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>import panda as np

### Step2
<br>Read the csv file

### Step3
<br>get the value of x and y

### Step4
<br>cheat the linear regression model and fit

### Step5
<br>perdic the output

## Program:
```
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars.csv")
x = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCo2 = regr.predict([[3300,1300]])
print('Predicted Co2 for the corresponding weight and volume',predictedCo2)






```
## Output:
![output](.//variate.png)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.