# Manipulating Lists

## Objectives for this lesson

***

* Add elements with `.append()`
* Remove elements with `.pop()`

## Adding and removing elements

***

Until now, you've been working with a list of popular travel destinations and with this list you have been using non-destructive methods to access and slice data. As you can imagine, the popular travel destinations change frequently, so in this lesson, you'll be exploring ways you can change the elements in your list.  


The methods you have been using up to this point are known as non-destructive methods because these methods do not change the original data.  In this lesson we will explore some destructive methods and look at how they change the original data.

## Adding elements with the `.append()` method

***

The `top_travel_cities` list is quite short, and there is a lot of room for us to expand the list so we can include other destinations.  In our case, we want to add a new destination city in Asia, `Wuhan, China`. To add this destination to our list, we will use the `.append()` method.  To use this method, you need to first reference your list `top_travel_cities`, apply the method using the so-called "dot notation" and then pass the element you wish to add to the list as an argument to the method.  When it's all put together, the code looks like this:


```python
top_travel_cities.append('Wuhan, China')
```
After we run this line of code, our list will look like this:

```python
['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea', 'Wuhan, China']
```
As you can see, the list has been altered, and now the last element is the item that was appended to the list, `Wuhan, China`.  

What if you mistakenly ran the line of code twice and we noticed that the destination was added twice? We would now find ourselves in need of removing the last item in the list. Let's take a look at how we would do this with another Python method.

## Removing elements with the `.pop()` method

***

Removing an element from a list is very similar to adding, we will just be using another of Python's methods.  The method we will use is the `.pop()` method.  Unlike the `append()` method, this method needs no arguments, but you can specify some if you choose, which we will look into later. If you don't provide an argument, the `.pop()` default is to remove the last item in the list. 

For example, if we wanted to remove the last city, `Pyeongchang, South Korea`, from our list, we would use the following code:

```python
top_travel_cities.pop()
```
After running this line of code, our list would look like this:

```python
['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Archipelago Sea', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea']
```

While the default action for the `.pop()` method is to remove the last item from the list, it can also be used with an index to remove a specific item from the list.  

If you look at our list closely, you can see that they are all cities except for `Archipalago Sea`.  While this may be a popular travel destination, it is not a city so it doesn't fit in our data.  

If we want to remove this item from the list, we first must determine its index which can be done by counting, or we can use the `.index()` method like this:

```python
top_travel_cities.index('Archipelago Sea')
```

When we run this line of code, we learn that the index of `'Archipelago Sea'` is `7`.  With this information, we can now use the `.pop()` method to remove it from our list by passing the index as an argument to the `.pop()` method like this:

```python
top_travel_cities.pop(7)
```

Once we run this command, our original list will be altered and will now look like this:

```python
['Buenos Aires, Argentina', 'Iguazu Falls,Argentina', 'Los Cabos, Mexico', 'Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada', 'Salina Island, Sicily', 'Solta, Croatia', 'Marakesh, Morocco', 'Pyeongchang, South Korea']
```

## Recap

***

Awesome, now we can add and remove items from out list to keep it up to date.  Let's take some time to practice these new skills in the next lesson.