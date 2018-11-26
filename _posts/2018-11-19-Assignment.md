---
layout: post
title: Understading Python Assignment
---

The assignment in Python is different from C/C++, in C/C++,
the below code means allocate 4 bytes memory on the stack to store
an integer varaible.

```c
int a = 1;
```

However everything in Python is an object. The below code in Python
means create a integer object in memory and label it with a variable
called a. You can think of a as a pointer which points to the integer object.

```python
a = 1
```

What happens when you modify a variable? It depends on the type of the
variable. It is worth noting that Python is a strongly typed language.
Different from
statically typed language, Python is dynamically-typed language.
If the type is immutatble, like int, float, string, tuple etc. Changing
a variable will **create a new object** and label it with the variable.


```python
a = 1
a += 1 # create a new integer object with value 2 and label it with variable a
```

If the type is mutable, changing a variable will **change the object it points
to**. Check the below example.

```python
lst = []
print(id(lst))
lst.append(1)
print(id(lst)) # the output is same as the output of second line
```
