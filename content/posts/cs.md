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

In short OOP can contain mutiple funtions within a class. This causes the program to run more smoothly, with less line of codes and can be updated very easily.


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
<p> ok here is an example using the old code. If we wanted to change our first_name we can simply do so. </p>

<pre><code>
class name:
    first_name="wonder"
    last_name="land"

name_a=name()
print(name_a.first_name)

name_a.first_name = "Kazi"
print(name_a.first_name)


</code></pre>

### This will give us the output : 

<pre><code>

wonder
Kazi

</code></pre>

<p>Notice the first time we printed the output of name_a.first_name we got wonder which is from the class. And the second time we printed the output we told the computer that name_a.first_name has the value "Kazi". And it printed out Kazi. So in short you can change instance variables anyway you want.</p>


### <center>Object Constructors</center>

def __init__ (self)

The init argument has to accept atleast one argument . Which in this case is self. In every init funtions self has to be there. The init funtions triggers automatically upon creation of a new instance for example.  C = cash() if cash was a class with a innit funtion inside. 

+ But what is self?

Self is just a memory location just like we discusssed before. We need to call self because everytime we run the funtion inside of the class the computer needs to know what memory adress to look for. And self provides that memory adress. Memory adress can be different time to time. It is only same while you are running the program. The self in the init funtions holds the same memory adress as the class. 

Object constructors are similar to the funtions we have learned in the previous notes. Except we have to have self at the start. But the only differance is that for example : 

class cool: 
    def __init__( self, x, y ):
        self.x = x
        self.y= y

z = cool(12, 13)

print(z.x, z.y)

Output : 12  13

In this case notice how we can just give out class the value and it would simply give us the output we wanted which is both the value of x and y. we didn't have to assing any values inside the class itself. Now this is a very easy example but you get the point. You can make it do complicated math problem using these structures so easy without tempting with different funtions at different times. Everything is just done in one place at one time.   


# + Notes to remeber : 

Classes are blue prints. They are orgranized pattern for a complicated piece of data. 

Inside of a class we can have funtions. 

A constructor is an object that runs the first time an object is created.

The __init__ funtions job is to act as a constructor. 

The __init__ funtion always takes ATLEAST one argument. Which is a referance to the object that is being created memory adress. 

You can have as many argument inside the __init__ funtions you want. But you must atleast have one argument. 

All the funtions inside of a class needs to have atleast one argument. which is self. This is not only limited to the __init__ funtions but any funtions that is beign created inside of that class. 

Remeber that you can class different funtions inside of a class. For example lets say you have a funtion inside of a class that takes in the input first and last name. You also have a different funtion that determines that persons net worth. In the second funtion you can call the first funtion to get the name and print out for example lets say " Habib's Net Worth is $8M". In this case you didn't really have to do much to get the first name you just called the first funtion which already have done that. 

Remember that when in the second funtion you call the first funtion you must use the . syntax. Meaning for exmaple from our previous exmaple if we want need the x value in our second funtion we need to write self.x = x. Example : 
class cool: 
    def __init__( self, x, y ):
        self.x = x
        self.y= y

    def double(self):
        total = self.x * self.x 
        print(total)

z = cool(12, 13)

print(z.x, z.y)

Hope you understad the way we structure it. It is very imporant for the variable to exist before you call it in your second funtion. 

You can call a single funtion from the class using the . syntax. For example using our old example we can just print the double. By saying z.double(). 

