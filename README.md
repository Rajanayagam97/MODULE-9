# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
```
class Generate:

def __init__(self, first,d,last):

    self.first = first
    
    self.d = d
    
    self.last=last

def Ap_generate(self):

    L=[i for i in range(self.first,self.last+1,self.d)]
    
    return L
Series = Generate(200,2,301)

print(Series.Ap_generate())
```
## OUTPUT:
<img width="1259" height="173" alt="491567558-1d2b3df9-08d6-4f93-b7a7-8ad7a82f8801" src="https://github.com/user-attachments/assets/0f828a0c-f54a-43f0-be8c-7cf87a40417a" />


## RESULT:
the program is excuted and verified.
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
# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
```
rows=int(input())

columns=int(input())

matrix=[[0]*columns for row in range(rows)]

for i in range(rows):

lines=list(map(int, input().split()))

for j in range(columns):

    matrix[i][j]=lines[j]
print(matrix)

for i in range(rows):

for j in range(columns):

    if(i==j):
    
        print(matrix[i][j],end=" ")
   
    else:
    
        print(' ',end=" ")

print()
```
### Output:
<img width="961" height="399" alt="491570374-00f675e8-531b-4bad-bcb1-3af7f88ce425" src="https://github.com/user-attachments/assets/5ac72d60-3b09-4b30-bd58-773816840a25" />

## Result
The program is excuted and verified
