# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
# Register No:212224110053
# Developed By:M.K.Suriya prkash
# 1-Norm of a Matrix
def one_norm(matrix):
    cols=zip(*matrix)
    norms=max(sum(abs(x)for x in col)for col in cols)
    return norms
    
matrix=eval(input())
norm=one_norm(matrix)
print(f"{norm:2f}")



# 2-Norm of a Matrix
'''
Program to find 2-norm of a matrix.
Developed by: M.K.Suriya prakash
RegisterNumber: 212224110053
'''
import numpy as np

matrix=eval(input())
np_matrix=np.array(matrix)
l2_norm=np.linalg.norm(np_matrix,2)
print(f"{l2_norm:.2f}")





# Infinity Norm of a Matrix
import numpy as np
mat=np.array(eval(input()))
norm=np.linalg.norm(mat,ord=np.inf)
print("{:.2f}".format(norm))




```
## Output:
### 1-Norm of a Matrix




![image](https://github.com/user-attachments/assets/78714dd0-f83e-4f6f-9c84-0b5579ef259f)

### 2-Norm of a Matrix



![image](https://github.com/user-attachments/assets/7bc3b361-0681-459b-b231-9ef1d8a4e653)


### Infinity Norm of a Matrix



![image](https://github.com/user-attachments/assets/85cb5741-79c8-4e46-a6f2-80f4c56fd2c3)


## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
