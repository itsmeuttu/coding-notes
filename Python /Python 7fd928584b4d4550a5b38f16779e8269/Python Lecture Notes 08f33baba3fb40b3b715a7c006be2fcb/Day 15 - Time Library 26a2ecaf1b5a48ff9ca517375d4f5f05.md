# Day 15 - Time Library

The **`time`** module in Python provides various functions to work with time-related tasks. The **`time`** module provides time-related functions like getting the current time, formatting time, converting time, and sleeping.

Here are some of the commonly used functions in the **`time`** module:

1. **`time()`**: This function returns the current time in seconds since the epoch (January 1, 1970, 00:00:00 UTC).

Example:

```python
import time

current_time = time.time()
print("Current time:", current_time)
```

Output:

```python
Current time: 1648794649.727663
```

1. **`sleep()`**: This function suspends the execution of the current thread for a given number of seconds.

Example:

```python
import time

print("Before sleep")
time.sleep(5)
print("After sleep")
```

Output:

```python
Before sleep
After sleep

Note that the program will sleep for 5 seconds before executing the next line.
```

1. **`asctime()`**: This function takes a time tuple as an argument and returns a string representing the time in a readable format.

Example:

```python
import time

current_time = time.localtime()

readable_time = time.asctime(current_time)
print("Readable time:", readable_time)
```

Output:

```python
Readable time: Tue Mar 30 14:17:56 2023
Note that the localtime() function is used to get the current time as a time tuple.
```

1. **`strftime()`**: This function takes a time tuple or struct_time object as an argument and returns a string representing the time in a specified format.

Example:

```python
import time

current_time = time.localtime()

formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", current_time)
print("Formatted time:", formatted_time)
```

Output:

```python
Formatted time: 2023-03-30 14:21:33
In this example, 
the strftime() function is used to format the current time in a specific format.
```

## Quiz

Create a python program capable of greeting you with Good Morning, Good Afternoon and Good Evening. Your program should use time module to get the current hour. Here is a sample program and documentation link for you:

```python

```