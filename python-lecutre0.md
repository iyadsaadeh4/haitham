# Python

Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

It is used for:

web development (server-side),
software development,
mathematics,
system scripting.

## Setup

- [Python 3.9](https://www.python.org/downloads/)
- [vscode](https://code.visualstudio.com/download)

Extensions:

- Pylance
- Python

## Syntax

```python
print("Hello World!")
```

### Indentation

Correct:

```python
if 5 > 2:
  print("Five is greater than two!")

```

Error:

```python
if 5 > 2:
print("Five is greater than two!")
```

## Variables

A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume). Rules for Python variables:

- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and \_ )
- Variable names are case-sensitive (age, Age and AGE are three different variables)

In python, variables are created when when you assign a value ot it:

```python
x = 5
y = "Hello, World"
```

## Comments

```python
# This is a comment
print("Hello, World!")
```

## Data Types

In Python, the data type is set when you assign a value to a variable:

Example Data Type

```python

x = "Hello World" # str
x = 20 # int
x = 20.5 # float
x = 1j # complex
x = ["apple", "banana", "cherry"] # list
x = ("apple", "banana", "cherry") # tuple
x = range(6) # range
x = {"name" : "John", "age" : 36} # dict
x = {"apple", "banana", "cherry"} # set
x = frozenset({"apple", "banana", "cherry"}) # frozenset
x = True # bool
x = b"Hello" # bytes
x = bytearray(5) # bytearray
x = memoryview(bytes(5)) # memoryview
x = None # NoneType
```

## Control flow

### If statement

```python
a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
```

### Loops

```python
# While loop
i = 1
while i < 6:
  print(i)
  i += 1

# While loop with break
i = 1
while i < 6:
  print(i)
  if i == 3:
    break
  i += 1

# For loop
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)

# For loop with continue
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    continue
  print(x)


# For range
# range(start, end - exclusive -, increment)
for x in range(2, 30, 3):
  print(x)
```

### Functions

A function is a block of code which only runs when it is called.

You can pass data, known as parameters, into a function.

A function can return data as a result.

```python
def my_function():
  print("Hello from a function")
```

### Lambdas

Syntax: `lambda arguments : expression`

```python
x = lambda a : a + 10
print(x(5))
```

### Classes

Python is an object oriented programming language.

Almost everything in Python is an object, with its properties and methods.

A Class is like an object constructor, or a "blueprint" for creating objects.

```python
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self):
    print("Hello my name is " + self.name)
p1 = Person("John", 36)

print(p1.name)
print(p1.age)
```

### Input

```python
username = input("Enter username:")
print("Username is: " + username)
```

## Practice

1. Write a program that asks the user how many Fibonnaci numbers to generate and then generates them. Take this opportunity to think about how you can use functions. Make sure to ask the user to enter the number of numbers in the sequence to generate.(Hint: The Fibonnaci seqence is a sequence of numbers where the next number in the sequence is the sum of the previous two numbers in the sequence. The sequence looks like this: 1, 1, 2, 3, 5, 8, 13, …)

2. Write a password generator in Python. Be creative with how you generate passwords - strong passwords have a mix of
   lowercase letters, uppercase letters, numbers, and symbols. The passwords should be random, generating a new password every
   time the user asks for a new password. Include your run-time code in a main method.
   Extra:
   Ask the user how strong they want their password to be. For weak passwords, pick a word or two from a list.
