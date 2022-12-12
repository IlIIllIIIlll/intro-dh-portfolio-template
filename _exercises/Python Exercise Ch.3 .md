---
layout: page
title: Exercises Ch. 3
description: Introducing Lists
---

## 3-1 Names
Store the names of a few of your friends in a list called `names`. Print each person’s name by accessing each element in the list, one at a time.


```python
list = ['Ashley', 'Eda', 'Elias', 'Aidan']
print(list[0])
print(list[1])
print(list[2])
print(list[3])
```

    Ashley
    Eda
    Elias
    Aidan


## 3-2 Greeting
Start with the list you used in Exercise 3-1, but instead of just printing each person’s name, print a message to them. The text of each message should be the same, but each message should be personalized with the person’s name.


```python
Eda = "Hi " + list[1] + ", " + "do you want some brownies?"
print(Eda)
Elias = "Hi " + list[2] + ", " + "do you want some sanwiches?"
print(Elias)
Aidan = "Hi " + list[3] + ", " + "do you want some milkshakes?"
print(Aidan)
```

    Hi Eda, do you want some brownies?
    Hi Elias, do you want some sanwiches?
    Hi Aidan, do you want some milkshakes?


## 3-3 Your Own List
Think of your favorite mode of transportation, such as a motorcycle or a car, and make a list that stores several examples. Use your list to print a series of statements about these items, such as “I would like to own a Honda motorcycle.”


```python
list = ['BMW','Mercedes-Benz','Maserati', 'Cadillac', 'KIA', 'Hyundai']
print(list)
```

    ['BMW', 'Mercedes-Benz', 'Maserati', 'Cadillac', 'KIA', 'Hyundai']



```python
BMW = "I want to have a " + list[0] + "."
print(BMW)
Maserati = list[2] + " cars are known to be relatively expensive. But I'd like to buy one."
print(Maserati)
KIA = "Did you know? " + list[4] +  " is a Korean car brand."
print(KIA)
```

    I want to have a BMW.
    Maserati cars are known to be relatively expensive. But I'd like to buy one.
    Did you know? KIA is a Korean car brand.


## 3-4 Guest List
If you could invite anyone, living or deceased, to dinner, who would you invite? Make a list that includes at least three people you’d like to invite to dinner. Then use your list to print a message to each person, inviting them to dinner.


```python
list = ['grandmother', 'grandfather', 'dad', 'mom']
print(list)
```

    ['grandmother', 'grandfather', 'dad', 'mom']



```python
grandmother = "Hi " + list[0] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandmother)
grandfather = "Hi " + list[1] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandfather)
dad = "Hi " + list[2] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(dad)
mom = "Hi " + list[3] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(mom)
```

    Hi grandmother! It'd be great if you could come over to have some dinner with me!
    Hi grandfather! It'd be great if you could come over to have some dinner with me!
    Hi dad! It'd be great if you could come over to have some dinner with me!
    Hi mom! It'd be great if you could come over to have some dinner with me!


## 3-5 Changing Guest List
You just heard that one of your guests can’t make the dinner, so you need to send out a new set of invitations. You’ll have to think of someone else to invite. 
- Start with your program from Exercise 3-4. Add a print statement at the end of your program stating the name of the guest who can’t make it.
- Modify your list, replacing the name of the guest who can’t make it with the name of the new person you are inviting.
- Print a second set of invitation messages, one for each person who is still in your list.


```python
#stating who cannot come to the dinner
list = ['grandmother', 'grandfather', 'dad', 'mom']
not_available = list[-1]
message = not_available.title() + " will not be able to come to dinner party."
print(message)
```

    Mom will not be able to come to dinner party.



```python
#Inviting new person
list[3] = 'uncle'
print(list)
```

    ['grandmother', 'grandfather', 'dad', 'uncle']



