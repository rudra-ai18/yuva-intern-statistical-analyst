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
