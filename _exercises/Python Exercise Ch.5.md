---
layout: page
title: Exercises Ch. 5
description: *If* Statements
---

## 5-1 Conditional Tests
Write a series of conditional tests. Print a statement describing each test and your prediction for the results of each test. Your code should look something like this:


```python
food = 'ramen'
print("Is food == 'ramen'? I predict True.")
print(food == 'ramen')
```

    Is food == 'ramen'? I predict True.
    True



```python
food = 'ramen'
print("Is food == 'ramen'? I predict False.")
print(food != 'ramen')
```

    Is food == 'ramen'? I predict False.
    False


* Create at least 10 tests. Have at least 5 tests evaluate to True and another 5 tests evaluate to False.


```python
# 1
pet = 'rabbit'
print("Is pet == 'rabbit'? I predict True.")
print(pet == 'rabbit')

pet = 'rabbit'
print("Is pet == 'rabbit'? I predict False")
print(pet != 'rabbit')
```

    Is pet == 'rabbit'? I predict True.
    True
    Is pet == 'rabbit'? I predict False
    False



```python
# 2
fruit = 'pineapple'
print("Is fruit == 'pineapple'? I predict True.")
print(fruit == 'pineapple')

fruit = 'pineapple'
print("Is fruit == 'pineapple'? I predict False")
print(fruit != 'pineapple')
```

    Is fruit == 'pineapple'? I predict True.
    True
    Is fruit == 'pineapple'? I predict False
    False



```python
# 3
family = 'mom and dad'
print("Are my family members 'mom and dad'? I predict True.")
print(family == 'mom and dad')

family = 'mom and dad'
print("Are my family members 'mom and dad'? I predict False.")
print(family != 'mom and dad')
```

    Are my family members 'mom and dad'? I predict True.
    True
    Are my family members 'mom and dad'? I predict False.
    False



```python
# 4
food = 'bibimbap'
print("Is my favorite food 'bibimbap'? I predict True.")
print(food == 'bibimbap')

food = 'bibimbap'
print("Is my favorite food 'bibimbap'? I predict False.")
print(food != 'bibimbap')
```

    Is my favorite food 'bibimbap'? I predict True.
    True
    Is my favorite food 'bibimbap'? I predict False.
    False



```python
# 5
phone = 'iPhone'
print("My phone is 'iPhone'. I state True.")
print(phone == 'iPhone')

phone = 'iPhone'
print("My phone is 'iPhone'. I state False.")
print(phone != 'iPhone')
```

    My phone is 'iPhone'. I state True.
    True
    My phone is 'iPhone'. I state False.
    False


## 5-2 More Conditional Tests: 

You don’t have to limit the number of tests you create to 10. If you want to try more comparisons, write more tests and add them to `conditional_tests.py`. Have at least one True and one False result for each of the following:

* Tests for equality and inequality with strings
* Tests using the lower() function
* Numerical tests involving equality and inequality, greater than and less than, greater than or equal to, and less than or equal to
* Tests using the and keyword and the or keyword
* Test whether an item is in a list
* Test whether an item is not in a list


```python
# Tests for equality and inequality with strings
sentence = "Is the password 'Hello_World!'?"
print("The sentence is == Is the password 'Hello_World?' I predict True.")
print(sentence == "Is the password 'Hello_World!'?")

sentence = "Is the password 'Hello_World!'?"
print("The sentence is == Is the password 'hello_world?' I predict False.")
print(sentence == "Is the password 'hello_world!'?")
```

    The sentence is == Is the password 'Hello_World?' I predict True.
    True
    The sentence is == Is the password 'hello_world?' I predict False.
    False



```python
# Tests using the lower() function
password = 'Hello_World!'
password == 'hello_world!'
```




    False




```python
password = 'Hello_World!'
password.lower() == 'hello_world!'
```




    True




```python
# Numerical tests involving equality and inequality, greater than and less than, greater than or equal to, and less than or equal to
age = 20
print("\n")
print("Is 20 less than 21? I predict True.")
print(age < 21)
print("\n")
print("Is 20 greater than 18? I predict True.")
print(age > 18)
print("\n")
print("Is 20 greater than or equal to 26? I predict False.")
print(age >= 26)
print("\n")
print("Is 20 less than or equal to 14? I predict False.")
print(age <= 14)
```

    
    
    Is 20 less than 21? I predict True.
    True
    
    
    Is 20 greater than 18? I predict True.
    True
    
    
    Is 20 greater than or equal to 26? I predict False.
    False
    
    
    Is 20 less than or equal to 14? I predict False.
    False



```python
# Tests using the 'and' keyword and the 'or' keyword
age1 = 20
age2 = 25
age1 < 22 and age2 <= 25
```




    True




```python
# or expression fails only when both individual tests fail
age1
age2 = 25
age1 > 23 or age2 >= 27
```




    False




```python
# Test whether an item is in a list
fruits = ['kiwi', 'mango', 'cherry', 'blueberry']
'kiwi' in fruits
```




    True




```python
fruits = ['kiwi', 'mango', 'cherry', 'blueberry']
'durian' in fruits
```




    False




```python
# Test whether an item is NOT in a list
family = ['grandfather', 'dad', 'mom']
member = 'aunt'
if member not in family:
    print(member.title() + ", please join us for a dinner party!")
```

    Aunt, please join us for a dinner party!


## 5-6 Stages of Life: 
Write an `if-elif-else` chain that determines a person’s stage of life. Set a value for the variable age, and then:

* If the person is less than 2 years old, print a message that the person is a baby.
* If the person is at least 2 years old but less than 4, print a message that the person is a toddler.
* If the person is at least 4 years old but less than 13, print a message that the person is a kid.
* If the person is at least 13 years old but less than 20, print a message that the person is a teenager.
* If the person is at least 20 years old but less than 65, print a message that the person is an adult.
* If the person is age 65 or older, print a message that the person is an elder.


```python
age = 74
if age < 2:
    print("You are a baby.")
elif age >= 2 and age < 4: 
    print("You are a toddler.")
elif age >= 4 and age < 13: 
    print("You are a kid.")
elif age >= 13 and age < 20: 
    print("You are a teenager.")
elif age >= 20 and age < 65: 
    print("You are an adult.")
else:
    print("You are an elder.")
```

    You are an elder.


## 5-7 Favorite Fruit: 
Make a list of your favorite fruits, and then write a series of independent if statements that check for certain fruits in your list.

* Make a list of your three favorite fruits and call it favorite_fruits.
* Write five if statements. Each should check whether a certain kind of fruit is in your list. If the fruit is in your list, the if block should print a statement, such as You really like bananas!


```python
favorite_fruits = ['kiwi', 'cherry', 'blueberry']
if 'kiwi' in favorite_fruits:
    print("I like kiwis, especially the gold ones.")
if 'mango' in favorite_fruits:
    print("I like mango!")
if 'cherry' in favorite_fruits:
    print("I like cherries. They're very tasty.")
if 'durian' in favorite_fruits:
    print("I like durians?")
if 'blueberry' in favorite_fruits:
    print("I like blueberries, as they are easy to eat.")
```

    I like kiwis, especially the gold ones.
    I like cherries. They're very tasty.
    I like blueberries, as they are easy to eat.


## 5-8 Hello Admin: 
Make a list of five or more usernames, including the name 'admin'. Imagine you are writing code that will print a greeting to each user after they log in to a website. Loop through the list, and print a greeting to each user:

* If the username is 'admin', print a special greeting, such as Hello admin, would you like to see a status report?
* Otherwise, print a generic greeting, such as Hello Eric, thank you for logging in again.


```python
users = ['admin', 'Ashley', 'mintypop', 'Chris', 'berrymore__' ]
for user in users:
    if user == 'admin':
        print("Hello " + user + ", would you like to see this week's progress report?")
    else:
        print("Hello " + user + ", I hope you are having a great day.")
```

    Hello admin, would you like to see this week's progress report?
    Hello Ashley, I hope you are having a great day.
    Hello mintypop, I hope you are having a great day.
    Hello Chris, I hope you are having a great day.
    Hello berrymore__, I hope you are having a great day.


## 5-9 No Users: 
Add an if test to hello_admin.py to make sure the list of users is not empty.

* If the list is empty, print the message We need to find some users!
* Remove all of the usernames from your list, and make sure the correct message is printed.


```python
users = ['admin', 'Ashley', 'mintypop', 'Chris', 'berrymore__' ]
for user in users:
    if user == 'admin':
        print("Hello " + user + ", your user list is full.")
```

    Hello admin, your user list is full.



```python
users = ['admin', 'Ashley', 'mintypop', 'Chris', 'berrymore__' ]
if users:
    for user in users:
        print("The user " + user + " is already an existing username.")
    print("\nHave a great day.")
else:
    print("The user does not exist.")
```

    The user admin is already an existing username.
    The user Ashley is already an existing username.
    The user mintypop is already an existing username.
    The user Chris is already an existing username.
    The user berrymore__ is already an existing username.
    
    Have a great day.



```python
users = []
if users:
    for user in users:
        print("The user " + user + " is already an existing username.")
    print("\nHave a great day.")
else:
    print("The user does not exist.")
```

    The user does not exist.


## 5-10 Checking Usernames: 
Do the following to create a program that simulates how websites ensure that everyone has a unique username.

* Make a list of five or more usernames called current_users.
* Make another list of five usernames called new_users. Make sure one or two of the new usernames are also in the current_users list.
* Loop through the new_users list to see if each new username has already been used. If it has, print a message that the person will need to enter a new username. If a username has not been used, print a message saying that the username is available.
* Make sure your comparison is case insensitive. If 'John' has been used, 'JOHN' should not be accepted.


```python
# Make a list of five or more usernames called current_users
current_users = ['chkim2002', 'Ashley', 'mintypop', 'Chris', 'berrymore__']
```


```python
# Make another list of five usernames called new_users. Make sure one or two of the new usernames are also in the current_users list
new_users = ['mintypop', 'cod1ng1sb3est', 'IlIllIlll', 'desse122', 'sadlegend89']
```


```python
# Loop through the new_users list to see if each new username has already been used
# If it has, print a message that the person will need to enter a new username
# If a username has not been used, print a message saying that the username is available

current_users = ['chkim2002', 'Ashley', 'mintypop', 'Chris', 'berrymore__']
new_users = ['mintypop', 'cod1ng1sb3est', 'IlIllIlll', 'desse122', 'sadlegend89']

for users in new_users:
    if users.lower() in current_users:
        print("I'm sorry, " + users + ", but your username is already taken.")
    else:
        print("That username is available " + users + ". Great choice!")
```

    I'm sorry, mintypop, but your username is already taken.
    That username is available cod1ng1sb3est. Great choice!
    That username is available IlIllIlll. Great choice!
    That username is available desse122. Great choice!
    That username is available sadlegend89. Great choice!