```python
#printing second set of invitation list
grandmother = "Hi " + list[0] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandmother)
grandfather = "Hi " + list[1] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandfather)
dad = "Hi " + list[2] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(dad)
uncle = "Hi " + list[3] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(uncle)
```

    Hi grandmother! It'd be great if you could come over to have some dinner with me!
    Hi grandfather! It'd be great if you could come over to have some dinner with me!
    Hi dad! It'd be great if you could come over to have some dinner with me!
    Hi uncle! It'd be great if you could come over to have some dinner with me!


## 3-6 More Guests
You just found a bigger dinner table, so now more space is available. Think of three more guests to invite to dinner.
- Start with your program from Exercise 3-4 or Exercise 3-5. Add a print statement to the end of your program informing people that you found a bigger dinner table.
- Use insert() to add one new guest to the beginning of your list.
- Use insert() to add one new guest to the middle of your list.
- Use append() to add one new guest to the end of your list.
- Print a new set of invitation messages, one for each person in your list.


```python
#announcing that I got a bigger table
grandmother = "Hi " + list[0] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandmother)
grandfather = "Hi " + list[1] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandfather)
dad = "Hi " + list[2] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(dad)
uncle = "Hi " + list[3] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(uncle)
new = 'I have a bigger dinner table now!'
print(new)
```

    Hi grandmother! It'd be great if you could come over to have some dinner with me!
    Hi grandfather! It'd be great if you could come over to have some dinner with me!
    Hi dad! It'd be great if you could come over to have some dinner with me!
    Hi uncle! It'd be great if you could come over to have some dinner with me!
    I have a bigger dinner table now!



```python
#adding guest to the beginning of my list
list.insert(0, 'sister')
print(list)
```

    ['sister', 'grandmother', 'grandfather', 'dad', 'uncle']



```python
#adding guest to the middle of my list
list.insert(2, 'brother')
print(list)
```

    ['sister', 'grandmother', 'brother', 'grandfather', 'dad', 'uncle']



```python
#adding guest to the end of my list
list.append('aunt')
print(list)
```

    ['sister', 'grandmother', 'brother', 'grandfather', 'dad', 'uncle', 'aunt']



```python
#printing the new invitation letter
sister = "Hi " + list[0] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(sister)
grandmother = "Hi " + list[1] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandmother)
brother = "Hi " + list[2] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(brother)
grandfather = "Hi " + list[3] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandfather)
dad = "Hi " + list[4] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(dad)
uncle = "Hi " + list[5] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(uncle)
aunt = "Hi " + list[6] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(aunt)
```

    Hi sister! It'd be great if you could come over to have some dinner with me!
    Hi grandmother! It'd be great if you could come over to have some dinner with me!
    Hi brother! It'd be great if you could come over to have some dinner with me!
    Hi grandfather! It'd be great if you could come over to have some dinner with me!
    Hi dad! It'd be great if you could come over to have some dinner with me!
    Hi uncle! It'd be great if you could come over to have some dinner with me!
    Hi aunt! It'd be great if you could come over to have some dinner with me!


## 3-7 Shrinking Guest List
You just found out that your new dinner table won’t arrive in time for the dinner, and you have space for only two guests.

- Start with your program from Exercise 3-6. Add a new line that prints a message saying that you can invite only two people for dinner.
- Use pop() to remove guests from your list one at a time until only two names remain in your list. Each time you pop a name from your list, print a message to that person letting them know you’re sorry you can’t invite them to dinner.
- Print a message to each of the two people still on your list, letting them know they’re still invited.
- Use del to remove the last two names from your list, so you have an empty list. Print your list to make sure you actually have an empty list at the end of your program.


```python
#invite only two people to dinner
sister = "Hi " + list[0] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(sister)
grandmother = "Hi " + list[1] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandmother)
brother = "Hi " + list[2] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(brother)
grandfather = "Hi " + list[3] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(grandfather)
dad = "Hi " + list[4] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(dad)
uncle = "Hi " + list[5] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(uncle)
aunt = "Hi " + list[6] + "!" + " It'd be great if you could come over to have some dinner with me!"
print(aunt)
update = "It turns out, I don't have enough spaces for all of you. I can only invite two now."
print(update)
```

    Hi sister! It'd be great if you could come over to have some dinner with me!
    Hi grandmother! It'd be great if you could come over to have some dinner with me!
    Hi brother! It'd be great if you could come over to have some dinner with me!
    Hi grandfather! It'd be great if you could come over to have some dinner with me!
    Hi dad! It'd be great if you could come over to have some dinner with me!
    Hi uncle! It'd be great if you could come over to have some dinner with me!
    Hi aunt! It'd be great if you could come over to have some dinner with me!
    It turns out, I don't have enough spaces for all of you. I can only invite two now.



