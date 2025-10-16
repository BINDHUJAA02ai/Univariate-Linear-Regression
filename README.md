# Implementation of Univariate Linear Regression
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

## REGISTER NUMBER : 212224230038
## COMPLETED BY : BINDHUJAA S



import numpy as np
X= np.array(eval(input()))
Y= np.array(eval(input()))
X_mean=np.mean(X)
Y_mean=np.mean(Y)
num=0
denom=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denom=(X[i]-X_mean)**2
  m=num/denom
  c=Y_mean-m*X_mean
  print(m,c)
  Y_pred=m*X+c
  print(Y_pred)

  import matplotlib.pyplot as plt
  plt.scatter(X,Y,color='RED')
  plt.plot(X,Y_pred,color='blue')
  plt.show()










```

## Output
</br><img width="684" height="551" alt="500858145-78510642-16e2-4947-bd8a-2e00e855ea30" src="https://github.com/user-attachments/assets/d34a375f-f65c-4d72-835c-cfa33b8664a5" />
</br><img width="752" height="564" alt="500858812-39b8117b-1acf-4550-bbca-c31038b46e9c" src="https://github.com/user-attachments/assets/575d15f2-3196-4f93-9c75-3413bda388ec" />

</br>
<img width="689" height="507" alt="500858924-da6f1dcb-2a85-4be3-b882-ba55b69f4a64" src="https://github.com/user-attachments/assets/ae163bea-367d-42f8-8326-5a1d6568b1d1" />

</br><img width="651" height="516" alt="500859230-04af1765-2311-49e4-91a8-9058ac248d79" src="https://github.com/user-attachments/assets/911f5b60-9b88-4e7f-a6a3-43a68fe60412" />

<img width="746" height="538" alt="500859375-85fee704-b80b-4d57-bdea-1961c5d5fd89" src="https://github.com/user-attachments/assets/59230bdf-b917-4c9e-bdae-62006cb8a1cc" />

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
