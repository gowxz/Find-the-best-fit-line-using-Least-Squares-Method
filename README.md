# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by:Gowtham S 
RegisterNumber:2305002008

import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
n,d=0,0
for i in range(len(x)):
  n+=((x[i]-x_mean)*(y[i]-y_mean))
  d+=((x[i]-x_mean)**2)
m=n/d
b=y_mean-(m*x_mean)
m=round(m,2)
b=round(b,2)
print(m,b)
y_p=(m*x)+b
print(y_p)
error=y-y_p
print(error)
plt.scatter(x,y,color='black')
plt.plot(x,y_p,color='black')
plt.show()  
*/
```

## Output:
C:\Users\admin\Pictures\Screenshots\Screenshot (16).png


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
