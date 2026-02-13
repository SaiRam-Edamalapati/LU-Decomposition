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
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Sai Ram E
RegisterNumber: 212224240141
*/
import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))

P, L, U = lu(A)

print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Sai Ram E
RegisterNumber: 212224240141
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))

B = np.array(eval(input()))

lu, pivot = lu_factor(A)
x = lu_solve((lu, pivot), B)

print(x)
```

## Output:
![lu decomposition]()
<img width="1227" height="804" alt="Screenshot 2026-02-13 082445" src="https://github.com/user-attachments/assets/f97ec2de-28a5-4d23-9b0a-6922a6b90f8b" />
<img width="1233" height="581" alt="Screenshot 2026-02-13 082535" src="https://github.com/user-attachments/assets/2fc7e9a9-93e1-47e8-97cc-affc4114bd59" />

<img width="1230" height="929" alt="Screenshot 2026-02-13 082740" src="https://github.com/user-attachments/assets/e63867c3-04ae-4451-b6a3-06074abf0166" />
<img width="1227" height="317" alt="Screenshot 2026-02-13 082821" src="https://github.com/user-attachments/assets/6cec023c-2f95-4343-8006-af1a265295f9" />






## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

