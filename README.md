# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Step 1:
Get the independent variable X and dependent variable Y.
## Step 2:
Calculate the mean of the X -values and the mean of the Y -values.
## Step 3:
Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
## Step 4:
Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)
## Step 5:  
Use the slope m and the y -intercept to form the equation of the line.
## Step 6:
Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
# Univariate Linear Regression
# Develpoed by: Dhanusya.K
# Register number: 23006651

import numpy as np
import matplotlib.pyplot as plt 
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
  num+=(x[i]-xmean)*(y[i]-ymean)
  den+=(x[i]-xmean) **2
m=num/den
b=ymean-m*xmean
print(m,b)
ypred=m*x+b
print(ypred)
plt.scatter(x,y,color="Red")
plt.plot(x,ypred, color="Blue")
plt.show()
```
## Output
![image](https://github.com/Dhanu654/Univariate-Linear-Regression/assets/148514965/49458a6b-b161-4dd5-bb16-e3c95c565d7c)
![image](https://github.com/Dhanu654/Univariate-Linear-Regression/assets/148514965/a3ad7f05-bde2-4f60-b913-4d9f5264bbcb)
![image](https://github.com/Dhanu654/Univariate-Linear-Regression/assets/148514965/34b6fec6-ab0b-4fd0-b513-036c2fabc8c2)
</br>
</br>
</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
