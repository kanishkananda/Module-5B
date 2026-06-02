## Python Programming Module 5
## Name: Kanishka.N
## Register Number: 212225230127
## Ex:1 NumPy Program: Column-wise Sorting of a 2D Array
## 🎯 Aim
To write a NumPy program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm
1. Import NumPy: Start by importing the NumPy library.
2. Get Input: Accept a 2D NumPy array from the user.
3. Sort Column-wise: Use the np.sort() function with axis=0 to sort each column in ascending order.
4. Store Result: Store the sorted result in a new array.
5. Display Output: Print the original array and the column-wise sorted array.
## 🧾 Program:
```
import numpy as np
l=eval(input("Enter the array: "))
a=np.array(l)
print("Given Array: ")
print(f"{a}")

print(f"Sorted array: \n{np.sort(a,axis=0)}")
```
## Output
<img width="671" height="386" alt="image" src="https://github.com/user-attachments/assets/6c96831a-e3ab-4330-8ef0-afc72df79a99" />

## Result:
Thus the NumPy program that sorts the elements in each column of a given 2D array in ascending order is executed successfully.

## Ex:2 NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y
## 🎯 Aim
To write a Python program using NumPy that finds the indices where elements in array x are greater than or equal to their corresponding elements in array y.

## 🧠 Algorithm
1. Import NumPy: Import the NumPy library.
2. Define Arrays: Define two NumPy arrays, x and y, with the same shape (i.e., same number of elements).
3. Use Boolean Indexing:
      -x > y gives a boolean array where elements of x are greater than y.
      -x == y gives a boolean array where elements of x are equal to y.
4. Find Indices: Use np.where() to get the indices where the conditions x >= y are satisfied.
5. Print Indices: Print the indices where the condition holds true.
## 🧾 Program:
```
import numpy as np  
x=eval(input("Enter the First array: ")) 
y=eval(input("Enter the Second array: ")) 
l1=np.array(x) 
l2=np.array(y) 
print()
print(np.where(l1>l2)) 
print(np.where(l1==l2))
```
## Output:
<img width="631" height="309" alt="image" src="https://github.com/user-attachments/assets/e8192bb1-59cb-45fc-bb66-bf61bb4f3da8" />

## Result
Thus the Python program using NumPy that finds the indices where elements in array x are greater than or equal to their corresponding elements in array y.

## Ex:3 NumPy Program: Replace the Second Column in a 2D Array
## 🎯 Aim
To write a NumPy program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. Import NumPy: Start by importing the NumPy library.
2. Get Input: Get a 2D NumPy array and a new column (as another array) from the user.
3. Delete Column: Use np.delete() to remove the second column (index 1) from the original array.
4. Insert Column: Use np.insert() to insert the new column at the second column's original position.
5. Display Result: Print the updated array with the replaced column.
## 🧾 Program
```
import numpy as np
orig=np.array(eval(input("Enter the Original array: ")))
new=np.array(eval(input("Enter the new column: ")))
print("Printing Original array")
print(orig)
modif=np.delete(orig,1,axis=1)
print("Array after deleting column 2 on axis 1")
print(modif)
result=np.insert(modif,1,new,axis=1)
print("Array after inserting column 2 on axis 1")
print(result)
```
## Output:
<img width="744" height="584" alt="image" src="https://github.com/user-attachments/assets/e622116a-6e58-4835-9d22-920ba745ceb5" />

## Result:
Thus the NumPy program that deletes the second column from a given 2D array and inserts a new column at the same position is executed successfully.

## Ex:4 Pandas Program: Create and Display a DataFrame with Custom Index Labels
## 🎯 Aim
To create and display a DataFrame using the Pandas library in Python from a given dictionary, and apply specific index labels to the rows.

## 🧠 Algorithm
1. Import Libraries: Import the required libraries – pandas and numpy.
2. Create Dictionary: Define a dictionary exam_data with keys: 'name', 'score', 'attempts', and 'qualify'.
3. Index Labels: Create a list of custom index labels called labels.
4. Create DataFrame: Use pd.DataFrame() to create the DataFrame by passing the dictionary and index labels.
5. Display Output: Display the DataFrame using print() or by simply calling the DataFrame variable.
## 💻 Program
```
import pandas as pd 
import numpy as np 
exam_data  = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 
'Kevin', 'Jonas'], 
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19], 
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1], 
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']} 
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j'] 
df = pd.DataFrame(exam_data , index=labels) 
print(df)
```
## Output:
<img width="754" height="508" alt="image" src="https://github.com/user-attachments/assets/fde5ec6f-29a5-493b-acb1-15918348eccc" />

## Result:
Thus the program to create and display a DataFrame using the Pandas library in Python from a given dictionary, and apply specific index labels to the rows is executed successfully.

## Ex:5 Pandas Program: Join Two DataFrames Along Rows
## 🎯 AIM
To write a Python program using Pandas to join two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame.

## 🧠 ALGORITHM
1. Import Libraries: Import the pandas library.
2. Create First DataFrame: Use a dictionary to create student_data1.
3. Create Second DataFrame: Use another dictionary to create student_data2.
4. Concatenate DataFrames: Use pd.concat() with axis=0 to concatenate both DataFrames row-wise.
5. Display Result: Print the new combined DataFrame.
## 💻 Program
```
import pandas as pd
a=eval(input("Enter the dataset1 :"))
b=eval(input("Enter the dataset2 :"))
df1=pd.DataFrame(a)
df2=pd.DataFrame(b)
print("\n")
print("Original DataFrames:")
print(df1)
print("-"*20)
print(df2)
print()
mer=pd.concat([df1,df2])
print("Join the said two dataframes along rows:")
print(mer)
```
## Output
<img width="767" height="735" alt="image" src="https://github.com/user-attachments/assets/1e492b1c-e794-4a2e-9499-25dccd1ee37b" />

## Result:
Thus the Python program using Pandas to join two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame is executed successfully.

