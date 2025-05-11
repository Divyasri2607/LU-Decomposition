# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy and scipy module to use the built-in functions for calculation
2. Prepare the lists for the given matrix and assign in np.array()
3. Using the scipy.linalg.lu(), we get L and U of the given matrix. Using the scipy.linalg.lu_factor() and scipy.linalg.lu_solve we get the LU decomposition of the given matrix.
4. End of the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Divya Sri V
RegisterNumber: 212224230070
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Divya Sri V
RegisterNumber: 212224230070
'''

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
PV,lu=lu_factor(A)
result=lu_solve((PV,lu),B)
print(result)
```

## Output:
![Screenshot 2025-05-12 004018](https://github.com/user-attachments/assets/5180a783-ca54-434f-819d-78970ef64f3b)

![Screenshot 2025-05-12 004426](https://github.com/user-attachments/assets/8683495d-31de-4279-9b7e-dadba3eae849)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

