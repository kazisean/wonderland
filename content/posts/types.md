---
title: " ( Python ) Format Funtion & Errors"
date: 2022-12-19T08:48:39-05:00
tags : ["cs"]
---

The format funtion takes in 2 argument. The first aurgument is the thing you want to format (a string or number). The second argument would be a pattern want to apply (how you want it to be formated). This second argument is always expressed as a string. It would have to have "". Inside those quotation marks first we need to declare the data type. If the data type is a float inside the "" we need to put an f. 

Example :  format(my_data,"f")

After that if we want to convert the data to 2 decimal places we can do the following. 

Example :  format(my_data,".2f")

+ The format number always returns a string

If we wanted to have a comma after 2 decimal places we can format like the following. 

Example :  format(my_data,",.2f")

# <center>Formating Integers</center>

Example : Example :  format(my_data,",d")

in this case we put d because we assumed that the data type is an integer. 

## <center>Types of Erros and their meaning</center>


Syntax error : A misuse of the python language. It is when for example we forget to put a closing parenthesis on your print statement. 

Runtime Error : A error that takes place during the running of your program. The program does run but at some point it crashes. An example would be diving a number by zero which would give us an invalid answer. 

Logic Error : A type of error where your programs runs fine without crashing but gives you an output which you dont want. Meaning somethign in the code went wrong and giving you the wrong answer. These are the hardest error's to find. 