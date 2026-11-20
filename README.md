# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the NumPy and SciPy libraries.
2. Read the given matrix A.
3.Perform LU decomposition to obtain the lower triangular matrix L and upper triangular matrix U. 
4.Display the L and U matrices and stop the program.

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: JAGADEESH.A
RegisterNumber: 212224230098
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by: JAGADEESH.A
RegisterNumber: 21224230098
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
*/
```

## Output:
<img width="1320" height="388" alt="Screenshot 2026-11-04 123247" src="https://github.com/user-attachments/assets/9d813d62-ebbd-4b9c-b963-21ccb47e9768" />

<img width="1326" height="212" alt="Screenshot 2026-11-04 123304" src="https://github.com/user-attachments/assets/01c115ec-129e-415a-897c-76350028d9b9" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

