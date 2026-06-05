## EX 1: Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
```python3
dict1 = eval(input())
dict2 = eval(input())
dict2.update(dict1)
print(dict2)
```

## Output
<img width="1193" height="858" alt="image" src="https://github.com/user-attachments/assets/46799e5e-2409-4bcb-8d46-7bc2e5a05935" />

## Result
Thus the python program that merges **two dictionaries** and combines their key-value pairs is completed successfully.
<br>
<br>
# EX 2: Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
```python3
key_value = eval(input())

kv = sorted(key_value.items())

print("Keys and Values sorted in alphabetical order by the key")

for i in kv:
    print(i, end=" ")
```

## Sample Output
<img width="1184" height="748" alt="image" src="https://github.com/user-attachments/assets/646e3ec9-9c82-4cd5-a3d3-cd8d6f8f6c43" />

## Result

Thus the python program to sort a dictionary and print is completed successfully.



<br>
<br>

# EX 3: Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
```python3
try:
    n=int(input())
    l=[]
    for i in range(n):
        l.append(int(input()))
    print(l)
    print(l[6])
except IndexError:
    print("6 is not accepted")
```

## Output
<img width="1543" height="854" alt="image" src="https://github.com/user-attachments/assets/87e77317-f328-4ba8-92d3-cc06eec4809d" />

## Result
Thus the python program that handles an **IndexError** when trying to access an element beyond the available range of a list is completed successfully.






<br>
<br>
---

# EX 4: Python Script to Reverse File Contents and Save to Another File

## 🎯 Aim
To write a Python program that reverses the contents of a file and saves the reversed content into another file.

## 🧠 Algorithm
1. Create a function `create_file(file_path, content)` to write the given content into a file.  
2. Create a function `reverse_file_content(input_file_path, output_file_path)` to:  
   - Read the content of the input file.  
   - Reverse the content using slicing (`[::-1]`).  
   - Write the reversed content into the output file.  
3. Create a function `read_file(output_file_path)` to read and return the content of the output file.  
4. Get input content from the user, create the input file, reverse its content, and display the reversed result.  

## 🧾 Program
```python
def create_file(file_path, content):
    with open(file_path, 'w') as file:
        file.write(content)

def reverse_file_content(input_file_path, output_file_path):
    with open(input_file_path, 'r') as file:
        content = file.read()
    revcont = content[::-1]
    with open(output_file_path, 'w') as file:
        file.write(revcont)

def read_file(output_file_path):
    with open(output_file_path, 'r') as file:
        content = file.read()
        return content

# Example usage
input_file_path = 'test_case_1.txt'
output_file_path = 'reversed_1.txt'
file_content = input("Enter file content: ")
create_file(input_file_path, file_content)
reverse_file_content(input_file_path, output_file_path)
print(read_file(output_file_path))
```

## 🖥️ Example Output
<img width="1545" height="827" alt="image" src="https://github.com/user-attachments/assets/57c5d7e3-37f4-4165-aace-b13445bb264b" />



## ✅ Result
Thus, the program has been successfully executed to reverse the contents of a file and save it to another file.

---






<br>
<br>

# EX 5: Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `Circle` and a method `area` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program

```python3
import math
class Circle:
    def __init__(self,radius):
        self.radius=radius
    def area(self):
        return math.pi *self.radius*self.radius
r=float(input())        
C=Circle(r)        
print("Area of circle: {:.2f}".format(C.area()))
    
```
## Output
<img width="1362" height="804" alt="image" src="https://github.com/user-attachments/assets/c78e47ae-9611-4319-9062-aaa5ec856a06" />

## Result
Thus the python  program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `Circle` and a method `area` to perform the calculation is completed successfully.
