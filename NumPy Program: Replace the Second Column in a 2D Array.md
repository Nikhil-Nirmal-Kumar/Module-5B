# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np
A = np.array(eval(input()))
b=eval(input())
c=[]
for i in b[0]:
    c.append([i])
new_col = np.array(c)
print("Printing Original array")
print(A)
A_deleted = np.delete(A, 1, axis=1)
print("Array after deleting column 2 on axis 1")
print(A_deleted)
A_inserted = np.insert(A_deleted, 1, new_col.T, axis=1)
print("Array after inserting column 2 on axis 1")
print(A_inserted)
```

## Output
<img width="1143" height="686" alt="image" src="https://github.com/user-attachments/assets/b69cdbe7-da6d-4530-a45f-7f170617d7ae" />

## Result
