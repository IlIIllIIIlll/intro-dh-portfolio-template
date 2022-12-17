---
layout: page
title: Exercises Ch. 6
description: Dictionaries
---

## 6-1 Person: 
Use a dictionary to store information about a person you know. Store their first name, last name, age, and the city in which they live. You should have keys such as first_name, last_name, age, and city. Print each piece of information stored in your dictionary.


```python
Ashley = {'first_name': 'Ashley', 'last_name': 'Park', 'age': '20', 'city': 'Seoul'}
```


```python
print(Ashley['first_name'])
print(Ashley['last_name'])
print(Ashley['age'])
print(Ashley['city'])
Ashley
```

    Ashley
    Park
    20
    Seoul





    {'first_name': 'Ashley', 'last_name': 'Park', 'age': '20', 'city': 'Seoul'}



## 6-2 Favorite Numbers: 
Use a dictionary to store people’s favorite numbers. Think of five names, and use them as keys in your dictionary. Think of a favorite number for each person, and store each as a value in your dictionary. Print each person’s name and their favorite number. For even more fun, poll a few friends and get some actual data for your program.


```python
favorite_numbers = {'Claire': '2', 'Lara': '20', 'Clara': '16', 'Meehee': '48', 'Angel': '86'}
for key, value in favorite_numbers.items():
    print(f"Name: {key}")
    print(f"Number: {value}")
```

    Name: Claire
    Number: 2
    Name: Lara
    Number: 20
    Name: Clara
    Number: 16
    Name: Meehee
    Number: 48
    Name: Angel
    Number: 86


## 6-3 Glossary: 
A Python dictionary can be used to model an actual dictionary. However, to avoid confusion, let’s call it a glossary.

* Think of five programming words you’ve learned about in the previous chapters. Use these words as the keys in your glossary, and store their meanings as values.
* Print each word and its meaning as neatly formatted output. You might print the word followed by a colon and then its meaning, or print the word on one line and then print its meaning indented on a second line. Use the newline character (\n) to insert a blank line between each word-meaning pair in your output.


```python
words = {'conditional tests': 'Test which allows one to check any condition of interest within coding.', 
         'if-statement': 'Statement that allows you to examine the current state of a program and respond appropriately to that state.', 
         'looping': 'Action that allows you to take the same action, or set of actions, with every item in a list.', 
         'variable': 'Word or phrase that holds a value, which is the information associated with that variable.', 
         'string': 'Almost any series of characters within single or double quotation mark.'
        }
print("Conditional Tests: " + "\n" + words['conditional tests'])
print("\n")
print("If-Statement: " + "\n" + words['if-statement'])
print("\n")
print("Looping: " + "\n" + words['looping'])
print("\n")
print("Variable: " + "\n" + words['variable'])
print("\n")
print("String: " + "\n" + words['string'])
```

    Conditional Tests: 
    Test which allows one to check any condition of interest within coding.
    
    
    If-Statement: 
    Statement that allows you to examine the current state of a program and respond appropriately to that state.
    
    
    Looping: 
    Action that allows you to take the same action, or set of actions, with every item in a list.
    
    
    Variable: 
    Word or phrase that holds a value, which is the information associated with that variable.
    
    
    String: 
    Almost any series of characters within single or double quotation mark.


## 6-4 Glossary 2: 
Now that you know how to loop through a dictionary, clean up the code from Exercise 6-3 by replacing your series of print statements with a loop that runs through the dictionary’s keys and values. When you’re sure that your loop works, add five more Python terms to your glossary. When you run your program again, these new words and meanings should automatically be included in the output.


```python
words = {
    'conditional tests': 'Test which allows one to check any condition of interest within coding.', 
    'if-statement': 'Statement that allows you to examine the current state of a program and respond appropriately to that state.', 
    'looping': 'Action that allows you to take the same action, or set of actions, with every item in a list.', 
    'variable': 'Word or phrase that holds a value, which is the information associated with that variable.', 
    'string': 'Almost any series of characters within single or double quotation mark.',
    'dictionary': 'Set of string that allows us to store data in key-value form.',
    'list': 'Collection of items in a particular order, storing sets of information in one place.',
    '\ n': 'Indication to insert a new line within Python coding.',
    'title.()/lower.()/upper.()': 'code to print string in titlecase, lowercase, and uppercase.',
    'syntax highlighting': 'When the editor highlights different parts of the program in different ways/color.'
}
for key, value in words.items():
    print(f"{key.title()}" + ":" )
    print(f"{value}")
    print("\n")
#this part took me exactly an hour because I didn't realize that I forgot to add commas at the end of each line and it gave me syntax error on the colon so what the heck.
```

    Conditional Tests:
    Test which allows one to check any condition of interest within coding.
    
    
    If-Statement:
    Statement that allows you to examine the current state of a program and respond appropriately to that state.
    
    
    Looping:
    Action that allows you to take the same action, or set of actions, with every item in a list.
    
    
    Variable:
    Word or phrase that holds a value, which is the information associated with that variable.
    
    
    String:
    Almost any series of characters within single or double quotation mark.
    
    
    Dictionary:
    Set of string that allows us to store data in key-value form.
    
    
    List:
    Collection of items in a particular order, storing sets of information in one place.
    
    
    \ N:
    Indication to insert a new line within Python coding.
    
    
    Title.()/Lower.()/Upper.():
    code to print string in titlecase, lowercase, and uppercase.
    
    
    Syntax Highlighting:
    When the editor highlights different parts of the program in different ways/color.
    
    


