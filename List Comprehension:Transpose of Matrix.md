# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
```
def create(r, c):
    mat = []
    for i in range(r):
        row = list(map(int, input().split()))
        mat.append(row)
    return mat

r = int(input())
c = int(input())

matrix = create(r, c)
transpose = [[matrix[j][i] for j in range(r)] for i in range(c)]

for row in transpose:
    print(row)
```
## OUTPUT:
<img width="543" height="418" alt="image" src="https://github.com/user-attachments/assets/5912f993-3fac-4dd9-9901-c86058546f21" />



## RESULT:
Thus, the program has been executed and verified successfully.

