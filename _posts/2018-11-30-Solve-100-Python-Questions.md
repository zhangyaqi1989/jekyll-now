---
layout: post
title: Solve 100 Python Questions
---
## Question 1 (Level 1)
Write a program which will find all such numbers which are
divisible by 7 but are not a multiple of 5, between 2000
and 3200 (both included). The numbers obtained should be
printed in a comma-separated sequence on a single line.

```python
nums = [num for num in range(2000, 3200 + 1) if num % 7 == 0 and num % 5 != 0]
print(','.join(map(str, nums)))
```


## Question 2 (Level 1)
Write a program which can compute the factorial of a given numbers.
The results should be printed in a comma-separated sequence on a single line.
Suppose the following input is supplied to the program:
8
Then, the output should be:
40320

```python
import math
n = 8
print(math.factorial(n))
```


## Question 3 (Level 1)
With a given integral number n, write a program to generate a dictionary that contains (i, i*i) such that is an integral number between 1 and n (both included). and then the program should print the dictionary.
Suppose the following input is supplied to the program:
8
Then, the output should be:
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}

```python
n = 8
dic = {x : x * x for x in range(1, n + 1)}
print(dic)
```


## Question 4 (Level 1)
Write a program which accepts a sequence of comma-separated numbers from console and generate a list and a tuple which contains every number.
Suppose the following input is supplied to the program:
34,67,55,33,12,98
Then, the output should be:
['34', '67', '55', '33', '12', '98']
('34', '67', '55', '33', '12', '98')

```python
# s = input()
s = "34,67,55,33,12,98"
print(list(map(str, s.split(','))))
print(tuple(map(str, s.split(','))))
```


## Question 5 (Level 1)
Define a class which has at least two methods:
getString: to get a string from console input
printString: to print the string in upper case.
Also please include simple test function to test the class methods.

```python
class Soln():
    def __init__(self):
        self.string = ""
    def getString(self):
        self.string = input()
    def printString(self):
        print(self.string)
soln = Soln()
soln.getString()
soln.printString()
```