## 6-5. Rivers: 
Make a dictionary containing three major rivers and the country each river runs through. One key-value pair might be 'nile': 'egypt'.

* Use a loop to print a sentence about each river, such as The Nile runs through Egypt.
* Use a loop to print the name of each river included in the dictionary.
* Use a loop to print the name of each country included in the dictionary.


```python
rivers = {'amazon': 'brazil', 'mississippi': 'united states', 'ganges': 'india'}
```


```python
# Use a loop to print a sentence about each river, such as The Nile runs through Egypt
for river, country in rivers.items():
    print(river.title() + " River runs through " + country.title() + ".")
```

    Amazon River runs through Brazil.
    Mississippi River runs through United States.
    Ganges River runs through India.



```python
# Use a loop to print the name of each river included in the dictionary
for river in rivers.keys():
    print(river.title())
```

    Amazon
    Mississippi
    Ganges



```python
# Use a loop to print the name of each country included in the dictionary
for countries in rivers.values():
    print(countries.title())
```

    Brazil
    United States
    India


## 6-7 People: 
Start with the program you wrote for Exercise 6-1. Make two new dictionaries representing different people, and store all three dictionaries in a list called people. Loop through your list of people. As you loop through the list, print everything you know about each person.


```python
Ashley = {'first_name': 'Ashley', 'last_name': 'Park', 'age': '20', 'city': 'Seoul'}
Nicholas = {'first_name': 'Nicholas', 'last_name': 'Park', 'age': '24', 'city': 'Barcelona'}
Lynette = {'first_name': 'Lynette', 'last_name': 'Park', 'age': '21', 'city': 'London'}

people = [Ashley, Nicholas, Lynette]

for friends in people:
    print(friends)
```

    {'first_name': 'Ashley', 'last_name': 'Park', 'age': '20', 'city': 'Seoul'}
    {'first_name': 'Nicholas', 'last_name': 'Park', 'age': '24', 'city': 'Barcelona'}
    {'first_name': 'Lynette', 'last_name': 'Park', 'age': '21', 'city': 'London'}


## 6-8 Pets: 
Make several dictionaries, where the name of each dictionary is the name of a pet. In each dictionary, include the kind of animal and the owner’s name. Store these dictionaries in a list called pets. Next, loop through your list and as you do print everything you know about each pet.



```python
cookie = {'kind': 'cat', "owner's_name": 'Sally'}
choco = {'kind': 'dog', "owner's_name": 'Michael'}
sonic = {'kind': 'hedgehog', "owner's_name": 'John'}
poppy = {'kind': 'parrot', "owner's_name": 'Amy'}

pets = [cookie, choco, sonic, poppy]

for pet in pets:
    print(pet)
```

    {'kind': 'cat', "owner's_name": 'Sally'}
    {'kind': 'dog', "owner's_name": 'Michael'}
    {'kind': 'hedgehog', "owner's_name": 'John'}
    {'kind': 'parrot', "owner's_name": 'Amy'}


## 6-9 Favorite Places: 
Make a dictionary called `favorite_places`. Think of three names to use as keys in the dictionary, and store one to three favorite places for each person. To make this exercise a bit more interesting, ask some friends to name a few of their favorite places. Loop through the dictionary, and print each person’s name and their favorite places.


```python
#Using list inside dictionary

favorite_places = {
    'Sarah': ['Japan', 'Indonesia', 'Croatia'],
    'James': ['Brazil', 'South Korea', 'France'],
    'Morgan': ['Argentina', 'Morocco', 'Switzerland'],
}

for name, places in favorite_places.items():
    print("\n" + name.title() + "'s favorite places are:")
    
    for place in places:
        print("\t" + place.title())
```

    
    Sarah's favorite places are:
    	Japan
    	Indonesia
    	Croatia
    
    James's favorite places are:
    	Brazil
    	South Korea
    	France
    
    Morgan's favorite places are:
    	Argentina
    	Morocco
    	Switzerland


## 6-11 Cities: 
Make a dictionary called `cities`. Use the names of three cities as keys in your dictionary. Create a dictionary of information about each city and include the country that the city is in, its approximate population, and one fact about that city. The keys for each city’s dictionary should be something like country, population, and fact. Print the name of each city and all of the information you have stored about it.


```python
#Using dictionary inside dictionary

cities = {
    'Seoul': {
        'location': 'South Korea',
        'population': '9,976,000',
        'fact': 'Seoul is capital of South Korea.'
    },
    'Beijing': {
        'location': 'China',
        'population': '21,333,000',
        'fact': 'Beijing is home to seven UNESCO World Heritage Sites.'
    },
    'Frankfurt': {
        'location': 'Germany',
        'population': '791,000',
        'fact': 'Frankfurt’s population has one of the highest quality of life in the world.'
    }
}

for city, city_facts in cities.items():
    print("\n" + city + ":")
    locations = city_facts['location']
    populations = city_facts['population']
    facts = city_facts['fact']
    
    print("\tLocation: " + locations.title())
    print("\tPopulation: " + populations.title())
    print("\tFact: " + facts)
```

    
    Seoul:
    	Location: South Korea
    	Population: 9,976,000
    	Fact: Seoul is capital of South Korea.
    
    Beijing:
    	Location: China
    	Population: 21,333,000
    	Fact: Beijing is home to seven UNESCO World Heritage Sites.
    
    Frankfurt:
    	Location: Germany
    	Population: 791,000
    	Fact: Frankfurt’s population has one of the highest quality of life in the world.

