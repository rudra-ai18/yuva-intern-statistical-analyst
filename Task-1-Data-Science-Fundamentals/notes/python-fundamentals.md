# Python Fundamentals

## Day 3 — Python Basics

### 1. Variables

A variable is a name used to store a value.

```python
name = "Rudra"
age = 21
height = 6.3
is_student = True
```

### 2. Basic Data Types

- **int:** whole numbers, e.g. `21`
- **float:** decimal numbers, e.g. `6.3`
- **str:** text, e.g. `"Rudra"`
- **bool:** `True` or `False`

The `type()` function can be used to check the data type.

```python
age = 21
print(type(age))
```

### 3. Input and Output

Use `print()` to display output.

```python
print("Hello Rudra")
```

Use `input()` to take user input.

```python
name = input("Enter your name: ")
print(name)
```

By default, `input()` returns a string.

### 4. Type Conversion

Type conversion changes a value from one data type to another.

```python
x = "100"
x = int(x)

price = "10.5"
price = float(price)

number = 100
text = str(number)
```

Common conversions include `int()`, `float()`, and `str()`.

### 5. Operators

#### Arithmetic Operators

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

- `+` addition
- `-` subtraction
- `*` multiplication
- `/` division
- `//` floor division
- `%` remainder
- `**` power

#### Comparison Operators

```python
a = 10
b = 5

print(a > b)
print(a < b)
print(a == b)
print(a != b)
```

Comparison results are Boolean values: `True` or `False`.

#### Logical Operators

- `and`
- `or`
- `not`

Example:

```python
age = 21
student = True

print(age > 18 and student)
```

## Practice Completed

The Day 3 practice focuses on:
- Storing student information using variables
- Building a basic calculator
- Calculating age from birth year
- Calculating total and average marks
- Identifying Python data types

## Key Takeaway

Python fundamentals provide the base for later work with data analysis libraries such as NumPy and Pandas. Understanding variables, data types, input/output, type conversion, and operators is essential before moving to conditions, loops, functions, and data structures.

---

**Day 3 Status: Complete ✅**


## Day 4 — Conditions and Loops

### 1. if Statement

The `if` statement runs a block of code when a condition is true.

```python
age = 21

if age >= 18:
    print("Adult")
```

Python uses indentation to define the block of code.

### 2. if / else

Use `else` when there are two possible outcomes.

```python
age = 16

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

### 3. if / elif / else

Use `elif` when multiple conditions need to be checked.

```python
marks = 75

if marks >= 90:
    print("A")
elif marks >= 75:
    print("B")
elif marks >= 60:
    print("C")
else:
    print("D")
```

Conditions are checked from top to bottom.

### 4. for Loop

A `for` loop is used to repeat an action for a sequence or a range of values.

```python
for i in range(5):
    print(i)
```

Output:

```text
0
1
2
3
4
```

### 5. range()

Common forms:

```python
range(5)          # 0, 1, 2, 3, 4
range(2, 6)       # 2, 3, 4, 5
range(1, 10, 2)   # 1, 3, 5, 7, 9
```

The stop value is not included.

### 6. while Loop

A `while` loop repeats as long as its condition is true.

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

The condition should eventually become false to avoid an infinite loop.

### 7. break

`break` immediately stops the loop.

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

### 8. continue

`continue` skips the current iteration and moves to the next one.

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

### Real-World Data Example

Conditions can be used to classify values.

```python
spending = 15000

if spending >= 10000:
    print("High-value customer")
else:
    print("Regular customer")
```

### Key Takeaway

**Condition = decision**

**Loop = repetition**

The main concepts learned today are `if`, `if/else`, `if/elif/else`, `for`, `range()`, `while`, `break`, and `continue`.

---

**Day 4 Status: Complete ✅**


## Day 5 — Data Structures & File Handling

### 1. Lists

A list stores multiple values in an ordered and changeable collection.

```python
marks = [78, 85, 65, 92]
print(marks[0])
print(marks[-1])

marks[0] = 80
marks.append(88)
marks.remove(65)

print(len(marks))

for mark in marks:
    print(mark)
```

Lists use zero-based indexing, so the first item is at index 0.

### 2. List Slicing

Slicing selects part of a list.

```python
marks = [78, 85, 65, 92, 88]
print(marks[1:4])
```

The stop index is not included.

### 3. Tuples

A tuple is an ordered collection whose elements cannot be changed after creation.

```python
coordinates = (27.17, 78.01)
print(coordinates[0])
```

**List = changeable**

**Tuple = fixed**

### 4. Dictionaries

A dictionary stores data as key-value pairs.

```python
student = {
    "name": "Rudra",
    "age": 21,
    "city": "Agra",
    "marks": 85
}

print(student["name"])
print(student["marks"])

student["marks"] = 90
student["course"] = "Data Science"
```

Dictionaries are useful when different pieces of information need meaningful keys.

### 5. Sets

A set stores unique values.

```python
numbers = {1, 2, 3, 3, 4}
print(numbers)
```

Duplicate values are automatically removed.

Sets are useful when only unique values are needed.

### 6. File Handling

Files can be opened in different modes, including read (`r`), write (`w`), and append (`a`).

#### Reading

```python
with open("data.txt", "r") as file:
    content = file.read()

print(content)
```

#### Writing

```python
with open("notes.txt", "w") as file:
    file.write("I am learning Python.")
```

#### Appending

```python
with open("notes.txt", "a") as file:
    file.write("\nDay 5 completed.")
```

Using `with open()` helps ensure the file is properly closed.

### Data Structure Comparison

| Structure | Syntax | Main Characteristic |
|---|---|---|
| List | `[]` | Ordered and changeable |
| Tuple | `()` | Ordered and fixed |
| Dictionary | `{}` | Key-value pairs |
| Set | `{}` | Unique values |

### Key Takeaway

Data structures help organize information in Python. Lists are useful for ordered collections that may change, tuples are useful for fixed collections, dictionaries represent key-value information, and sets handle unique values. File handling allows Python programs to read and write data stored outside the program.

---

**Day 5 Status: Complete ✅**
