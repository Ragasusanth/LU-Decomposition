# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## (i) To find the L and U matrix

## Algorithm
### Step 1: Import the necessary libraries (NumPy and LU from SciPy).

### Step 2: Get the input matrix from the user.

### Step 3: Use the lu() function to perform LU Decomposition and obtain P, L, and U matrices.

### Step 4: Print the L (Lower triangular) and U (Upper triangular) matrices.

## Program:

```
'''Program to find L and U matrix using LU decomposition.
Developed by: RAGA.SUSANTH 
RegisterNumber:  212224230217
'''

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

## (ii) To find the LU Decomposition of a matrix

## Algorithm

### Step 1: Import NumPy and required LU functions from SciPy.

### Step 2: Input the coefficient matrix A and the constant matrix B.

### Step 3: Use lu_factor() to decompose matrix A into LU form.

### Step 4: Use lu_solve() with the LU decomposition to find and print the solution vector X.

```
'''Program to solve a matrix using LU decomposition.
Developed by: RAGA SUSANTH   
RegisterNumber:  212224230217 
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
PV,LU=lu_factor(A)
result=lu_solve((PV,LU),B)
print(result)
```

## Output:

(i) To find the L and U matrix

![image](https://github.com/user-attachments/assets/5f28d90d-ea2f-4048-801e-b9cba3cb30cf)

(ii) To find the LU Decomposition of a matrix

![image](https://github.com/user-attachments/assets/17bb0677-da4d-4b1d-828d-5266554e8aac)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

