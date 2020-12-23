# Manipulating Lists

## Adding and removing elements

***

We have been working with a list of popular travel destinations and with this list we have been using non-destructive methods to access and slice data.  As you can imagine, the popular travel destinations change frequently, so in this lesson we will explore the ways you can change the elements in your list with some destructive methods.  These methods are considered destructive because they will alter the original data list we created, unlike the mnethods we learned earlier which allow the data list to remain intact.

## Objectives for this lesson

***

* Add elements with `.append()`
* Remove elements with `.pop()`

In this lesson we will practice adding and removing elements in our list of travel destinations.  Here is the list for your reference:

```python
top_travel_cities = ['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea']
```
## Adding with the `.append()` method

***

If we take a close look at the list we will see that it doesn't have the destination that we talked about adding in the previous lesson, `'Wuhan, China'`.  Using the `.append()` method, let's add this destination to our list `top_travel_cities`.  To do this we will need to enter the following code into the code console below:

```python
top_travel_cities.append('Wuhan, China')
```

## Try it out

***

In the code console below, add the destination `'Wuhan, China'` to the list `top_travel_cities` using the `.append()` method.  Once you have added the item to the list, type the list name and look at the result of your change.
>**Level up** - create your own list of city names and add elements to it using the `.append()` method.  Add a few items and take a look at the list after each addition to see how it gets added to the end of the list.

<iframe frameborder="0" width="100%" height="600" src="https://repl.it/@DSExperience/CitiesTry5?lite=true"></iframe>

Great!! Now that we can see how to add elements to our list, lets take a look at how we remove items.

## Removing with the `.pop()` method

***

In this section we will be working with the following list, it is similar to our previous list, but when we tried to add the new destination, `'Wuhan, China'` we mistakenly added it twice.  Let's use the `.pop()` method to remove it.  The code we will input to do this looks like this:

```python
top_travel_cities.append('Wuhan, China')
```

## Try it out

***

In the code console below, we have loaded the list referenced above with the duplicate destination, using the `.pop()` method, remove the extra element, `'Wuhan, China'` from the list `top_travel_cities`. Once you have removed it, take a look at the list again to see if your code worked.
>**Level up** - type your own list as you did before, and practice removing items from it using the `.pop()` method.  Also, try removing a specific item from our list using the index as an argument with the `.pop()` method.  Remember, you can find the index of an item by passing the item as an argument to the `.index()` method.

<iframe frameborder="0" width="100%" height="700" src="https://repl.it/@DSExperience/CitiesTry6?lite=true"></iframe>

Good, now we are able to add and remove items from our list in the event we need to update it.  Let's take a look at some other tools that are helpful when working with lists.