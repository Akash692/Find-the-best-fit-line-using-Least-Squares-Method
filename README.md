# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. a# Implementation of Univariate Linear Regression


##program

Program to implement univariate Linear Regression to fit a straight line using least squares.

Developed by: DHANAAAKHAASH S.T

RegisterNumber:  212224240032

```
import numpy as np
import matplotlib.pyplot as plt

X = np.array(eval(input()))
Y = np.array(eval(input()))


X_mean = np.mean(X)
Y_mean = np.mean(Y)
num =0
denom=0


for i in range(len(X)):
    num+=(X[i] -X_mean)* (Y[i] -Y_mean)
    denom+= (X[i] - X_mean)**2
    
m= num/denom


b=Y_mean-m*X_mean

print(m,b)

Y_predicted= m*X+b
print(Y_predicted)
plt.scatter(X,Y)
plt.plot(X,Y_predicted,color='red')
plt.show()

```
## Output:

<img width="1348" height="728" alt="{6A3FCD38-7584-494E-97E2-78C09322D6BD}" src="https://github.com/user-attachments/assets/6df5ffb8-f063-42ad-b7ea-d67c4c75763d" />

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.


