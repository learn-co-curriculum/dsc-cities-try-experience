# Python Data Types

## Objectives for this lesson

***

By the end of this lesson, you will be able to:

* Identify the type of data
* Identify a string
* Identify an integer
* Identify a float
* Identify a boolean

## Different data types

***

While the focus of this short course is the `list` data type, in this lesson we will take a brief look at the different types of data that can make up a list (a list, as you'll see later, is in fact a _compound_ data type). You'll learn about the differences and some of the characteristics of these types of data. In this lesson we will simply introduce the different data types but you will dive deeper into each one as they are introduced in the following lessons.

## The `str` data type

***

The first type of data is the **string** or `str`. A lot of information in the world is in the form of text. To capture this information and operate on it in Python we take this text and make it into the `str` data type. Let's take a look at how this can be done in Python. 

Below, you can see name of a city. By putting double quotes ("") or single quotes ('') around the name, we create a **string**. Double quotes ("") or single quotes ('') can be used interchangeably, but we will cover that a little later in the course.  If you wanted to create a `str` from the city name *Buenos Aires* in Python, it would look like this:  

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

## The `int` data type

***

In our Data Science program, you will certainly be using numbers in many different ways during your journey, and the **integer** or `int` is one type of number we use in Python. 

An `int` is simply a whole number, it can be positive or negative but it is a whole number without a decimal point.  When using integers in Python, it is important to note that any mathematical operation with integers will only return integers. Examples of `int` are:

```
73
186282
-87
0
```

Unlike a `str`, the `int` data type does not need quotes around it.  If it is enclosed in quotes, it becomes a `str` and it cannot be used in mathematical operations, however, if necessary a `str` can be converted to a `int`.

## The float data type

***

We know that math is not always clean cut, and many times we need more accurate numbers, so we need to use decimals to increase our accuracy, in Python we call these numbers with decimals, a **float** or `float`.  A **float** is any number that has a decimal in it. If we combine integers and floats in a mathematical operation, we will get a **float** as the result, always. Additionally, just like an integer, a float does not need any quotes, and if you do put it in quotes, it becomes a **string**. Some examples of **floats** are:

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
A **Boolean** or `bool` has two possible values: `True` or `False`.
It's fairly rare for programmers to explicitly write the word True or False. Instead our programs can respond to questions for you with a **boolean** and use this result to choose which path the program takes.

```python
5 == 5  # True
5 == 2  # False
2 + 2 == 4  # True
2.0 == 2   # True
```

## The `type()` function

***

Now that we know that there are many different data types, let's explore one way we can check the type of data you have. You can check the data type with the `type()` function. To check the type of data, you can simply pass the data as an argument to the `type()` function. For example, if you wanted to find out what type of data `Toronto` is, you could simply do this:

```
type('Toronto')
```
Or, if you were to assign 'Toronto' to a variable, it would look like this:

```python
city = 'Toronto'

type(city)
```

## Recap

***

Excellent, now that you have a little understanding of a few of the types of data Python uses, we can begin to put it to work and see how we can use this information.


