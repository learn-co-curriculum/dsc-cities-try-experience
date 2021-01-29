# Accessing Multiple Items in a List

## Objectives for this lesson

* Knowledge check - Slicing

***

Now you know how to select multiple items from a list, let's use what you've learned and answer the questions below. If you're having trouble with any of these questions, try reviewing the previous lesson.

### Question 1 - 
***
#### Using our list of top travel cities below, select the line of code which will result in a list containing `"Buenos Aires, Los Cabos, and Walla Walla Valley."`

```python
top_travel_cities = ['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```


[1] `top_travel_cities[3, 6]`  
[2] `top_travel_cities[2:4]`  
[3] `top_travel_cities[2, 5]`  
[4] `top_travel_cities[3:5]`  
[5] `top_travel_cities[2:5]`  
[6] `top_travel_cities[3:6]`  

### Question 2 - 
***
### Using our list of top travel cities, match the code on the left with the output on the right.

```python
top_travel_cities = ['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```

[1] `top_travel_cities[0:2]`
[2] `top_travel_cities[:3]`
[3] `top_travel_cities[-4:-2]`
[4] `top_travel_cities[-3:]`
[5] `top_travel_cities[2:6]`
[6] `top_travel_cities[4:6]`

[1] `['Solta', 'Greenville']`
[2] `['Solta', 'Greenville', 'Buenos Aires']`
[3] `['Iguazu Falls', 'Salina Island']`
[4] `['Salina Island', 'Toronto', 'Pyeongchang']`
[5] `['Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh']`
[6] `['Walla Walla Valley', 'Marakesh']`