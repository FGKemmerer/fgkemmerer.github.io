---
layout: post
title: 1.2 Fahrenheit and Celsius
---

If Hello World gives a first illusion of awareness, then this conversion table program gives the first glimmer of rational thought. It also seems fitting that the first useful program would be somehow transformative. In some ways, this experience and journey are transformative for me too. 

As an introductory program that “does something” the K&R introduces the reader to formulaic expressions with a simple equation for converting (transforming) Celsius to Fahrenheit. 

In terms of the gcc, the code provided by the K&R for the initial conversion is right on point and runs flawlessly. Likewise, the exercises used here are simple. Inserting a heading and flipping the conversion from Celsius to Fahrenheit.  

While the gcc has little to no problems here, there is a lot of material here and the learning curve begins. It took me about 3 hours to fully grasp everything here. 

Notably, the basic data types discussed are not immediately obvious to the uninitiated (but I suspect this is a newbie problem). These are: 

    Integer (int)
    Floating Point (float)
    Character (char)
    Short Integer (short)
    Long Integer (long)
    Double-Precision Floating Point (double)

Other data types are also hinted at, but I suspect these have their own explanations later. 

At this point, I needed to play a bit with these to try and wrap my head around what is going on. In terms of pure language I can understand these data types as almost word types (noun, verb, adjective, etc). There are appropriate times and places for each, but not for others. For instance, if I simply need a single character (one byte) worth of data for something, the most appropriate is char. However, if I needed to do work with fractional numbers/decimals, I would need to use at least float (or possibly double). 

Data types aside, this is my first exposure to the idea of loops. They make logical sense, but are hard to visualize (at least for now). The K&R makes good use of the lesson here too. After introducing loops, they demonstrate the data type concepts by switching the data type from int to float. 

As it happens, the gcc behaves as expected and int rounds the numbers out while float gives degrees more accuracy. There is one critical line here that merits consideration: 


    “If an arithmetic operator has integer operands, an integer operation is performed. 
    If an arithmetic operator has one floating-point operand and one integer operand, 
    however, the integer will be converted to floating point before the operation is done.”

Meaning, that integer data types are treated almost like “X.00000”. A quick check with the gcc verifies this. By leaving the step, higher and lower bounds as integers and changing the celscius and fahrenheit data type to float (and operands from d% to f%), the data type output is float also (but the reverse is not true).

What remains unclear to me is if this is an effective way to save memory or a lazy work around where float should have been used for both pieces of data.
 
