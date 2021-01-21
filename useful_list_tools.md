# Useful List Tools

## Objectives for this lesson

***

* Check the length of a list with the `len()` function
* Create a set of unique elements from a list
* Convert a set back to a list

## Checking the length of a list with the `len()` function

***

When working with a list of items like the list we have been using, you may find it necessary to find out how long the list is.  Python has a built in function to help you to determine the length of your list, and that function is `len()`.  To use this tool, you simply need to pass the name of the list you are working with as an argument to the function.  For example, if we wanted to find out the length of our list `top_travel_cities`, below it would look like this:

```python
top_travel_cities = ['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea', 'Wuhan, China', 'Wuhan, China', 'Toronto, Canada', 'Albuquerque, New Mexico', 'Salina Island, Sicily']

len(top_travel_cities)
```

When we run the above line of code, we will get the length number of componenets in the list, which in this case is `13`.  Notice that we did not put the name of the list in quotes.  The name of the list is a variable, and is only recognized by python if we don't put quotes around it. 

## Finding the unique items in a list

***

At times, you may find yourself working with a list that has repeated entries of some of the elements, this could be by design, or could, as in our case, indicate an error in the creation of the list.  Below we have a list that has some of our items more than once, and for this list of top destinations, it will muddy up our information.  For our situation, we are going to create a set of the unique items in our list using the `set()` function.  The `set()` function id another built in function in Python, and this will create a set of the unique elements in our list.  It is important to note that there are differences between a `list` and a `set`.  The first difference is the one we are going to use, and that is that a set has no duplicates.  When a list is converted to a set, each element, no matter how many times it is in the list, is recorded only once in the `set`.  To illustrate this, we will take a look at our list of destinations which, as you can see, has a few duplicates.

```python
top_travel_cities = ['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea', 'Wuhan, China', 'Wuhan, China', 'Toronto, Canada', 'Albuquerque, New Mexico', 'Salina Island, Sicily']
```

If we pass the name of this list to the `set()` function, we will remove all of the duplicates.  We can check this by using the `len()` function that we learned earlier.  First we will create a new variable to store the `set` and we will call this `top_cities_set` and we create this like this:

```python
top_cities_set = set(top_travel_cities)
```

When you create this `set`, you will notice that it is formatted a little different than a list.  The set we just created looke like this:

```python
{'Solta, Croatia', 'Los Cabos, Mexico', 'Pyeongchang, South Korea', 'Archipelago Sea', 'Walla Walla Valley, Washington', 'Buenos Aires, Argentina', 'Greenville, South Carolina', 'Wuhan, China', 'Albuquerque, New Mexico', 'Iguazu Falls,Argentina', 'Toronto, Canada', 'Salina Island, Sicily', 'Marakesh, Morocco'}
```
As you can see, the set is enclosed in curly braces `{}` instead of the square braces `[]` like the original list.  Now lets take a look at the length to compare the original `list` and our new `set` with the `len()` function, like this:

```python
len(top_travel_cities)
len(top_cities_set)
```

If we run these two commands, we will see that the `len(top_travel_cities)` is `17` and the `len(top_cities_set)`is 13.

Another difference of a set is that the elements are not ordered like they are in a list.  This means that we cannot reference the individual elements using an index as we do in a list.  This could be problematic if we need to access the individual elements.  To make this new collection easier to work with, we will convert it to a list.

## Converting a `set` to a `list`

***

At the beginning of this module we learned how to create a list by simply entering the data in the list format.  You will find during our data science course, that you will want to convert one type of data to another, as in our case now, we want to convert a `set` to a `list` so or data is easier to work with.  To convert our `top_cities_set` to a list, we pass it to the `list()` function as an argument like this:

```python
list(top_cities_set)
```

The result of this is a list like our original list with only 1 occurrence of each element.  Our new list looks like this:

```python
['Wuhan, China', 'Buenos Aires, Argentina', 'Salina Island, Sicily', 'Solta, Croatia', 'Walla Walla Valley, Washington', 'Pyeongchang, South Korea', 'Greenville, South Carolina', 'Toronto, Canada', 'Albuquerque, New Mexico', 'Archipelago Sea', 'Marakesh, Morocco', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico']
```

Notice that our new list now has a different order, this is because the order of a set is not rigid, it will not always be the same order, but it will contain all of the elements.

## Recap

***

Now we have learned how to check the length of a list with the `len()` function, create a `set` of unique elements from our list using the `set()` function, and convert the set to a list with the `list()` function.  It may have been a little difficult to follow all of this, but no worries, we will have a chance to practice all of this in the following lab to help understand these tools better.