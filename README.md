# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1
import pandas as pd.

Step2
Read the CSV file.

Step3
Get the value of x and y variables.

Step4
Create the linear regression model and fit.

Step5
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.

step6
Print the predicted output.

## Program:
```
REG.NO:212222230132
NAME: SANJAY S
import pandas as pd
from sklearn import linear_model
df=pd.read_csv('/content/cars (1)(1).csv')
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("final output:",predictedCO2)






```
## Output:

### Insert your output

Coefficient: [0.00755095 0.00780526]



Intercept: 79.69471929115939


Predicted CO2 for the corresponding weight and volume [114.75968007]


![image](https://github.com/22002102/Multivariate-Linear-Regression/assets/119091638/64b85712-7af3-4766-a72f-8d991021a661)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
