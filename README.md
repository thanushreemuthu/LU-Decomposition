# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
(i) To find the L and U matrix

1. Take the input as a square matrix A. 
2. Convert the input into a NumPy array for mathematical operations.
3. Use the lu function from the scipy.linalg library to compute the LU decomposition of matrix A, which returns permutation matrix P, lower triangular matrix L, and upper triangular matrix U.
4. Print the variable 'L' and 'U'.


(ii) To find the LU Decomposition of a matrix

1. Define the package as scipy.linalg import lu.
2. Take two inputs from the user:
A: A square matrix (coefficient matrix).
b: A vector (right-hand side of the linear equations).
3. Convert the inputs into NumPy arrays for numerical operations.
4. : Use the lu_factor function from scipy.linalg to compute the LU decomposition of matrix A. This returns:
lu: Combined LU decomposition.
piv: Pivot indices.
5. Use lu_solve with the LU decomposition (lu, piv) and vector b to compute the solution vector x.
6. Print the variable 'X'
```
## Program:
(i) To find the L and U matrix
```
Program to find L and U matrix using LU decomposition.
Developed by: Thanushree M
RegisterNumber: 24900590
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
```
Program to solve a matrix using LU decomposition.
Developed by: Thanushree M
RegisterNumber: 24900590
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
![Alt text](<Screenshot from 2024-12-06 16-09-54.png>)
![Alt text](<Screenshot from 2024-12-06 15-21-17.png>)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

