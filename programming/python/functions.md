---
layout: page
title: Writing your own functions
---

Writing your own functions
==========================

Python allows you to group useful code that you're going to use over and over again into what's called a *function*.
You might want to write a function that handles all the behaviour of your robot once it's got the info back from the vision system,
 or perhaps something much smaller like a precise left turn.


A simple function that calculates the square of a number:

~~~~~ python
def square(num):
    return num ** 2
~~~~~

This would be used by some other code as follows:

~~~~~ python
sq = square(5)
print(sq)  # prints: 25
~~~~~

Another advantage of grouping your code like this is that if you decide you change the way that it works slightly,
 (but still having it return the same answer) you can do this easily,
 and the changed code will be used throughout your code, without having to change it in many, many places:

The same function modified & printing a log message:

~~~~~ python
def square(num):
    print(f"found the square of {num}")
    return num * num
~~~~~
