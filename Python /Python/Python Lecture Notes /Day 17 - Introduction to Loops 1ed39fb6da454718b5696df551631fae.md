# Day 17 - Introduction to Loops

Sometimes a programmer wants to execute a group of statements a certain number of times. This can be done using loops. Based on this loops are further classified into following main types;

- for loop
- while loop

# The for Loop

for loops can iterate over a sequence of iterable objects in python. Iterating over a sequence is nothing but iterating over strings, lists, tuples, sets and dictionaries.

## Example: iterating over a string:

```
name = 'Abhishek'
for i in name:
    print(i, end=", ")

```

## Output:

A, b, h, i, s, h, e, k,

## Example: iterating over a list:

```python
colors = ["Red", "Green", "Blue", "Yellow"]
for x in colors:
    print(x)

```

## Output:

```python
Red
Green
Blue
Yellow
```

Similarly, we can use loops for lists, sets and dictionaries.

## range():

What if we do not want to iterate over a sequence? What if we want to use for loop for a specific number of times?

Here, we can use the range() function.

## Example:

```python
for k in range(5):
    print(k)

```

## Output:

```python
0
1
2
3
4
Here, we can see that the loop starts from 0 by default and increments at each iteration.
But we can also loop over a specific range.
```

## Example:

```
for k in range(4,9):
    print(k)

```

## Output:

```python
4
5
6
7
8
```

## About third parameter of range (ie range(x, y, z))

```python
for i in range(1, 8, 2):

 print(i)
```

```python
Output:
1
3
5
7

```

### Explanation:

This code will generate a sequence of numbers starting from 1 (inclusive) up to 8 (exclusive), incrementing by 2 at each step.

When the code runs, the loop will iterate over this sequence, and the variable **`i`** will take on each value in the sequence in turn.

In the first iteration, **`i`**
 will be equal to 1, so the **`print(i)`**
 statement will output 1. In the second iteration, **`i`**
 will be equal to 3, so the **`print(i)`**
 statement will output 3, and so on, until the loop has iterated over all the values in the sequence.

## Another Example:

```python
for i in range(1, 5, 8):
    print(i)
```

### output:

```python
1
```

### Explanation:

The **`range()`** function generates a sequence of numbers, starting from the first argument (inclusive) up to the second argument (exclusive), incrementing by the third argument.

In this code, the **`range(1, 5, 8)`** function generates a sequence of numbers starting from 1 (inclusive) up to 5 (exclusive), incrementing by 8. However, since the increment is greater than the distance between the start and end of the sequence, the **`range()`** function will only generate the first number, 1.

Therefore, when the code runs, it will print the number 1 once, and then exit the loop since there are no more elements in the range sequence.

![Untitled](Day%2017%20-%20Introduction%20to%20Loops%201ed39fb6da454718b5696df551631fae/Untitled.png)

![Untitled](Day%2017%20-%20Introduction%20to%20Loops%201ed39fb6da454718b5696df551631fae/Untitled%201.png)

## Question Practise:

**Q1.**  Write a for loop that prints the even numbers from 2 to 10.

Sol: 

```python
for i in range(2,11,2):
	print(i)
```

output:

```python
2
4
6
8
10
```

**Q2**. 1. Write a for loop that iterates over a list of strings and prints each string in uppercase.

Sol:

```python
list = ['Death Note', 'Demon Slayer', ' Dr. Stone']
for i in  list:
	print(i.upper())
```

Output:

```python
DEATH NOTE
DEMON SLAYER
 DR. STONE
```

**Q3**. Write a for loop that calculates the sum of all the numbers in a list.

```python
list =[ 4, 5, 6, 8, 9 ]
a = 0
for i in list:
	a = a + i
print(a)
```

Output:

```python
32
```

**Q4.** Write a for loop that calculates the factorial of a given number.

```python
n = int(input("Enter your Number: "))
x = 1
for i in range(1,n+1):
	x = x * i
print("The factoria of" , n , "is" ,x)
```

Output:

120

**Q5.** Write a for loop that prints the multiplication table of a given number.

```python
n = int(input("Enter your number: "))
for i in range(1,11):
    print(n, 'X',i, '=', n*i)
```

Output:

```python
Enter No : 6
6 X 1 = 6
6 X 2 = 12
6 X 3 = 18
6 X 5 = 30
6 X 6 = 36
6 X 7 = 42
6 X 8 = 48
6 X 9 = 54
6 X 10 = 60
```