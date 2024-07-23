# Day 19 - Break and Continuity

# break statement

The break statement enables a program to skip over a part of the code. A break statement terminates the very loop it lies within.

## example

```python
for i in range(1,101,1):
    print(i ,end=" ")
    if(i==50):
        break
    else:
        print("Mississippi")
print("Thank you")

```

### output

```
1 Mississippi
2 Mississippi
3 Mississippi
4 Mississippi
5 Mississippi
.
.
.
50 Thank you

```

## Continue Statement

The continue statement skips the rest of the loop statements and causes the next iteration to occur.

## example

```python
for i in [2,3,4,6,8,0]:
    if (i%2!=0):
        continue
    print(i)

```

## output

```
2
4
6
8
0

```

## Short trick:

```python
break:  Loop ko chod ke chla jyega
continue: itriation ko chod ke nikal jyega
```

continue and break are used to alter the normal flow of a loop in Python. However, the key difference is that continue skips the remaining code for the current iteration and proceeds to the next iteration, while break terminates the entire loop immediately. In this particular example, where we are printing numbers from 1 to 10 and skipping even numbers, the output is the same for both continue and break. But in other scenarios, the difference between continue and break can affect the behavior of the loop.