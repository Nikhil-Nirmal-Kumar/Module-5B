# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd 
student_data1 = pd.DataFrame({ 'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'], 'name': ['Danniella Fenton', 'Ryder Storey', 'Bryce Jensen', 'Ed Bernal', 'Kwame Morin'],  'marks': [200, 210, 190, 222, 199]}) 
student_data2 = pd.DataFrame({ 'student_id': ['S4', 'S5', 'S6', 'S7', 'S8'], 'name': ['Scarlette Fisher', 'Carla Williamson', 'Dante Morse', 'Kaiser William', 'Madeeha Preston'], 'marks': [201, 200, 198, 219, 201]}) 
print("Original DataFrames:") 
print(student_data1)
print("-------------------------------------") 
print(student_data2) 
print("\nJoin the said two dataframes along rows:") 
result_data = pd.concat([student_data1, student_data2]) 
print(result_data)
```

## Output
<img width="828" height="602" alt="image" src="https://github.com/user-attachments/assets/fac12be2-153d-4382-adfd-72219259ea80" />
<img width="835" height="444" alt="image" src="https://github.com/user-attachments/assets/ba9d35f9-eb95-4c7b-9248-935d6d17e21e" />

## Result
