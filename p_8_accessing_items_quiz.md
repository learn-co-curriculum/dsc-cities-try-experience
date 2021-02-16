# Accessing Single Items in a List

## Knowledge check - Indexing

***

Now that you have dug into accessing individual items in a list, use what yoy have learned and answer the questions below.  If you are having trouble with any of these questions, try reviewing the previous lesson.


### Question 1 -
***
#### Which of the following is a list?

[] ("Marakesh", "Croatia", "Iguazu Falls", "Toronto")
[x] ['Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
[] [Greenville, Buenos Aires, Los Cabos, Walla Walla Valley]
[] {"Solta", "Los Cabos", "Albuquerque", "Toronto"}
[x] ['Solta', "Greenville", 'Los Cabos', "Iguazu Falls", 'Toronto']
[] ['Pyeongchang' 'Toronto' 'Salina Island' 'Iguazu Falls']


### Question 2 -
***
#### Which answer will return the index of 4 from the following list?
- names = ['Kieron', 'Michael', 'Dayana', 'Joshua', 'Andy', 'Cierra', 'Mathew'] 

[] names.index('Cierra')
[] names['Andy']
[] names.index("Joshua")
[] names.index('Andy')
[] index['Cierra']


### Question 3 -
***
#### Using the list below, match the line of code with the item it references:

```python
top_travel_cities = ['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```
[1] `top_travel_cities[0]`  
[2] `top_travel_cities[-4]`  
[3] `top_travel_cities[2]`  
[4] `top_travel_cities[3]`  
[5] `top_travel_cities[-2]`  
[6] `top_travel_cities[-3]`  
[7] `top_travel_cities[1]`  

[1] `'Solta'`  
[2] `'Iguazu Falls'`  
[3] `'Buenos Aires'`  
[4] `'Los Cabos'`  
[5] `'Toronto'`  
[6] `'Salina Island'`  
[7] `'Greenville'`  


### Question 4 - 
***
#### Which of the following lines of code would assign 'Walla Walla Valley' to the variable 'top_us_city'?  

```python
top_travel_cities = ['Solta', 'Greenville', 'Buenos Aires', 'Los Cabos', 'Walla Walla Valley', 'Marakesh', 'Albuquerque', 'Archipelago Sea', 'Iguazu Falls', 'Salina Island', 'Toronto', 'Pyeongchang']
```

[1] `top_us_city = top_travel_cities[4]`  
[2] `top_us_city = top_travel_cities[3]`  
[3] `top_us_city = top_travel_cities(5)`  
[4] `top_travel_cities[3] = top_us_city`  
[5] `top_us_city = top_travel_cities['Walla Walla Valley']`  
[6] `top_travel_cities['Walla Walla Valley']  = top_us_city`  


### Question 5 -
***
#### Match the lines of code with the output using the list below.
- names = ['Kieron', 'Michael', 'Dayana', 'Joshua', 'Andy', 'Cierra', 'Mathew'] 

[1] names[2]
[2] names.index('Cierra')
[3] names[-3]
[4] names = [Kieron, Michael, Dayana, Joshua, Andy, Cierra, Mathew]
[5] names[7]
[6] names.index('Joshua')

[1] 'Dayana'
[2] 5
[3] 'Andy'
[4] NameError: name 'Kieron' is not defined
[5] IndexError: list index out of range
[6] 3
 

