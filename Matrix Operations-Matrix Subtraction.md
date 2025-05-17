# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:
```
def read_matrix(rows, cols, name):
    print(f"\nEnter elements of {name}:")
    matrix = []
    for i in range(rows):
        row = list(map(int, input(f"Row {i + 1}: ").split()))
        if len(row) != cols:
            raise ValueError("Incorrect number of columns.")
        matrix.append(row)
    return matrix
def subtract_matrices(matrix1, matrix2):
    result = []
    for i in range(len(matrix1)):
        row = []
        for j in range(len(matrix1[0])):
```
## OUTPUT:
```
Input             Result
2                Enter elements of Matrix A:
3                5 7 9
                 4 6 8
                 Enter elements of Matrix B:
                 1 2 3
                 1 1 1
---------------------------------------------------------------
```
## RESULT:
The program was successful.

