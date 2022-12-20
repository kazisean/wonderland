---
title: "( Python ) Strings and slicing"
date: 2022-12-19T19:09:31-05:00
tags : ["cs"]
category : ["Class Notes"]
---


Indexing starts like this : 

Starts from 0
If we wanted to found from backward the first number would be -9 instade of 0. This is called negative indexing. 
https://cdn.discordapp.com/attachments/966939751280164915/1054567521673551883/image.png
For more info look at this ^

The len funtion returns everything within a string. Even spaces. 

Strings are immutable 

ord() = get the order in the ascii table where the character is
chr() = takes a number as an input and returns the value from the ascii table


capitalize() - It capitalize the first value of the string and makes everything else lower case

lower() - It makes all the values in the string lower case 

is.lower() - Returns a true or false value 

count() - takes in a value and finds out how many of them there are inside the string 

find() - similar to count but this time it returns where the value is in the index of the string

upper() - makes all the values inside of a string upper case

title() - Makes the first letter of every char capital

replace () - Takes in two values. First you need to put the value of the string you want to change and then after the comma you put the new value as a string. 

Example : my_string.replace("kazi","First Name")

This will replace the word kazi from my_string and and replace it with First Name and would print it out. But this does not change the string global. You need to store it as a new varible if you want to do so. 

+ All sequence and strings are Iterable meaning they can be extracted one at a time.

We can iterate over all the values from a string using a for loop. 





