# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the linear regression using gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
dataset=pd.read_csv('student_scores.csv')
dataset.head()
x=dataset.iloc[:,:-1].values
x
y=dataset.iloc[:,1].values
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=1/3,random_state=0)
from sklearn.linear_model import LinearRegression
regressor=LinearRegression()
regressor.fit(x_train,y_train)
y_pred=regressor.predict(x_test)
y_pred
y_test
plt.scatter(x_train,y_train,color='green')
plt.plot(x_test,regressor.predict(x_test),color='red')
plt.title("Hours vs Scores (Training Set")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
plt.scatter(x_test,y_test,color='green')
plt.plot(x_test,regressor.predict(x_test),color='red')
plt.title("Hours vs Scores (Training Set")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
```
#OUTPUT:

![image](https://user-images.githubusercontent.com/70479123/161579590-426b4ff8-e3f7-4348-aa4f-c3de742f4daf.png)
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
![image](https://user-images.githubusercontent.com/70479123/161579686-a09d4d28-ca4f-470b-95ef-7434b6bfb6e2.png)

## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
