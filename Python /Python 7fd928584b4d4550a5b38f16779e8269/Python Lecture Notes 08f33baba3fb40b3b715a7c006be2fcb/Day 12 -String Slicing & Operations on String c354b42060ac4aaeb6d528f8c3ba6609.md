# Day 12 -String Slicing & Operations on String

# Length of a String

We can find the length of a string using **len()** function.

## Example:

```python
fruit = "Mango"
len1 = len(fruit)
print("Mango is a", len1, "letter word.")

```

## Output:

```python
Mango is a 5 letter word.
```

# String as an array

A string is essentially a sequence of characters also called an array. Thus we can access the elements of this array.

## Example:

```
pie = "ApplePie"
print(pie[:5])
print(pie[6])	#returns character at specified index

```

## Output:

```
Apple
i

```

Note: This method of specifying the start and end index to specify a part of a string is called slicing.

## Slicing Example:

```python
pie = "ApplePie"
print(pie[:5])      #Slicing from Start
print(pie[5:])      #Slicing till End
print(pie[2:6])     #Slicing in between
print(pie[-8:])     #Slicing using negative index

```

## Output:

```
Apple
Pie
pleP
ApplePie

```

# Loop through a String:

Strings are arrays and arrays are iterable. Thus we can loop through strings.

## Example:

```python
alphabets = "ABCDE"
for i in alphabets:
    print(i)

```

## Output:

```
A
B
C
D
E

```

![Untitled](Day%2012%20-String%20Slicing%20&%20Operations%20on%20String%20c354b42060ac4aaeb6d528f8c3ba6609/Untitled.png)

## Coding:

```python
fruit = "Mango"
mangoLen = len(fruit)
print(mangoLen)
# print(fruit[0:4]) # including 0 but not 4
# print(fruit[1:4]) # including 1 but not 4
# print(fruit[:5])
# print(fruit[0:-3])
# print(fruit[:len(fruit)-3])
print(fruit[-1:len(fruit) - 3])
print(fruit[-3:-1])

# Quick Quiz:
# nm = "Happy"
# print(nm[-4:-2])

```