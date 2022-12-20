---
title: "( Python ) List"
date: 2022-12-19T20:33:19-05:00
tags : ["cs"]
category : ["Class Notes"]
---


# <center>List</center>

When you multiply a list you dublicate them with in that list at the end. Okay this might be confusing. Here is an example : 

exp_list  = [2,3] *2 

print(exp_list)

Output : 
[2,3,2,3]

Now do you see what I mean? Pretty cool. 

+ Index notation is always going to be []

Indexing starts from 0

the len()  funtion when used on a list returns the number of items stored inside that list. It returns a number. 


# <center>Slicing</center>

Example : 

ltr = "Kazi"

print(ltr[0:2])

Output:
Ka

As you can see that this slicing method return the value based on the index number. 

We can also do the same thing with list. 

# How to add a value to an existing list

we can do that by list_name += ["new value"]

This will add the value at the end of the list

+ Make sure to not forget the brackets

We can also add a value at the start of a list by list_name = ["new value"] + list_name

The more eaiser way to do add something to a list is using the append method. 

list_name.append("New value")

+ Notes
The append method takes in one value. 
the append method is parenthesis 
the append method adds at the end of a list 

del my_list[0] this will delete whatever value is at the 0 position of the list.

sort funtion :

my_list.sort() - The sort funtion takes no aurgument and sorts the number in assending order. Meaning from less to bigger number
my_list.reverse() - This funtion takes all the value from the end and put them at the front. It reorders

.index() - This function finds out where a value is in a list. It retuns an integer.

max() - Max number in a list
min() - Min number in a list






