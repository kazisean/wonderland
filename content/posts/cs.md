---
title: "( Python ) Object Oriented Programming "
date: 2022-12-16T12:25:30-05:00
tags : ["cs"]
---

<!-- <details>
<summary>Vocabulary</summary>

```
print - outputs

```
</details> -->

<!-- # 	 <center>Intro to Programming ( Python) Notes </center> -->
### <center>Introduction to Object Oriented Programming</center>

OOP or Object Oriented Programming is similar to funtions. 

A funtion - is a collection of commands and data. <br>
OOP -  is a collecton of funtions and data. 

In short OOP can contain mutiple funtions within a class. This causes the program to run more smoothly, with less life of codes and can be updated very easily.


### <center>Classes, Properties & Instances</center>

###  So what is a class ? 

<p>A class is basically like a blurprint or template for creating objects. A class can contain mutiple funtions inside of them. A class is nothing more than a design document. For example look at the code below :  </p>

<pre><code>
class name:
    first_name="wonder"
    last_name="land"

name_a=name()
print(name_a)


</code></pre>

<p>If you end up running this code we would prob see something similar to this >> </p>

<pre><code>
<__main__.name object at 0x7fa74d47fca0>

</code></pre>

###  So what happend?

<p>You might be wondering what has happend with this output. This output clearly doesn't make any sense. Well lets start from the start to figure out what this output is. You see what are wrote "class name:" we have created a new class called name. Remeber that  every class you make in a program has to be a different name or it will cause errors while running. Anyways back to the code. Under the class name we have created two variables caleed first_name and last_name. These two varibles contains two different strings. When we look at the next line of code we can see that we created a new varible called name_a. What name_a does is call upon the class "name". Which is why as you can see the value inside name_a is name(). This is calling the class name. On the next line we can see that we print the output of name_a. Which led us to this we looking __main__ thing as the output. Well this main thing is saying that there is an object or class created at the memory location of your computer 0x7fa74d47fca0. For now in short since we only called the class and we only printed out the memory location of that class object. If we wanted to print out lets say first name for example we would have to write the following. </p>


<pre><code>
class name:
    first_name="wonder"
    last_name="land"

name_a=name()
print(name_a.first_name)


</code></pre>

### This will give us the output : 

<pre><code>
wonder

</code></pre>

<p>Which is what we wanted. Now to sum up everything that has happend in that print statement we can say that: </p>

1. We told the computer to go that memory locaiton (<__main__.name object at 0x7fa74d47fca0>)
2. After going to that memory location look for a varible called first_name.
3. Lastly print out the value of first_name.

<p>Very cool. This ia a very basic example but you get the point. </p>


## Notes to remember: 
By default Instance Variables are  mutable or can be changed. 

# what I mean by this?
<p> ok here is an example using the old code.</p>



### <center>Object Constructors</center>


### <center>Instance Methods</center>

