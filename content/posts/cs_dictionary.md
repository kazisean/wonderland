---
title: "( Python ) Dictionaries Notes"
date: 2022-12-18T19:25:52-05:00
tags : ["cs"]
---


# <center>Basics of Python Dictionary </center>

Dictionary is a way to orgazine and maintain our data. A Dictonary is another iterable data structure that is build into pyhton. Kind of similar to llist. But unlike list in dictionary you can store data that relates to one another. 

+ Example of a dictionary 
my_dictonary = {"one" : "Messi", "two": "Ronaldo", "three":"Neymar"}

print(my_dictonary["one"])

Output : 
Messi

From this example we can see that we can print out the value inside a dictionary using their keys. This is very similar to how we would print out list but in list we use numbers where to print out a specific value of dictionary we use the key. Keys could be anything from strings to numbers. 

# What can dictonaries contain ? 

In a dictionary the value of the key can be anything. For example one key could contain a list where inside the same dicitonary another key could hold a string. We just need to make sure that the key it self is either a string or number. 

# How do you print out values inside a multiple dictionary?

Example : 
my_dictonary = {
                                "one" : ["Messi", "Mbappe"], 
                                "two": "Ronaldo", 
                                "three":"Neymar"}

print(my_dictonary["one"][1])

Output : 
Mbappe

In this example we in we can see that there is a list stored inside a key. We can acess different values from list by 

1. First indicating the key value
2. Second indicating the list value

This is very similar to how we would call out a specific value in list. But in this case as you can see we first had to indicate our key and then we have to open a new bracket to indicate the listing index. This is because when indexing each bracket can only hold one single value.




+ Notes to remeber 
In a dictionary we have keys. Each keys have to be a uniqe name. 
In a dictionary the keys are one to one mapping. Meaning that each one is connected to one.
Each key in python only points to one value. 


# <center>Dictionary Methoods</center>
There are some key methoods we must know. 
<center>len</center>
Finds the number of keys the dictionary contains . To use len we can simply use the len() funtion. For example if we wanted to find the len of our privious dicitonary we would do the following. 

my_dictonary = {
                                "one" : ["Messi", "Mbappe"], 
                                "two": "Ronaldo", 
                                "three":"Neymar"}

print(len(my_dictonary))

Output : 
3

In this example we can see how using the len funtion we can find out how many keys are inside a dictionary. 


+ Notes to remeber : 
Remeber that in the len funtion it counts from 1 instade of 0. Just like how we humans count.

<center>get() methood</center>

The get(key) methood returns value associated with a key. For example if we wanted to get all the keys of two inside of our dictionary we would do the following :

my_dictonary = {
                                "one" : ["Messi", "Mbappe"], 
                                "two": "Ronaldo", 
                                "three":"Neymar"}

print(my_dictonary.get("two"))

Output :
Ronaldo

In this example we can see that we can figure our if a key exist using the get methood. If the key doesn't exist the method would return nothing. It would not give us an error. 

<center>keys() methood</center>

This is similar to the get method as before but the keys() method would return all the keys we have stored inside a dictionary. 

my_dictonary = {
                                "one" : ["Messi", "Mbappe"], 
                                "two": "Ronaldo", 
                                "three":"Neymar"}

print(my_dictonary.keys())

Output :

dict_keys(['one', 'two', 'three'])


In this example we can see that in the output first it printed out the dicitonary name and all of the keys that it contained. This is very useful. 

+ Notes to remember 
The keys methood does not take any value inside its bracket. It is simply just a dictionary name dot key() LOL

<center>values() methood</center>

This is very very similar to the keys method but the values method returns all of the values inside of a dictionary. For example: 

my_dictonary = {
                                "one" : ["Messi", "Mbappe"], 
                                "two": "Ronaldo", 
                                "three":"Neymar"}

print(my_dictonary.values())

Output:
dict_values([['Messi', 'Mbappe'], 'Ronaldo', 'Neymar'])

In this example we can see that it printed out all the of values inside of our dictionary. 

<center>pop() method</center>

This pop method returns the value of a key inside of a dictionary after that it deletes that key from the dictionary. For example if we wanted to get rid of "three" in our dicitonary after printing it we could do the following. 

my_dictonary = {
                                "one" : ["Messi", "Mbappe"], 
                                "two": "Ronaldo", 
                                "three":"Neymar"}

print(my_dictonary.pop("three"))
print(my_dictonary)

Output : 

Neymar
{'one': ['Messi', 'Mbappe'], 'two': 'Ronaldo'}

In this example we can see that the pop funtion first printed out the value of the key after that it removed it from the dictionary. 

+ Note
If an  invalid key is send into the pop funtion an error would take place


<center>popitem() method</center>
Lets say that we wanted to remove something from our dictionary but we don't know which one to remove. Using the pop item method we can remove a random key from the dictionary. For example :

my_dictonary = {
                                "one" : ["Messi", "Mbappe"], 
                                "two": "Ronaldo", 
                                "three":"Neymar"}

print(my_dictonary.popitem())
print(my_dictonary)

Output : 
('three', 'Neymar')
{'one': ['Messi', 'Mbappe'], 'two': 'Ronaldo'}

From this output we can see that the popitem method has removed the key three randomly. It has first printed out the key and its value and then removed it. From the next print statement we can see that the key three is gone from our dictionary. 


