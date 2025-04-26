# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import required libraries numpy and scipy.linalg.
2. Input the matrix/matrices using eval(input()).
3. Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve().
4. Print the results L and U matrices or solution X matrix.

## Program:
(i) To find the L and U matrix

    '''Program to find L and U matrix using LU decomposition.
    Developed by: NITHYA S
    RegisterNumber: 212224240106
    '''
    import numpy as np
    from scipy.linalg import lu
    A=np.array(eval(input()))
    P,L,U=lu(A)
    print(L)
    print(U)
(ii) To find the LU Decomposition of a matrix

    '''Program to solve a matrix using LU decomposition.
    Developed by: NITHYA S
    RegisterNumber: 212224240106
    '''
    import numpy as np
    from scipy.linalg import lu_factor,lu_solve
    A=np.array(eval(input()))
    b=np.array(eval(input()))
    lu,piv=lu_factor(A)
    X=lu_solve((lu,piv),b)
    print(X)

## Output:

(i) L and U matrix

![image](https://github.com/user-attachments/assets/77d81127-4b9c-47bf-a831-da5686ae3d1c)

(ii) LU Decomposition of a matrix

![image](https://github.com/user-attachments/assets/7bbeb90e-7d5a-44d6-857c-f3b1a6b81601)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

