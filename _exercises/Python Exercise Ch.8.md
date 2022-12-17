---
layout: page
title: Exercises Ch. 8
description: Functions
---

## 8-1 Message:
Write a function called `display_message()` that prints one sentence telling everyone what you are learning about in this chapter. Call the function, and make sure the message displays correctly.


```python
def display_message():
    """Introduction"""
    print("Nice to meet you! I'm learning how to create a function.")
```


```python
display_message()
```

    Nice to meet you! I'm learning how to create a function.


## 8-2 Favorite Book: 
Write a function called `favorite_book()` that accepts one parameter, title. The function should print a message, such as `One of my favorite books is Alice in Wonderland.` Call the function, making sure to include a book title as an argument in the function call.


```python
def favorite_book(title):
    """What is your favorite book."""
    print("My favorite book is called " + "'" + title.title() + ".'")
```


```python
favorite_book('A Wrinkle in Time')
```

    My favorite book is called 'A Wrinkle In Time.'


## 8-3 T-Shirt: 
Write a function called `make_shirt()` that accepts a size and the text of a message that should be printed on the shirt. The function should print a sentence summarizing the size of the shirt and the message printed on it.

Call the function once using positional arguments to make a shirt. Call the function a second time using keyword arguments.


```python
def make_shirt(size, message):
    """Description of T-Shirt"""
    print("The size of the t-shirt is " + size + ".")
    print("The message written on the t-shirt is " + "'" + message + ".'")
```


```python
make_shirt('S', 'YOLO')
```

    The size of the t-shirt is S.
    The message written on the t-shirt is 'YOLO.'



```python
def make_shirt(size, message):
    """Description of T-Shirt"""
    print("The size of the t-shirt is " + size + ".")
    print("The message written on the t-shirt is " + "'" + message + ".'")
```


```python
make_shirt(size = 'S', message = 'YOLO')
```

    The size of the t-shirt is S.
    The message written on the t-shirt is 'YOLO.'


## 8-5 Cities: 
Write a function called `describe_city()` that accepts the name of a city and its country. The function should print a simple sentence, such as Reykjavik is in Iceland. Give the parameter for the country a default value. Call your function for three different cities, at least one of which is not in the default country.


```python
def describe_city(city, country = 'Italy'): # parameter = the one inside the parenthesis
    """Cities in Italy."""
    print(city + " is a city in " + country + ".")
```


```python
describe_city('Venice')
describe_city('Milan')
describe_city('Tokyo', country = 'Japan')
```

    Venice is a city in Italy.
    Milan is a city in Italy.
    Tokyo is a city in Japan.


## 8-6 City Names: 
Write a function called `city_country()` that takes in the name of a city and its country. The function should return a string formatted like this:

    "Santiago, Chile"


```python
def city_country(city, country):
    """Returning the name of city and its country."""
    name = city + ", " + country + "."
    return name.title()

example = city_country('Seoul', 'South Korea')
print(example)
```

    Seoul, South Korea.


## 8-7 Album: 
Write a function called `make_album()` that builds a dictionary describing a music album. The function should take in an artist name and an album title, and it should return a dictionary containing these two pieces of information. Use the function to make three dictionaries representing different albums. Print each return value to show that the dictionaries are storing the album information correctly.

Add an optional parameter to `make_album()` that allows you to store the number of tracks on an album. If the calling line includes a value for the number of tracks, add that value to the album’s dictionary. Make at least one new function call that includes the number of tracks on an album.


```python
def make_album(artist_name, album_title):
    """Information of the album."""
    album_1 = {'Artist Name': artist_name, 'Album Title': album_title}
    return album_1

music1 = make_album('The Weeknd', 'Starboy')
print(music1)
music2 = make_album('Imagine Dragons', 'Evolve')
print(music2)
music3 = make_album('Halsey', 'Badlands')
print(music3)
```

    {'Artist Name': 'The Weeknd', 'Album Title': 'Starboy'}
    {'Artist Name': 'Imagine Dragons', 'Album Title': 'Evolve'}
    {'Artist Name': 'Halsey', 'Album Title': 'Badlands'}



```python
def make_album(artist_name, album_title, track):
    """Information of the album."""
    album_1 = {'Artist Name': artist_name, 'Album Title': album_title}
    if track: 
        album_1['Tracks'] = track
    return album_1

music1 = make_album('The Weeknd', 'Starboy', '18')
print(music1)
music2 = make_album('Imagine Dragons', 'Evolve', '15')
print(music2)
music3 = make_album('Halsey', 'Badlands', '11')
print(music3)
```

    {'Artist Name': 'The Weeknd', 'Album Title': 'Starboy', 'Tracks': '18'}
    {'Artist Name': 'Imagine Dragons', 'Album Title': 'Evolve', 'Tracks': '15'}
    {'Artist Name': 'Halsey', 'Album Title': 'Badlands', 'Tracks': '11'}

