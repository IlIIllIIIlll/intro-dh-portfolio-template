---
layout: page
title: Exercises Ch. 2
description: Variables and Simple Data Types
---

## 2-1 Simple Messages
Store a message in a variable, and then print that message.


```python
message = "I am currently eating a peach yogurt."
print(message)
```

    I am currently eating a peach yogurt.


## 2-2 Simple Messages
Store a message in a variable, and print that message. Then change the value of your variable to a new message, and print the new message.


```python
message = "I am currently eating a peach yogurt."
print(message)
```

    I am currently eating a peach yogurt.



```python
message = "I think I like blueberry yogurt better though."
print(message)
```

    I think I like blueberry yogurt better though.



```python
message = "I am currently eating a peach yogurt."
print(message)
message = "I think I like blueberry yogurt better though."
print(message)
```

    I am currently eating a peach yogurt.
    I think I like blueberry yogurt better though.


## 2-3 Personal Message
Store a person’s name in a variable, and print a message to that person. Your message should be simple, such as, “Hello Eric, would you like to learn some Python today?”


```python
name = "Ashley"
```


```python
message = "Hello " + name + ", " + "would you like to learn some more Python today?"
print(message)
```

    Hello Ashley, would you like to learn some more Python today?


## 2-4 Name Cases
Store a person’s name in a variable, and then print that person’s name in lowercase, uppercase, and titlecase.


```python
name = "Ashley Park"
print(name)
```

    Ashley Park



```python
print(name.lower())
print(name.upper())
print(name.title())
```

    ashley park
    ASHLEY PARK
    Ashley Park


## 2-5 Famous Quote
Find a quote from a famous person you admire. Print the quote and the name of its author.


```python
quote = 'Confucius once said, "Life is really simple, but we insist on making it complicated."'
print(quote)
```

    Confucius once said, "Life is really simple, but we insist on making it complicated."


## 2-6 Famous Quote (2)
Repeat Exercise 2-5, but this time store the famous person’s name in a variable called `famous_person`. Then compose your message and store it in a new variable called `message`. Print your message.


```python
famous_person = "Confucius"
message = famous_person + ' once said, "Life is really simple, but we insist on making it complicated."'
print(message)
```

    Confucius once said, "Life is really simple, but we insist on making it complicated."


## 2-7 Stripping Names
Store a person’s name, and include some whitespace characters at the beginning and end of the name. Make sure you use each character combination, "\t" and "\n", at least once.


```python
print("Ashley Park")
```

    Ashley Park



```python
print("\tAshley Park")
```

    	Ashley Park



```python
print("\tAshley Park\nLikes to code.")
```

    	Ashley Park
    Likes to code.



```python
message = "Ashley Park is 162cm.           "
print(message.rstrip())
second_message = "       Her dad's height is 175cm."
print(second_message.lstrip())
```

    Ashley Park is 162cm.
    Her dad's height is 175cm.



```python
print("\tAshley Park is 162cm\n\tHer dad's height is 175cm.")
```

    	Ashley Park is 162cm
    	Her dad's height is 175cm.



```python
name = "\tAshley Park"
print(name.lstrip())
new_name = "\nEda Chen"     "."
print(new_name.rstrip())
```

    Ashley Park
    
    Eda Chen.


## 2-10 Adding Comments
Choose two of the programs you’ve written, and add at least one comment to each. If you don’t have anything specific to write because your programs are too simple at this point, just add your name and the current date at the top of each program file. Then write one sentence describing what the program does.


```python
famous_person = "Confucius"
message = famous_person + ' once said, "Life is really simple, but we insist on making it complicated."' #Use one apostrophe when you are using quotation again in your message.
print(message)
```

    Confucius once said, "Life is really simple, but we insist on making it complicated."



```python
name = "\tAshley Park" #takes away spaces at the left
print(name.lstrip())
new_name = "\nEda Chen"     "."
print(new_name.rstrip()) #takes away spaces at the right
```

    Ashley Park
    
    Eda Chen.



```python
print(name.lower()) #print name in lowercase
print(name.upper()) #print name in uppercase
print(name.title()) #print name in titlecase
```

    	ashley park
    	ASHLEY PARK
    	Ashley Park