---
layout: page
title: Basic Python (Variables, Strings, Numbers, Lists)
description: This notebook has codes about variables, strings, numbers and lists. 
---

# Variables


```python
greeting = "Hello World!"
```


```python
print(greeting)
```

    Hello World!



```python
sleep = "I am very sleepy right now."
```


```python
print(sleep)
```

    I am very sleepy right now.



```python
sleep = "She is very sleepy right now."
print(sleep)
```

    She is very sleepy right now.


## Notes about Variables
* Variables cannot start with number, it cannot contain a space, and it cannot contain a hyphen. 
* They should be short but descriptive.
* Underscore, number, and letters are available to use. 


```python
ex_1 = "This is a string."
print(ex_1)
```

    This is a string.



```python
ex_2 = 'This is also a string.'
print(ex_2)
```

    This is also a string.



```python
ex_3 = "Here is a string.'
print(ex_3)
```


      Input In [8]
        ex_3 = "Here is a string.'
                                  ^
    SyntaxError: EOL while scanning string literal




```python
ex_4 = 'I asked the question, "When should I use single quotes."'
print(ex_4)
```

    I asked the question, "When should I use single quotes."



```python
historian = "edward gibbon"
print(historian)
```

    edward gibbon



```python
print(historian.title())
```

    Edward Gibbon



```python
print(historian.title)
```

    <built-in method title of str object at 0x7fac2a60e530>



```python
novelist = "Becky Chambers"
print(novelist.lower())
```

    becky chambers



```python
"becky" == "becky"
```




    True




```python
"becky" == "Becky"
```




    False




```python
first_name = "ada"
last_name = "lovelace"
```


```python
full_name = first_name + " " + last_name
print(full_name)
```

    ada lovelace



```python
greeting = f"Hello, {first_name} {last_name}"
print(greeting)
```

    Hello, ada lovelace



```python
greeting = f"Hello, {first_name} {last_name}"
print(greeting.title())
```

    Hello, Ada Lovelace


## Whitespace


```python
print("tab")
```

    tab



```python
print("\ttab")
```

    	tab



```python
print("Languages: \nGreek\nLatin\nEnglish")
```

    Languages: 
    Greek
    Latin
    English



```python
str_rspace = "string     "
print(str_rspace)
```

    string     



```python
print(str_rspace.rstrip())
```

    string



```python
example = str_rspace + "."
print(example)
```

    string     .



```python
example_2 = str_rspace.rstrip() + "."
print(example_2)
```

    string.


## Numbers


```python
# integers
238+4834
```




    5072




```python
19-7
```




    12




```python
54*16
```




    864




```python
43/6
```




    7.166666666666667




```python
num = 45
num
```




    45




```python
num+5
```




    50




```python
type(num)
```




    int




```python
30/10 # this will return a float
```




    3.0




```python
f = 30/7
```


```python
f
```




    4.285714285714286




```python
type(f)
```




    float




```python
3**3
```




    27



## Lists


```python
subjects = ['classics', 'history', 'philosophy']
```


```python
print(subjects)
```

    ['classics', 'history', 'philosophy']



```python
print(subjects[0])
```

    classics



```python
print(subjects[-1])
```

    philosophy



```python
message = f"My most difficult subject is {subjects[1].title()}."
print(message)
```

    My most difficult subject is History.



```python
# how to modify a list
print(subjects)
```

    ['classics', 'history', 'philosophy']



```python
subjects[1] = 'sociology'
```


```python
print(subjects)
```

    ['classics', 'sociology', 'philosophy']



```python
# append
subjects.append('history')
print(subjects)
```

    ['classics', 'sociology', 'philosophy', 'history', 'history']



```python
subjects.append('mathematics')
print(subjects)
```

    ['classics', 'sociology', 'philosophy', 'history', 'history', 'mathematics']



```python
# insert
subjects.insert(0, 'religion')
print(subjects)
```

    ['religion', 'classics', 'sociology', 'philosophy', 'history', 'history', 'mathematics']



```python
subjects.insert(2, 'chemistry')
print(subjects)
```

    ['religion', 'classics', 'chemistry', 'sociology', 'philosophy', 'history', 'history', 'chemistry', 'mathematics']



```python
# delete items from a list
del subjects[5]
```


```python
print(subjects)
```

    ['religion', 'classics', 'chemistry', 'sociology', 'philosophy', 'history', 'chemistry', 'mathematics']



```python
del subjects[-2]
print(subjects)
```

    ['religion', 'classics', 'chemistry', 'sociology', 'philosophy', 'history', 'mathematics']



```python
# pop method
popped_subject = subjects.pop(0)
print(popped_subject)
print(subjects)
```

    classics
    ['chemistry', 'sociology', 'philosophy', 'history', 'mathematics']



```python
# remove
subjects.remove('sociology')
print(subjects)
```

    ['chemistry', 'philosophy', 'history', 'mathematics']



```python

```
