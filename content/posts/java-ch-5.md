---
title: "Introduction to Java Programming - Chapter 5 (Loops)"
date: 2023-02-25T20:52:20-05:00
tags : ["CS"]
---

## Introduction 
What are loops? 
<br> > Loops are constructs that control repeated execution of a block statements. 

What are the different types of loops in java?
 <>There are three types of loop in java 
1. while loops
2. do-while loops
3. for loops

## Chapter 5.2 : The while loop

What is a while loop?
<br>> A while loop keeps executing while the condition is true.

What does a while loop looks like?
```
    while(loop-condition){
        // Things to do while the loop condition is true
        Statements(s);
    }
```
After successfully running the program once it is known as one iteration (repetition) of the loop.
<br> The loop condition if true would keep running the program where is the condition is false it would terminate the loop and exit. 

<br>What is a counter-controlled loop? 
<br> > A counter-controlled loop is where we know exactly how many times the while loop need to be executed. 
<br> Hence we can setup a variable a first and keep changing that variable through the while and run the loop until the condition value is false. 
<br> Here is an example : 

```
    int count = 0;
    while (count < 100) {
    System.out.printIn("Welcome to Java!");
    count++;
}

```

In this part we first set count = 0. We will update this after each iteration of our while loop. 
Now observer how we used the loop condition. If the count variable is less than 100 which is true the loop runs
In the second line we can see the statement that it does during each iteration. 
*This is important* In this case we are using count ++ to increase the count variable which is outside of the loop. Hence after each iteration the loop would add +1 to the count variable. Which will make the loop control condition false after the program ran 100 times.
The loop condition would no longer be true





