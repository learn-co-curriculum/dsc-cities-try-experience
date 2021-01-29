# Slicing - Lab

## Objectives for this lesson

***

* Practice selecting multiple items from a list using a range of indices
* Select multiple items with slicing
* Create a new list from a slice of the original list

## Slicing

***

In this lesson you will practice slicing elements of a list.  In the code console below, we have loaded the list `top_travel_cities` for you. You will use slicing to select the the desired sections of the list as described in the instructions below.

## Try it out

***

In the code console below, type in the folowing code to see the result of the slice.

```python
print(top_travel_cities[0:3])

print(top_travel_cities[3:7])
```
>**Level up** - try choosing some slices of your own.  Think about what cities you would like to get and write the code to select just those cities.

<iframe frameborder="0" width="100%" height="800" src="https://repl.it/@DSExperience/CitiesTry4?lite=true"></iframe>


## Making slicing work

***

In this section you will learn how to slice the original list into separate lists according to some additional criteria.  We have added the country for each city so we can group them according to their continents.  

In the code console below, use slicing to create lists and set them equal to the appropriate variables as shown in the cell below:

```python
south_america = ['Buenos Aires, Argentina', 'Iguazu Falls, Argentina', 'Los Cabos, Mexico']
north_america = ['Walla Walla Valley, Washington', 'Albuquerque, New Mexico', 'Greenville, South Carolina', 'Toronto, Canada']
not_a_city = [ 'Archipelago Sea']
europe = ['Salina Island, Sicily', 'Solta, Croatia']
asia = ['Marakesh, Morocco', 'Pyeongchang, South Korea']
```

<iframe frameborder="0" width="100%" height="800" src="https://repl.it/@DSExperience/CitiesTry5?lite=true"></iframe>


## Recap

***

You now have a good understanding of the basics of a list and how to access the items in it, let's look deeper into how to manipulate a list by adding, removing and changing the items.


