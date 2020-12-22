### Finding Unique elements and length of lists

If we are not sure whether there are repeated elements, we can use Python to get a unique list.


```python
top_travel_cities.append('Solta')
```

For example, now that we have added Solta to the end of our list, Solta appears twice.

Well to see a unique list of the elements, we can call the `set` function. The set function is non-destructive on our list.


```python
unique_travel_cities = set(top_travel_cities)
unique_travel_cities
```




    {'Albuquerque',
     'Archipelago Sea',
     'Buenos Aires',
     'Greenville',
     'Iguazu Falls',
     'Los Cabos',
     'Marakesh',
     'Pyeongchang',
     'Salina Island',
     'San Antonio',
     'Solta',
     'Toronto',
     'Walla Walla Valley'}



The set function initializes a new set in Python.  A set is a different type collection in Python.  


```python
type(set())
```




    set



A set is just like a list, except elements do not have order and each element appears just once.


```python
unique_travel_cities[1]
```


    -------------------------------------------------------------------

    TypeError                         Traceback (most recent call last)

    <ipython-input-26-3d2453cad46e> in <module>()
    ----> 1 unique_travel_cities[1]
    

    TypeError: 'set' object does not support indexing


 So here, when we convert our list into a set, our set just consists of the unique elements.  But unfortunately this structure is a set, not a list.


```python
type(unique_travel_cities)
```




    set



So let's convert this set, which has a unique list of our travel cities, into a list.


```python
unique_travel_cities = list(unique_travel_cities)
```


```python
type(unique_travel_cities)
```




    list



So the array of `unique_travel_cities` is a unique list.


```python
unique_travel_cities
```




    ['Toronto',
     'Archipelago Sea',
     'Iguazu Falls',
     'Pyeongchang',
     'Los Cabos',
     'Buenos Aires',
     'Marakesh',
     'Greenville',
     'Albuquerque',
     'Salina Island',
     'Walla Walla Valley',
     'San Antonio',
     'Solta']



And you can see quickly that it differs from the list of top travel cities by checking the length.


```python
len(unique_travel_cities)
```




    13




```python
len(top_travel_cities)
```




    14




```python
top_travel_cities
```




    ['Solta',
     'Greenville',
     'Buenos Aires',
     'Los Cabos',
     'Walla Walla Valley',
     'Marakesh',
     'Albuquerque',
     'Archipelago Sea',
     'Iguazu Falls',
     'Salina Island',
     'Toronto',
     'Pyeongchang',
     'San Antonio',
     'Solta']



> **Note:** *For most purposes, Python developers prefer to work with `lists` as opposed to sets, as `lists` are generally easier to manipulate, as you will see in future lessons.*