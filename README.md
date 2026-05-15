# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

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
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: Roshan V
RegisterNumber:212225240124
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
n = int(input())

a = []

for i in range(n):
    row = []
    for j in range(n + 1):
        row.append(float(input()))
    a.append(row)

for i in range(n):
    for j in range(i + 1, n):
        ratio = a[j][i] / a[i][i]
        for k in range(n + 1):
            a[j][k] = a[j][k] - ratio * a[i][k]

x = [0 for i in range(n)]

x[n - 1] = a[n - 1][n] / a[n - 1][n - 1]

for i in range(n - 2, -1, -1):
    x[i] = a[i][n]
    for j in range(i + 1, n):
        x[i] = x[i] - a[i][j] * x[j]
    x[i] = x[i] / a[i][i]

for i in range(n):
    print("X%d = %.2f" % (i, x[i]), end=" ") 
*/
```

## Output:
<img width="1333" height="844" alt="image" src="https://github.com/user-attachments/assets/9e26a82f-3bb8-4c29-ac07-34ed0473c0ed" />
<img width="1363" height="415" alt="image" src="https://github.com/user-attachments/assets/7afa324f-8b4c-4a4e-a717-399e62e2126b" />


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