```python
print(list)
```

    ['sister', 'grandmother', 'brother', 'grandfather', 'dad', 'uncle', 'aunt']



```python
#using pop method to delete guests
list.pop()
print("Sorry, maybe later we can have dinner together?")
print(list)

list.pop()
print("Sorry, maybe later we can have dinner together?")
print(list)

list.pop()
print("Sorry, maybe later we can have dinner together?")
print(list)

list.pop()
print("Sorry, maybe later we can have dinner together?")
print(list)

list.pop(0)
print("Sorry, maybe later we can have dinner together?")
print(list)
```

    Sorry, maybe later we can have dinner together?
    ['sister', 'grandmother', 'brother', 'grandfather', 'dad', 'uncle']
    Sorry, maybe later we can have dinner together?
    ['sister', 'grandmother', 'brother', 'grandfather', 'dad']
    Sorry, maybe later we can have dinner together?
    ['sister', 'grandmother', 'brother', 'grandfather']
    Sorry, maybe later we can have dinner together?
    ['sister', 'grandmother', 'brother']
    Sorry, maybe later we can have dinner together?
    ['grandmother', 'brother']



```python
print(f"Hi {list[0]}, hi {list[1]}! You are still invited to come over for dinner.")
```

    Hi grandmother, hi brother! You are still invited to come over for dinner.



```python
del list[0]
del list[0]
print(list)
```

    []


## 3-8 Seeing the World

Think of at least five places in the world you’d like to visit.

- Store the locations in a list. Make sure the list is not in alphabetical order.
- Print your list in its original order. Don’t worry about printing the list neatly, just print it as a raw Python list.
- Use sorted() to print your list in alphabetical order without modifying the actual list.
- Show that your list is still in its original order by printing it.
- Use sorted() to print your list in reverse alphabetical order without changing the order of the original list.
- Show that your list is still in its original order by printing it again.
- Use reverse() to change the order of your list. Print the list to show that its order has changed.
- Use reverse() to change the order of your list again. Print the list to show it’s back to its original order.
- Use sort() to change your list so it’s stored in alphabetical order. Print the list to show that its order has been changed.
- Use sort() to change your list so it’s stored in reverse alphabetical order. Print the list to show that its order has changed.


```python
# Storing location in list
location = ['China', 'Netherlands', 'Germany', 'Dubai', 'Morocco']

# Printing the list
print(location)
```

    ['China', 'Netherlands', 'Germany', 'Dubai', 'Morocco']



```python
# Sorting the list in alphabetical order (temporary)
print(sorted(location))
print(location)
```

    ['China', 'Dubai', 'Germany', 'Morocco', 'Netherlands']
    ['China', 'Netherlands', 'Germany', 'Dubai', 'Morocco']



```python
# Sorting the list in reverse alphabetical order
print(sorted(location, reverse=True))
print(location)
```

    ['Netherlands', 'Morocco', 'Germany', 'Dubai', 'China']
    ['China', 'Netherlands', 'Germany', 'Dubai', 'Morocco']



```python
# Using reverse
location.reverse()
print(location)
```

    ['Morocco', 'Dubai', 'Germany', 'Netherlands', 'China']



```python
location.reverse()
print(location)
```

    ['China', 'Netherlands', 'Germany', 'Dubai', 'Morocco']



```python
# Sorting the list in alphabetical order (permanent)
location.sort()
print(location)
```

    ['China', 'Dubai', 'Germany', 'Morocco', 'Netherlands']



```python
location.sort(reverse=True)
print(location)
```

    ['Netherlands', 'Morocco', 'Germany', 'Dubai', 'China']