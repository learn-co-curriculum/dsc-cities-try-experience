# Indexing

## Objectives for this lesson

***

* Access elements of a `list`
* Assign a single element of a `list` to a variable
* Use the index of list items

## Accessing Elements of Lists

***

Now that our `top_travel_cities` list contains multiple elements we can dive a little deeper into the traits of a list. When we write list for ourselves, we normally list the elements in numerical order with a number representing the items rank in the list, this helps us to keep the list ordered like this:

1. Solta
2. Greenville
3. Buenos Aires

## Indexing - from the beginning

***

Much like you would number the list to keep it ordered for our use, Python also assigns a number to each element. This number is called an **index**.  This index is like the element's address within the list and represents the distance from the beginning.  The index begins at the first item and continues through the list in numerical order.  Unlike the way you may start to number a list with the number "1", in Python, the index begins with zero, you can think of the item as being "0" spaces from the beginning. 

Lets take a look at how you would use the index if you wanted to reference a single item in our list, `top_travel_cities`. First, you need to reference the list you're working with, and next you can access a specific element of the list by wrapping the index of the item in the list in brackets`[]`. Below is how you would reference the first element which has the index of `0`.

```python
top_travel_cities[0] 
```
This code would return `Solta`.

Here is a reminder of the list of cities we are working with:

```python
['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```
If you wanted to reference the 4th element in this list, `Los Cabos` you would do it like this:

```python
top_travel_cities[3]
```
## Indexing - from the end

***

Great, now you know how to access one item in the list using it's index, but how would we access the last element? What about the third from the last element?   

If you wanted to select the last element, `Peyongchang`, you could count all of the elements in the list, and in our list `Pyeongchang` would just be one less than the length of the list.  

Python has a great way to make this easier for us. In Python, you tell the computer to start at the end by using a negative index. Python will move the specified number of spaces from the end.  For example, to access the last element you simply use the index `[-1]` in our list to access `'Pyeongchang'` like this:


```python
top_travel_cities[-1]
```

And you can move back as many as you want. To access 'Toronto', you would do this:


```python
top_travel_cities[-2]
```

At times, you may want to access an element from a list and use it by itself. To do that, you can always set an element of your list `top_travel_cities` equal to a variable. If you wanted to assign `'Toronto' to a variable `top_canadian_city`, you would do it like this:


```python
top_canadian_city = top_travel_cities[-2]
```

## Recap

***

Awesome! Now that you know how to access the individual items in your list using indexing from both the beginning of a list and from the end, let's practice using the index to access our top travel cities.

