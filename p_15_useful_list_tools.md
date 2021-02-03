# Useful List Tools

## Objectives for this lesson

***

* Check the length of a list with the `len()` function
* Create a set of unique elements from a list
* Convert a set back to a list

## Checking the length of a list with the `len()` function

***

When working with a list of items, you may find it necessary to find out how long the list is. Python has a built-in function to help you to determine the **length** of your list, and that function is `len()`.  To use this tool, you simply need to pass the name of the list you are working with as an argument to the function.  For example, if you want to find out the length of your list `top_travel_cities`, it would look like this:

```python
top_travel_cities = ['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea', 'Wuhan, China', 'Wuhan, China', 'Toronto, Canada', 'Albuquerque, New Mexico', 'Salina Island, Sicily']

len(top_travel_cities)
```

When we run the line of code above, we will get the number of componenets in the list, which in this case is `13`.  Notice that we did not put the name of the list in quotes.  The name of the list is a **variable**, and is only recognized by python if we don't put quotes around it. 

## Finding the unique items in a list

***

At times, you may find yourself working with a list that has repeated entries of some of the elements, this could be by design, or could, as in our case, indicate an error in the creation of the list.  

You can see list that has some of our items more than once below. For this list of top destinations, it will muddy up our information. In this situation, you'll want to create a set of the unique items in our list using the `set()` function.  The `set()` function is another built-in function in Python, which create a **set of the unique elements** in our list.  

It is important to note that there are differences between a `list` and a `set`.  The first difference is that a set has no duplicates (which is the reason we use it here).  When a list is converted to a set, each element, no matter how many times it is in the list, is recorded only once in the `set`.  To illustrate this, let's take a look at our list of destinations which, as you can see, has a few duplicates:

```python
top_travel_cities = ['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea', 'Wuhan, China', 'Wuhan, China', 'Toronto, Canada', 'Albuquerque, New Mexico', 'Salina Island, Sicily']
```

If you pass the name of this list to the `set()` function, all duplicates are being removed. This can be checked this by using the `len()` function.  First, let's create a new variable (`top_cities_set`) to store the `set` like this:

```python
top_cities_set = set(top_travel_cities)
```

When you create this `set`, you'll notice that it is formatted a little different than a list. The set we just created looke like this:

```python
{'Solta, Croatia', 'Los Cabos, Mexico', 'Pyeongchang, South Korea', 'Archipelago Sea', 'Walla Walla Valley, Washington', 'Buenos Aires, Argentina', 'Greenville, South Carolina', 'Wuhan, China', 'Albuquerque, New Mexico', 'Iguazu Falls,Argentina', 'Toronto, Canada', 'Salina Island, Sicily', 'Marakesh, Morocco'}
```
As you can see, the set is enclosed in curly braces `{}` instead of the square braces `[]` like the original list. Let's now take a look at the length to compare the original `list` and our new `set` with the `len()` function, like this:

```python
len(top_travel_cities)
len(top_cities_set)
```

If you run these two commands, you'll see that `len(top_travel_cities)` is 17 and `len(top_cities_set)`is 13.

Another difference of a set is that the elements are not ordered like they are in a list.  This means that we cannot reference the individual elements using an index as we do in a list.  This could be problematic if we need to access the individual elements. While sets can be useful, we prefer lists for our application. That's why you'll learn next about how to convert a `set` into a `list.

## Converting a `set` to a `list`

***

At the beginning of this module, you learned how to create a list by simply entering the data in the list format. During Flatiron School's our Data Science course, you'll end up converting one data format into another **very often**, whether it is to merge different data structures or just because one data type is easier to work with. 

To convert `top_cities_set` to a list, we pass it to the `list()` function as an argument like this:

```python
list(top_cities_set)
```

The result of this is a list like our original list with only 1 occurrence of each element. The new list looks like this:

```python
['Wuhan, China', 'Buenos Aires, Argentina', 'Salina Island, Sicily', 'Solta, Croatia', 'Walla Walla Valley, Washington', 'Pyeongchang, South Korea', 'Greenville, South Carolina', 'Toronto, Canada', 'Albuquerque, New Mexico', 'Archipelago Sea', 'Marakesh, Morocco', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico']
```

Notice that the new list now has a different order, this is because the order of a set is not rigid - it will **not** always be the same order, but it will contain all of the elements.

## Recap

***

Now you've learned how to check the length of a list with the `len()` function, create a `set` of unique elements fromthe list using the `set()` function, and convert the set to a list with the `list()` function.  It may have been a little difficult to follow all of this, but no worries, you'll have a chance to practice all of this in the following lab to help understand these tools better.