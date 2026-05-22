# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the coefficient matrix and convert it into a NumPy array.
2. Use the lu() function from scipy.linalg to decompose the matrix into Lower triangular matrix (L) and Upper triangular matrix (U).
3. For solving the system of equations, read the constant matrix and apply lu_factor() and lu_solve() functions.
4. Display the L matrix, U matrix, and the solution vector obtained from LU Decomposition.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: k.akshara
RegisterNumber: 212225040016
*/import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
p,l,u=lu(matrix)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: akshara.k
RegisterNumber: 212225040016
*/
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix = np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```

## Output:

<img width="1142" height="373" alt="image" src="https://github.com/user-attachments/assets/ff1d82c1-27f7-4900-8a87-4db0776d2567" />
<img width="896" height="183" alt="image" src="https://github.com/user-attachments/assets/864e4e39-c0ed-4729-9a89-8733bc6f13fd" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

