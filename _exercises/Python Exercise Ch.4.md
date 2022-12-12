---
layout: page
title: Exercises Ch. 4
description: Working with Lists
---

## 4-1 Pizzas
Think of at least three kinds of your favorite pizza. Store these pizza names in a list, and then use a for loop to print the name of each pizza.

- Modify your for loop to print a sentence using the name of the pizza instead of printing just the name of the pizza. For each pizza you should have one line of output containing a simple statement like I like pepperoni pizza.
- Add a line at the end of your program, outside the for loop, that states how much you like pizza. The output should consist of three or more lines about the kinds of pizza you like and then an additional sentence, such as I really love pizza!


```python
pizza = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato']
print(pizza)
```

    ['BBQ Chicken', 'Pepperoni', 'Bacon Potato']



```python
for pizzas in pizza:
    print(pizzas)
```

    BBQ Chicken
    Pepperoni
    Bacon Potato



```python
#I like pizza
pizza = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato']
for pizzas in pizza:
    print(pizzas.title() + " is my favorite kind of pizza!")
```

    Bbq Chicken is my favorite kind of pizza!
    Pepperoni is my favorite kind of pizza!
    Bacon Potato is my favorite kind of pizza!



```python
#Adding more lines 
pizza = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato']
for pizzas in pizza:
    print(pizzas.title() + " is my favorite kind of pizza!")
    print("Eating pizza makes me happy everytime. Yum." + " Especially eating " + pizzas.title() + "!\n")
```

    Bbq Chicken is my favorite kind of pizza!
    Eating pizza makes me happy everytime. Yum. Especially eating Bbq Chicken!
    
    Pepperoni is my favorite kind of pizza!
    Eating pizza makes me happy everytime. Yum. Especially eating Pepperoni!
    
    Bacon Potato is my favorite kind of pizza!
    Eating pizza makes me happy everytime. Yum. Especially eating Bacon Potato!
    


## 4-2 Animals
Think of at least three different animals that have a common characteristic. Store the names of these animals in a list, and then use a for loop to print out the name of each animal.

- Modify your program to print a statement about each animal, such as A dog would make a great pet.
- Add a line at the end of your program stating what these animals have in common. You could print a sentence such as Any of these animals would make a great pet!


```python
animal = ['hedgehog', 'chinchilla', 'turtle']
for pets in animal:
    print(pets)
```

    hedgehog
    chinchilla
    turtle



```python
# Statement of each animals
animal = ['hedgehog', 'chinchilla', 'turtle']
for pets in animal:
    print(pets.title() + " will make a great pet!")
```

    Hedgehog will make a great pet!
    Chinchilla will make a great pet!
    Turtle will make a great pet!



```python
# Additional Statement
animal = ['hedgehog', 'chinchilla', 'turtle']
for pets in animal:
    print(pets.title() + " will make a great pet!")
print("These are all rare pets that are hard to take care of.")
```

    Hedgehog will make a great pet!
    Chinchilla will make a great pet!
    Turtle will make a great pet!
    These are all rare pets that are hard to take care of.


## 4-3 Counting to Twenty
Use a for loop to print the numbers from 1 to 20, inclusive.


```python
for value in range(1,21):
    print(value)
```

    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    11
    12
    13
    14
    15
    16
    17
    18
    19
    20


## 4-6 Odd Numbers
Use the third argument of the range() function to make a list of the odd numbers from 1 to 20. Use a for loop to print each number.


```python
odd_numbers = list(range(1,21,2))
print(odd_numbers)
```

    [1, 3, 5, 7, 9, 11, 13, 15, 17, 19]



```python
for odd_number in odd_numbers:
    print(odd_number)
```

    1
    3
    5
    7
    9
    11
    13
    15
    17
    19


## 4-10 Slices: 
Using one of the programs you wrote in this chapter, add several lines to the end of the program that do the following:

- Print the message, The first three items in the list are:. Then use a slice to print the first three items from that program’s list.
- Print the message, Three items from the middle of the list are:. Use a slice to print three items from the middle of the list.
- Print the message, The last three items in the list are:. Use a slice to print the last three items in the list.


```python
pizza_animals = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato', 'hedgehog', 'chinchilla', 'turtle']
print("First three times in the list are: ")
for combined in pizza_animals[0:3]:
    print("\t" + combined.title())
```

    First three times in the list are: 
    	Bbq Chicken
    	Pepperoni
    	Bacon Potato



```python
pizza_animals = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato', 'hedgehog', 'chinchilla', 'turtle']
print("Middle three times in the list are: ")
for combined in pizza_animals[1:4]:
    print("\t" + combined.title())
```

    Middle three times in the list are: 
    	Pepperoni
    	Bacon Potato
    	Hedgehog



```python
pizza_animals = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato', 'hedgehog', 'chinchilla', 'turtle']
print("Last three times in the list are: ")
for combined in pizza_animals[3:]:
    print("\t" + combined.title())
```

    Last three times in the list are: 
    	Hedgehog
    	Chinchilla
    	Turtle


## 4-11 My Pizzas, Your Pizzas: 
Start with your program from Exercise 4-1 (page 60). Make a copy of the list of pizzas, and call it friend_pizzas. Then, do the following:

- Add a new pizza to the original list.
- Add a different pizza to the list friend_pizzas.

Prove that you have two separate lists. Print the message, My favorite pizzas are:, and then use a for loop to print the first list. Print the message, My friend’s favorite pizzas are:, and then use a for loop to print the second list. Make sure each new pizza is stored in the appropriate list.


```python
pizza = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato', 'Hawaiian']
friend_pizzas = ['BBQ Chicken', 'Pepperoni', 'Bacon Potato', 'Cheese']
print(pizza)
print(friend_pizzas)
```

    ['BBQ Chicken', 'Pepperoni', 'Bacon Potato', 'Hawaiian']
    ['BBQ Chicken', 'Pepperoni', 'Bacon Potato', 'Cheese']



```python
print("My favorite pizzas are: ")
for pizzas in pizza:
    print("\t" + pizzas)
```

    My favorite pizzas are: 
    	BBQ Chicken
    	Pepperoni
    	Bacon Potato
    	Hawaiian



```python
print("My friend's favorite pizzas are: ")
for friend in friend_pizzas:
    print("\t" + friend)
```

    My friend's favorite pizzas are: 
    	BBQ Chicken
    	Pepperoni
    	Bacon Potato
    	Cheese

