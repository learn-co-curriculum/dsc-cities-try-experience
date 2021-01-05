# Mini Project

## Graphing cities

***

Ok, so now that we have a sense of how to read from and alter a list in Python, let's see how our knowledge of lists can help us in creating data visualizations in Python.

## Working with lists and maps

As we know, lists are used to store a collection of data.  In describing a city, we can use lists to organize our data in all sorts of ways.  For example, here is a list of the top 25 cities to travel to in the world in 2020:

```python
cities = ['Oaxaca', 'Mexico', '17.021886', '-96.784615',
          'San Miguel de Allende', 'Mexico', '20.910399','-100.737493',
          'Hoi An', 'Vietnam', '15.883323', '108.340323',
          'Chiang Mai', 'Thailand', '18.754378', '98.973933',
          'Florence', 'Italy', '43.773492', '11.247146',
          'Kyoto', 'Japan', '35.131373', '135.526008',
          'Udaipur', 'India', '24.3566124', '73.706713',
          'Luang Prabang', 'Laos', '19.863075', '102.215407',
          'Ubud', 'Indonesia', '-8.502221', '115.265032',
          'Istanbul', 'Turkey', '41.162210', '28.765515',
          'Mexico City', 'Mexico', '19.407963', '-99.147823',
          'Bangkok', 'China', '13.741712', '100.568078',
          'Rome', 'Italy', '41.899323', '12.494508',
          'Jaipur', 'India', '26.910191', '75.786958',
          'Tokyo', 'Japan', '35.668356', '139.736732',
          'Siem Reap', 'Cambodia', '13.382729', '103.890376',
          'Lisbon', 'Portugal', '38.762778', '-9.182357',
          'Charleston, SC', 'USA', '32.788745', '-80.003739',
          'Cuzco', 'Peru', '-13.535684', '-71.964657',
          'Porto', 'Portugal', '41.159228', '-8.625023',
          'Singapore', 'Singapore', '1.352427', '103.866592',
          'New Orleans, LA', 'USA', '29.942969', '-90.085780',
          'Seville', 'Spain', '37.387139', '-5.986822',
          'Mérida', 'Mexico', '20.963875', '-89.596392',
          'Kraków', 'Poland', '50.027269', '19.979097']
```

In this list of cities, we can see that each city has a little information about it.  We have the city name first, then the country, and then the location coordinates in the form of latitude and longitude.  We can also see that this is a bit messy, with all of the information packed into a list, it makes it a bit difficult to work with.  Lets get this list into a format that has a little more structure.  We can start by making a list of each of the elements for each list so that for each city we have a list of its atributes.  For example the first city in our list is 'Oaxaca', we can make the list of its attributes that will look like this:

```python
['Oaxaca', 'Mexico', '17.021886', '-96.784615']
```
We can iterate through the list with a for loop to get each city's information into a list and each list will have an index corresponding to its rank in the top 20.

```python
palermo = None
```

Now assign the variable `la_boca` to the last element of our list.