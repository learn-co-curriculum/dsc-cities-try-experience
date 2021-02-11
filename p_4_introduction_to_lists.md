# The `list` data type

## Objectives for this lesson

***

* Create a `list`
* Access individual elements of a `list`
* Access multiple elements of a `list`

### Creating a list 
***

Now that you have been introduced to some different types of data used in Python, in this module we will focus on one very useful **compound data type**, the `list`.  A `list` is a form of a collection, and a collection is just a way of grouping data together and lists certainly accomplish this.  

For example, let's consider the top cities for travel according to the magazine *Travel and Leisure*. Below is how we are used to seeing a list of travel locations in a document or on a website.

#### Travel Locations
1. Solta
2. Greenville
3. Buenos Aires
4. Los Cabos
5. Walla Walla Valley
6. Marakesh
7. Albuquerque
8. Archipelago Sea
9. Iguazu Falls
10. Salina Island
11. Toronto
12. Pyeongchang

Here is what that list looks like as a Python `list`:

```python
['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```


You can indicate that you are initializing a `list` with an opening bracket, `[`, and end the list with a closing bracket `]`. Each list item, also called an element, is separated with a comma `,`. The components of a list can be any data type or any combination of data types, in this example each element is a string representing a city name.

In the format above, a `list` is not very useful, but you can make it useful. To retrieve your list later, you can **declare a variable** and assign our list to it, so that you can name it and later retrieve the list and reference it's contents. It is important to note the difference between a string and a variable.  A string is indicated by text surrounded by single or double quotes, if you wish to reference a variable, you simply type it without any quotes to indicate to Python that you want the value associated with the name you typed. 

In the code block below, we are assigning our list of cities to the variable`top_travel_cities`.

```python
top_travel_cities = ['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```

If you type the code above into a python compiler, the information in the list will be stored in memory and you will be able to recall it or reference it simply by using the variable name `top_travel_cities`.  After assigning the list to the variable name, if you enter the variable name, `top_travel_cities`, into the code compiler, you will get the cell below as your output.

`['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']`

## Recap
***
Great, now that you have an idea of how to create a list and assign it to a variable, we can practice it ourselves and apply what we have learned. In the next lesson you will have an opportunity to do just that, using the interactive code console. Let's go!

