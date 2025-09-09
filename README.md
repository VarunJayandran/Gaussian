# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

Step 1: Import numpy from the Python libraray.

Step 2: Get the matrix input from the user.

Step 3: Calculate the variable using libraries.

Step 4: Print the result.

Step 5: End the program
## Program:
```
/*
'''Program to solve a matrix using Gaussian elimination without partial pivoting.
Developed by: VARUN J C
RegisterNumber: 212224240179

import numpy as np
import sys
n = int(input())
a  = np.zeros((n,n+1))
x = np.zeros(n)
for i in range(n):
    for j in range(n+1):
        a[i][j] = float(input())
for i in range(n):
    if a[i][i]==0.0:
        sys.exit('Divide by zero detected!')
    for j in range(i+1,n):
        ratio = a[j][i]/a[i][i];
        for k in range(n+1):
            a[j][k]=a[j][k]-ratio*a[i][k]
x[n-1]=a[n-1][n]/a[n-1][n-1]
for i in range (n-2,-1,-1):
    x[i] = a[i][n]
    for j in range(i+1,n):
        x[i] = x[i] - a[i][j]*x[j]
    x[i] = x[i]/a[i][i]
for i in range (n):
    print('X%d = %0.2f ' %(i,x[i]), end = '')

*/
```

## Output:

<img width="1229" height="577" alt="image" src="https://github.com/user-attachments/assets/4b80cae6-6de5-4f3d-8308-c44fc12268c8" />


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

