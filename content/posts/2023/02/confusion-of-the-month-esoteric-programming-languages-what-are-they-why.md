---
layout: blog
title: "Confusion of the Month: Esoteric Programming Languages - What are they & why?"
date: 2023-01-18T01:37:36.351Z
thumbnail: /images/uploads/netlifylogo.png
categories: Esoteric PL
tags:
  - Esoteric PLs
  - Esolang
  - Malbolge
  - Chicken (PL)
  - Chef (PL)
  - Piet
  - Intercal
---
## ***Happy January everyone!*** :snowflake:

I thought I'd start off my first ***Confusion of the Month*** - a monthly column that will discuss a topic that I came across that initially bewildered me and how I made sense of it - with a fun subject that I had recently became aware of. This subject being ***Esoteric Programming Languages*** *(aka Esolangs)* and why I am more than glad that I never had an assignment programming in one during my time as an undergraduate student (*so far* I should say, still have 3 months to go till I graduate :eyes:).

### What exactly is an "Esoteric Programming Language"

### Intercal

### Chicken

### Chef

### Piet

### BrainF\*\*k

Now, no blog on Esoteric Programming Languages would be credible without mentioning BrainF&&k. Composed in 1993 by Urban Müller, BrainF&&k is a Esoteric PL that consists of only 8 language commands: < > + - . , \[ and ] 

Many complain about the language's commands ususally have no hints as to what they mean, making it quite challenging to decipher. For example , the command , means to accept one byte of the input and store it in the data pointer. This along with the nature of the programming needing long sequences of characters to create the simplest of operations (the language is made such that the commands < and > increment or decrement the data pointer to a differing cell of memory and the commands + and - both increase and decrease the byte stored at that cell), creates a plethora of reasoning as to why the PL is usually refered to as a parody and is never truly used outside of amusement. 

~~~
++++++++[>++++[>++>+++>+++>+<<<<-]>+>+>->>+[<]<-]>>.>---.+++++++..+++.>>.<-.<.+++.------.--------.>>+.>++.
~~~

The above code snippet prints out your standard "Hello World" following with a new-line, in Brainf&&k

### Malbolge

Named after the 8th Circle of Hell in Dante Alighieri's Inferno, this programming language truly lives up to the name. In 1998, Ben Olmstead purposely created this programming language to be nearly impossible to design. For starters, Malbolge has only three registers - a (accumulator), c (code pointer), and d (data pointer)- and works in for a *terary* VM. Much like Brainf&&k, Malbolge also has only 8 language commands, although with a *twist*.  Malgbolge determines which instruction to tell the interpretor what to do by determining the value of:
~~~
([c] + c) % 94
~~~

when c is the code pointer. Although, after each instruction is executed the instruction get encrypted using what is called *Crazy Operation* such that it will not tell the interpretor the same thing the next time it is called. 

Although it took **2 years** to find a way to do so with the help of the Lisp program that used a local beam search, below is the standard "Hello World" program in Malbolge.
~~~
(=<`#9]~6ZY327Uv4-QsqpMn&+Ij"'E%e{Ab~w=_:]Kw%o44Uqp0/Q?xNvL:`H%c#DD2^WV>gY;dts76qKJImZkj
~~~

### Conclusion

So all-in-all, most Esoteric Programming Languages are there to just to poke fun at the very nature of various programming languages and are there for amusement. Although after learning about them, I am now able to think "At least I didn't have to program this in *Chicken*" after finishing up any challenges in my future as a programmer. :satisfied: :chicken: