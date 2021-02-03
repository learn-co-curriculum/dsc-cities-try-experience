# Adding and removing elements - lab

## Objectives for this lesson

***

* Add elements with `.append()`
* Remove elements with `.pop()`

In this lesson you will practice adding and removing elements in the list of travel destinations.  Here is the list for your reference:

```python
top_travel_cities = ['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea']
```
## Adding with the `.append()` method

***

If you take a close look at the list we will see that it doesn't have the destination that we talked about adding in the previous lesson, `'Wuhan, China'`.  Using the `.append()` method, let's add this destination to our list `top_travel_cities`.  

## Try it out

***

In the code console below, add the destination `'Wuhan, China'` to the list `top_travel_cities` using the `.append()` method.  Once you have added the item to the list, type the list name and look at the result of your change.

>**Level up** - create your own list of city names and add elements to it using the `.append()` method.  Add a few items and take a look at the list after each addition to see how it gets added to the end of the list.

<iframe frameborder="0" width="100%" height="600" src="https://repl.it/@DSExperience/CitiesTry5?lite=true"></iframe>

Great!! Now that you can add elements to alist, let's take a look at how we remove items.

## Removing with the `.pop()` method

***
Oops! When trying to add the new destination, `'Wuhan, China'` we mistakenly added it twice. This is where `.pop()` can be very helpful:   you can use this method to remove this duplicate list item.

## Try it out

***

In the code console below, we have loaded the list referenced above with the duplicate destination. Using the `.pop()` method, remove the extra element, `'Wuhan, China'` from the list `top_travel_cities`. Once you have removed it, take a look at the list again to see if your code worked.

>**Level up** - type your own list as you did before, and practice removing items from it using the `.pop()` method.  Also, try removing a specific item from our list using the index as an argument with the `.pop()` method.  Remember, you can find the index of an item by passing the item as an argument to the `.index()` method.

<iframe frameborder="0" width="100%" height="700" src="https://repl.it/@DSExperience/CitiesTry6?lite=true"></iframe>

## Recap

***

Great! you are now able to add and remove items from a list when this list needs to be updated.  Let's take a look at some other tools that are helpful when working with lists.