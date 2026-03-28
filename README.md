# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solution
5. End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Irfana M
RegisterNumber: 212225230105
*/
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Irfana M
RegisterNumber: 212225230105
*/
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
B = np.array(eval(input())) 
lu,piv = lu_factor(A)
X = lu_solve((lu,piv),B)
print(X)
```

## Output:
<img width="590" height="630" alt="image" src="https://github.com/user-attachments/assets/524afc71-f2d9-4195-9948-98d3e1bf7cd3" />

<img width="552" height="562" alt="image" src="https://github.com/user-attachments/assets/b28795da-9883-47f5-bf63-8227e334e2c8" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

