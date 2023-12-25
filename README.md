![image](https://github.com/DHARSAN23014208/Univariate-Linear-Regression/assets/149365413/0a28ed7e-32d1-4560-9d45-ae4c04c74999)# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
Developed by:DHARSAN KUMAR R
Regisrer number:23014208

import numpy as np 
import matplotlib.pyplot as plt
X=np.array([0,1,2,3,4,5,6,7,8,9])
Y=np.array([1,3,2,5,7,8,8,9,10,12])
XMean=np.mean(X)
YMean=np.mean(Y)
num,den=0,0
for i in range(len(X)):
  num+=(X[i]-XMean)*(Y[i]-YMean)
  den+=(X[i]-XMean)**2
m=num/den
c=YMean-m*XMean
print(m,c)
Y_pred=m*X+c
print(Y_pred)
plt.scatter(X,Y)
plt.plot(X,Y_pred,color="red")
plt.show() 

```
## Output
![image](https://github.com/DHARSAN23014208/Univariate-Linear-Regression/assets/149365413/5a532ad0-533e-4fc7-a962-6510585e24a2)


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
