## Python Data Types
***

Objectives
By the end of this lesson, you will be able to:

* Identify the type of data
* Identify a string
* Identify an integer
* Identify a boolean

## Different data types

***

While the focus of this module is the **list** `list` data type, in this lesson we will take a brief look at the different types of data that can make up a list. We will learn about the differences and some of the characteristics of these other types of data.

## String `str`

***

The first type of data we will look at is the **string** `str`. A lot of information in the world is in the form of text. To capture this information and operate on it in Python we take this text and make it into the **string** `str` data type. Below, we have the name of a city, . By putting quotes ("") or ('') around the name, we create a string. It would look like this:  

```
"Buenos Aires"
```

When programmers say string, what they mean is text. When programmers say data type, they just mean type of data. We can think of "Buenos Aires" as an instance of the string data type.  Below are a few examples of stings:

```python
"Oaxaca"
'Puerta Vallarta'
'Rome"
"My favorite city to visit is Juno, Alaska"
```

## Integer `int`

***

In our Data Science program, you will certainly be using numbers in many different ways during your journey, and the **integer** `int` is one form of number we use in python. An integer is simply a whole number, it can be positive or negative but it is a whole number without a decimal point.  When we use integers in Python it is important to note that any mathmatical operation with intgers will only return integers. Examples of integers are:

```
73
186282
-87
0
```

Unlike a **string**, the **integer** `int` data type does not need quotes around it.  If it is enclosed in quotes, it becomes a `str` and it cannot be used in mathmatical operations unless it is converted back to a float.

## Floats `float`

***

We know that math is not always clean cut, and many times we need more accurate numbers, so we need to use decimals to increase our accuracy, in Python we call these numbers with decimals, a **float** `float`.  A **float** `float` is any number that has a decimal in it. If we combine integers and floats in a mathematical operation, we will get a float as the result, always. Additionally, just like an integer, a float does not need any quotes, and if you do put it in quotes, it becomes a 88string. Some examples of floats are:

```
1.618
2.0
2.71828
-0.5
6.626068
0.1
3.14159
```

## Boolean `bool`

***

What is a **Boolean**?
A **Boolean** `bool` has two possible values: `True` or `False`.
It's fairly rare for programmers to explicitly write the word True or False. Instead our programs can respond to questions for us with a boolean and use this result to choose which path the program takes.

```python
5 == 5  # True
5 == 2  # False
2 + 2 == 4  # True
2.0 == 2   # True
```

## The `type()` function

***

Now that we know that there are many different data types, lets explore one way we can check the type of data we have.  We can check the data we have with the `type()` function. To check the type of data, we can simply pass the data as an argument to the `type()` function. For example, if we wanted to find out what type of data `Toronto` is we would do it like this:

```
type('Toronto')
```
Or, if we were to assign 'Toronto' to a variable it would look like this:

```python
city = 'Toronto'

type(city)
```

## Recap

***

Excellent, now that we have a little understanding of a few of the types of data python uses, we can begin to put it to work and see how we can use this information.


