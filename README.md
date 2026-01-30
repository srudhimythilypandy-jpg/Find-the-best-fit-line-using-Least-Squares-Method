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
Developed by:srudhi .m 
RegisterNumber:  25016156

import numpy as np
x=np.array([[1 ,1, 2], [1,2 ,1] ,[1, 3 ,4]])
print(x)

y=np.array([[5],[6],[10]])
print(y)

xd=x.T
print(x.T)

xdx=x.T@x
print(x.T@x)

xdx_inv=np.linalg.inv(xdx)
print(np.linalg.inv(xdx))

xdx_inv=np.linalg.inv(xdx)
print(np.linalg.inv(xdx))

temp=xd@x
print(xd@x)

import numpy as np
from sklearn.linear_model import LinearRegression
x=np.array([[1,2],[2,1],[3,4]])
print(x)

y=np.array([5,6,10])
print(y)

model=LinearRegression()
model.fit(x,y)
slope=model.coef_
intercept=model.intercept_
print(slope)
print(intercept)

a=1
b=2
predicted_value=model.predict([[a,b]])
print(predicted_value)

import matplotlib.pyplot as plt

plt.figure()
plt.scatter(y, y_predict)
plt.plot([y.min(), y.max()], [y.min(), y.max()], color='red')
plt.xlabel("Actual values (y)")
plt.ylabel("Predicted values (y_predict)")
plt.title("Actual vs Predicted")
plt.show()


*/
```

## Output:
![best fit line](sam.png)


<img width="909" height="577" alt="Screenshot 2026-01-30 105757" src="https://github.com/user-attachments/assets/1d233dee-5660-4c37-b77a-a9b8fe0cce76" />


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
