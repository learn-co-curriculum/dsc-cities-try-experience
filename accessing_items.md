# Accessing Single Items in a List
***

## Objectives for this lesson
***

* Access elements of a `list`
* Assign a single element of a list to a variable
* Use the index of list items

## Accessing Elements of Lists

***

Now our `top_travel_cities` list contains multiple elements. When we write list for ourselves, we normally list them in numerical order with a number representing the items rank in the list, this helps us to keep the list ordered like this:

1. Solta
2. Greenville
3. Buenos Aires

Much like we would keep the list ordered, Python also assigns a number to each element. This number is called an **index**.  This number is like the element's address within the list and the index represents the distance from the beginning.  The index begins at the first item and continues through the list in numerical order.  Unlike the way you may start to number a list with the number "1", in Python, the index begins with zero because the item is "0" spaces from the beginning. 
Lets take a look at how you would use the index if you wanted to reference a single item in the list, `top_travel_cities`. We would first reference the list we are working with, and then using the brackets to access a specific element of our list with the index of the item in the list. Below is how we would reference the first element which has the index of `0`.

```python
top_travel_cities[0] 
```
This code would reference `Solta`.

Here is a reminder of the list of cities we are working with:

```python
['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```
If we wanted to reference the 4th element in this list, `Los Cabos` we would do it like this:

```python
top_travel_cities[3]
```

Great, now we know how to access one item in the list using it's index, but how would we access the last element? What about the third from the last element?   Well, we could count all of the elements in the list, and in our list `Pyeongchang` would just be one less than that.  In Python we tell the computer to start at the end by using a negative index and python will move the number of spaces from the end that you give it.  For example, to access the last element you simply use the index `[-1]` in our list to access `'Pyeongchang'` like this:


```python
top_travel_cities[-1]
```

And we can move back as many as we want, so to access 'Toronto' we would do this:


```python
top_travel_cities[-2]
```

Each element in our list is a string, so, we can always set an element of our list `top_travel_cities` equal to a variable. If we wanted to assign `'Toronto' to a variable `top_canadian_city` we would do it like this:


```python
top_canadian_city = top_travel_cities[-2]
```

## Recap

***

Awesome!! Now that we know how to access the individual items in our list, lets practice using the index.

