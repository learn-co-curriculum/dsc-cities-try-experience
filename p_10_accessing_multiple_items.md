# Accessing Multiple Elements

## Objectives of this lesson

***

* Access multiple items of a list
* Slicing with indicies

## Slicing - **Start**

***

Imagine that we don't want to access just one element of a list, instead, multiple elements at once as a block.  Python allows us to do that as well.  To  do this, instead of passing a single number for the index, we pass a range of indices.  So if we wanted to select the first two elements in our list, `'Solta', 'Greenville'`, we would do it like this:

```python
top_travel_cities[0:2]
```

As we can see from the above example, we can access elements of a list by placing two numbers separated by a colon inside of our brackets. The first number indicates the index of the first element we want returned or where we would like to **start** our **slice**. 

## Indexing - **Stop**

***

From this first example, it is difficult to know if the second number represents the number of elements we want returned back, or the stopping index of the elements that we are retrieving.  Looking at our `top_travel_cities` it could be either.

```python
['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```

Let's take a look at a different slice and see how we would slice out one element from the list.  If we wanted to slice one item, like `'Walla Walla Valley'` we would do it like this:

```python
top_travel_cities[4:5]
```

Ok, so from this example, it is aparent that second number is not representing the number of elements we want returned.  Instead it must be the index at which we **stop** our selection of elements. In this case, we would say that the **stop** index id non-inclusive. So if we wanted to slice out elements 4 and 5, `'Walla Walla Valley', 'Marakesh'` we would want to **start** before `4` and **stop** before `6`, so we would code it like this:


```python
top_travel_cities[4:6]
```

A selection of elements using a range of indices is called a `slice`.  So, we can say we are `slicing` the elements with indices 4 and 5 in the line above.  Note that even though we are `slicing` elements, our list remains intact, it does not affect the original list at all.

In programming terms, we would say that slicing elements is non-destructive, because it does not change the underlying data structure.  We can do it as many times as we like, and our `top_travel_cities` list remains unchanged.  If we want to store that slice of elements, we would need to store it in another variable. For example, if we wanted to store `'Solta', 'Greenville'` as the variable `top_two` we would do it like this:

```python
top_two = top_travel_cities[0:2]
```
Now we have another variable called `top_two` that points to a list which contains elements equal to the first two elements of `top_travel_cities`.

## Recap

***

Now that we have discovered how to **slice** elements from a list and assign the results to a variable, let's practice writing the code.