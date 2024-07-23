# Basics

Here are the names of the common brackets and punctuation marks used in programming:

```python

Parentheses: ()
Curly braces: {}
Square brackets: []
Angle brackets: <>
Single quotes: ' '
Double quotes: " "
Backtick: `
Semicolon: ;
Colon: :
Comma: ,
Period: .
Question mark: ?
Exclamation mark: !
Ampersand: &
Asterisk: *
Plus sign: +
Minus sign: -
Forward slash: /
Backward slash: \
Percent sign: %
Caret: ^
Tilde: ~
Pipe: |
Equals sign: =
Less than sign: <
Greater than sign: >
Underscore: _
Hyphen: -
pound sign or hash: #
```

## **Data Types:**

```python
**# Integer data type
x = 5
y = 10
print(x + y)  # Output: 15

# Floating-point data type
a = 2.5
b = 3.75
print(a * b)  # Output: 9.375

# String data type
name = "John Doe"
print("Hello, " + name)  # Output: Hello, John Doe

# Boolean data type
is_sunny = True
is_raining = False
print(is_sunny and not is_raining)  # Output: True**
```

## **Data Structures:**

```python
# List data structure
fruits = ["apple", "banana", "cherry", "orange"]
print(fruits[1])  # Output: banana
fruits.append("pear")
print(fruits)  # Output: ['apple', 'banana', 'cherry', 'orange', 'pear']

# Dictionary data structure
person = {"name": "John Doe", "age": 30, "city": "New York"}
print(person["age"])  # Output: 30
person["occupation"] = "Engineer"
print(person)  # Output: {'name': 'John Doe', 'age': 30, 'city': 'New York', 'occupation': 'Engineer'}

# Tuple data structure
colors = ("red", "green", "blue")
print(colors[0])  # Output: red
# colors[0] = "orange"   # Raises a TypeError because tuples are immutable

# Set data structure
numbers = {1, 2, 3, 4, 5}
print(3 in numbers)  # Output: True
numbers.add(6)
print(numbers)  # Output: {1, 2, 3, 4, 5, 6}
```