Introduction
As we already know from living in the digital age and the lessons we've already seen, programming is a powerful tool for answering questions about data. It allows us to collect, clean up and format our data and then perform calculations on that data. Much of our digital information is in the form of text, for example song lyrics and emails. To clean up and format that text with Python, we need to become familiar with our first type of data, the String.

Objectives
By the end of this lesson, you will be able to:

Apply string methods to make changes to a string
Inspect documentation with various methods
What are Strings?
A lot of information in the world is in the form of text. To capture this information and operate on it in Python we take this text and make it into the String (str) data type.

Below, we have the name of a cartoon character, Homer Simpson. By putting quotes ("") or ('') around the name, we create a string.

"Homer Simpson"
When programmers say string, what they mean is text. When programmers say data type, they just mean type of data. We can think of 'Homer Simpson' as an instance of the string data type.

Here are a few other types of data in Python that we will talk more about in later lessons:

100 # Integer
10.0 # Float
True # Boolean
Since there are several types of data in Python we can discover the type of any piece of data by calling, or executing, the type() function. By calling or executing a function, we mean running the function so that it executes the code within it.

Let's look at an example below:

Note: Press the shift + enter keys to run the code below. The cell that populates below is the return or output of the type function.

type("Homer Simpson")
str
We need to pay attention to what type of data we are working with because they operate differently and have different values as well as functions that we are able to use on them.

For example, to create a new string (or to initialize a string) we cannot simply type letters. Instead, we need to be very explicit and tell Python it is about to see some text. We do this by surrounding our text with quotes, "". If we don't do that or end our quotation marks too early, Python will throw an error.

Then we try this new method out ourselves, to see if this user on StackOverFlow is right (they normally are).

"hello world".title()
'Hello World'
print('This hello is the world's')
  File "<ipython-input-16-8260ff671940>", line 1
    print('This hello is the world's')
                                   ^
SyntaxError: invalid syntax


print("This hello is the world's")
This hello is the world's
And our work is done.

Feel free to look at other common string operations here.

```python
type(top_canadian_city)
```




    str



Now we have a variable of `top_canadian_city`, equal to the string 'Toronto', and a variable of `top_travel_cities` equal to the list of cities.  


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
     'Pyeongchang']




```python
type(top_travel_cities)
```




    list



### Accessing Multiple Elements

Now imagine that we don't want to access just one element of a list, but multiple elements at once.  Python allows us to do that as well:


```python
top_travel_cities[0:2]
```




    ['Solta', 'Greenville']



As we can see from the above example, we can access elements of a list by placing two numbers separated by a colon inside of our brackets. The first number indicates the index of the first element we want returned.  

The second number could represent the number of elements we want returned back, or maybe it represents the stopping index of the elements that we are retrieving.  Looking at our `top_travel_cities` it could be either.


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
     'Pyeongchang']



Let's try a different experiment to answer our question.


```python
top_travel_cities[4:5]
```




    ['Walla Walla Valley']



Ok, so that second number is not representing the number of elements we want returned.  Instead it must be the index at which we stop our selection of elements.


```python
top_travel_cities[4:6]
```




    ['Walla Walla Valley', 'Marakesh']



This operation is called `slice`.  So, we can say we are `slicing` the elements with indices 4 and 5 in the line above.  Note that even though we are `slicing` elements, our list remains intact.


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
     'Pyeongchang']



In programming terms, we would say that slicing elements is non-destructive, because it does not change the underlying data structure.  We can do it as many times as we like, and our `top_travel_cities` array remains unchanged.  If we wish to store that slice of elements, we can store it in another variable.


```python
top_two = top_travel_cities[0:2]
top_two
```




    ['Solta', 'Greenville']



Now we have another variable called `top_two` that points to an array which contains an array of elements equal to the first two elements of `top_travel_cities`.

### Changing elements with destructive methods

Now that we can read and select certain elements from lists, let's work on changing these lists. To add a new element to a list, we can use the `append` method.


```python
top_travel_cities.append('San Antonio')
```

Now let's take another look at `top_travel_cities`.


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
     'San Antonio']



You will see that 'San Antonio' has been added to the list.  Note that unlike slice, `append` is destructive.  That is, it changes our underlying data structure.  Every time we execute the `append` method, another element is added to our list.   Now what if we accidentally add 'San Antonio' a second time to our list.


```python
top_travel_cities.append('San Antonio')
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
     'San Antonio']


