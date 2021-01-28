# Accessing Multiple Elements

## Objectives of this lesson

***

* Access multiple items of a list
* Slicing with indicies

## Slicing - **Start**

***

Imagine you don't want to access just one element of a list, instead, you want to select multiple elements at once as a block, Python allows you to do that as well. 

To do this, instead of passing a single number for the index, you pass a range of indices.  If you wanted to select the first two elements in our list, `'Solta', 'Greenville'`, you would do it like this:

```python
top_travel_cities[0:2]
```

As you can see from the above example, you can access elements of a list by placing two numbers separated by a colon inside of our brackets. The first number indicates the index of the first element you want returned or you would like to **start** your slice. 

## Indexing - **Stop**

***

From this first example, it is difficult to know if the second number represents the number of elements you want returned back, or the stopping index of the elements that you are retrieving.  Looking at our `top_travel_cities` it could be either.

```python
['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```

Let's take a look at a different slice and see how you can slice out two elements from the somewhere in the list.  If you want to slice two items, like `'Walla Walla Valley', 'Marakesh'` we can do it like this:

```python
top_travel_cities[4:6]
```

Ok, so from this example, it is aparent that second number is not representing the number of elements that we wanted returned.  Instead it must be the index at which we **stop** our selection of elements. In this case, you would say that the **stop** index is non-inclusive. So if you want to slice out elements 4 through 6, `'Walla Walla Valley', 'Marakesh', 'Albuquerque'` you need to **start** before `4` and **stop** before `7`, so you can code it like this:


```python
top_travel_cities[4:7]
```

A selection of elements using a range of indices is called a `slice`.  So, we are **slicing** the elements with indices 4, 5 and 6 in the code above.  Note that even though we are **slicing** elements, our list remains intact, it does not affect the original list at all.

In programming terms, we say slicing elements is **non-destructive**, because it does not change the underlying data structure.  You can do it as many times as you like, and the `top_travel_cities` list remains unchanged.  

If you want to store that slice of elements, you need to store it in another variable. For example, if you want to store `'Solta', 'Greenville'` as the variable `top_two` you can code it like this:

```python
top_two = top_travel_cities[0:2]
```
Now you have another variable called `top_two` that points to a list which contains elements equal to the first two elements of `top_travel_cities`.

## Recap

***

Now that you've discovered how to **slice** elements from a list and assign the results to a variable, let's practice writing the code.