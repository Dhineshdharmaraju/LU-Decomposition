# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy module to use the built-in functions for calculation.
2. Prepare the lists from each linear equations and assign in np.array().
3. Using the appropriate command, we can find the solutions.
4. End the program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: RANJEN MUNUSWAMY K B
RegisterNumber: 212225040331
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: DINESH D
RegisterNumber: 212225040079
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```

## Output:
<img width="1420" height="839" alt="image" src="https://github.com/user-attachments/assets/05113cce-3367-4045-ad4b-5d88636f273b" />
<img width="1150" height="890" alt="image" src="https://github.com/user-attachments/assets/f9610a8a-68bd-47bf-8ae6-1a49c6ec6076" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

