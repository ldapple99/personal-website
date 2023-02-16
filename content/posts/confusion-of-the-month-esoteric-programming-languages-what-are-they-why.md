---
layout: blog
title: "Confusion of the Month: Esoteric Programming Languages - What are they & why?"
date: 2023-01-18T01:37:36.351Z
thumbnail: /images/uploads/netlifylogo.png
categories: Confusion of the Month
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

### What exactly is an "Esoteric Programming Language"? :thinking:

Before diving into some of my favourite esoteric programming languages (*aka esolangs*), I think it will be worthwhile to discuss what it actually means for a programming langauge to be considered *esoteric*. Usually esoteric programming languages are written as parodies to the natures of widely-used programming languages (such as C#, FORTRAN). Although they can also be composed to test the boundries of programming language design, to create art, or even to generate a hacking interface to another language. Usually (and often thankfully), esolangs are not designed for serious programming. :relieved:

### INTERCAL

Designed by two Princeton University students, Don Woods and James M. Lyon, in 1972, INTERCAL (*aka the Compiler Language With No Pronounceable Acronym*) was originally designed as a satire on the structures of the programming languages that were there at the time (mainly FORTRAN). Most of the design choices in composing INTERCAl was chosen such to make the programmer's life as unpleasing as possible when using it by including statements such as `READ OUT` , `IGNORE`, or `FORGET`. I think one of the most interesting design choices in INTERCAL is the `PLEASE` modifier, which if not used enough in a program causes the rejection by the compiler with an error stating that the program is considered "*insufficiently polite*". *Meanwhile* if the `PLEASE` modifier is used too often, then that is grounds for another compiler rejection with an error of the program is considered "*excessively polite*".

Here is the standard "Hello World" program written in INTERCAL:
~~~
DO ,1 <- #13
PLEASE DO ,1 SUB #1 <- #238
DO ,1 SUB #2 <- #108
DO ,1 SUB #3 <- #112
DO ,1 SUB #4 <- #0
DO ,1 SUB #5 <- #64
DO ,1 SUB #6 <- #194
DO ,1 SUB #7 <- #48
PLEASE DO ,1 SUB #8 <- #22
DO ,1 SUB #9 <- #248
DO ,1 SUB #10 <- #168
DO ,1 SUB #11 <- #24
DO ,1 SUB #12 <- #16
DO ,1 SUB #13 <- #162
PLEASE READ OUT ,1
PLEASE GIVE UP
~~~

### CHICKEN

Do you only know one word? And it is 'chicken'? 
Well, you're in luck! Created by Torbjörn Söderstedt, CHICKEN is a PL with only two language commands: `chicken` and `\n`

Basically, the number of `chicken` you write before a new line corresponds to a different instruction to the interpreter. So for example, if you type 4 chickens before a new line then you called a *rooster* instruction which does your standard *multiply* command. 7 chickens and you get a *peck* instruction which corresponds to the standard *store* command. 

Here is your standard "Hello World" program in CHICKEN:

```
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken
chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken

chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken

chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken
chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken

chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken

chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken

chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken chicken
chicken chicken chicken chicken chicken chicken
```

...I don't think I need to say much else. :chicken:

### Chef

Would you like to take the CHICKEN programming language and put it in the oven for a nice Roasted Chicken? :cook: Then I think you'd like to learn more about the Chef programming language which was designed by David Morgan-Mar in 2002!

Chef is an esolang that structures programs (or should I say *recipes*) to follow the same formatting as usual cooking recipes with a Recipe Title, Cooking Time, Ingredients List (that hold different data values), and even Oven Temperatures. This is all followed by a Methods Section that hosts a plethora of instructions such as `Take *ingredient* from refrigerator.` (reads the numeric value from STDIN of the ingredient) or `Serve with *auxiliary-recipe* .` (which involks the *sous chef* to follow another *cooking recipe*). 

Here is the recipe for the *Hello World Cake with Chocolate Sauce* written by David Morgan-Mar to follow for a nice dessert for your roasted chicken. :chocolate_bar::cake:

```
Hello World Cake with Chocolate sauce.

This prints hello world, while being tastier than Hello World Souffle. The main
chef makes a "Hello world!" cake, which he puts in the baking dish. When he gets the
sous chef to make the "Hello" chocolate sauce, it gets put into the baking dish
and then the whole thing is printed when he refrigerates the sauce. When
actually cooking, I'm interpreting the chocolate sauce baking dish to be
separate from the cake one and Liquify to mean either melt or blend depending on
context.

Ingredients.
33 g chocolate chips
100 g butter
54 ml double cream
2 pinches baking powder
114 g sugar
111 ml beaten eggs
119 g flour
32 g cocoa powder
0 g cake mixture

Cooking time: 25 minutes.

Pre-heat oven to 180 degrees Celsius.

Method.
Put chocolate chips into the mixing bowl.
Put butter into the mixing bowl.
Put sugar into the mixing bowl.
Put beaten eggs into the mixing bowl.
Put flour into the mixing bowl.
Put baking powder into the mixing bowl.
Put cocoa  powder into the mixing bowl.
Stir the mixing bowl for 1 minute.
Combine double cream into the mixing bowl.
Stir the mixing bowl for 4 minutes.
Liquefy the contents of the mixing bowl.
Pour contents of the mixing bowl into the baking dish.
bake the cake mixture.
Wait until baked.
Serve with chocolate sauce.

chocolate sauce.

Ingredients.
111 g sugar
108 ml hot water
108 ml heated double cream
101 g dark chocolate
72 g milk chocolate

Method.
Clean the mixing bowl.
Put sugar into the mixing bowl.
Put hot water into the mixing bowl.
Put heated double cream into the mixing bowl.
dissolve the sugar.
agitate the sugar until dissolved.
Liquefy the dark chocolate.
Put dark chocolate into the mixing bowl.
Liquefy the milk chocolate.
Put milk chocolate into the mixing bowl.
Liquefy contents of the mixing bowl.
Pour contents of the mixing bowl into the baking dish.
Refrigerate for 1 hour.
```

### Piet

Not much of a Chef? That's okay! How about art? :artist:

Much like Chef, Piet (named after the famed artist, Piet Mondrian) is an esolang that is also written by David Morgan-Mar that is considered Turing-complete (same computational class as a Turing Machine). Although this time you'll be *painting* an *abstract painting* from 20 various *colours* you can choose from, 18 of them having various *hues*. Using a direction pointer (DP) that can be one of the 4 cardinal directions (up, down, left, right), the Piet program runs until it terminates. Commands are run depending on the change in lightness and hue of the colour that the DP is currently on. 

![Here is one of many implementations of the standard "Hello World" program in Piet](/images/uploads/piet_hello_world.gif "Here is one of many implementations of the standard \"Hello World\" program in Piet")



### BrainF\*\*k

Now, no blog on Esoteric Programming Languages would be credible without mentioning BrainF&&k. Composed in 1993 by Urban Müller, BrainF&&k is a Esoteric PL that consists of only 8 language commands: < > + - . , [ and ]

Many complain about the language's commands usually have no hints as to what they mean, making it quite challenging to decipher. For example , the command `,` means to accept one byte of the input and store it in the data pointer. This along with the nature of the programming needing long sequences of characters to create the simplest of operations (the language is made such that the commands `<` and `>` increment or decrement the data pointer to a differing cell of memory and the commands `+` and `-` both increase and decrease the byte stored at that cell), creates a plethora of reasoning as to why the PL is usually referred to as a parody and is never truly used outside of amusement. 

```
++++++++[>++++[>++>+++>+++>+<<<<-]>+>+>->>+[<]<-]>>.>---.+++++++..+++.>>.<-.<.+++.------.--------.>>+.>++.
```

The above code snippet prints out your standard "Hello World" following with a new-line, in Brainf&&k

### Malbolge

Named after the 8th Circle of Hell in Dante Alighieri's Inferno, this programming language truly lives up to the name. In 1998, Ben Olmstead purposely created this programming language to be nearly impossible to design. For starters, Malbolge has only three registers - `a` (accumulator), `c` (code pointer), and `d` (data pointer)- and works in for a *ternary* VM. Much like Brainf&&k, Malbolge also has only 8 language commands, although with a *twist*.  Malgbolge determines which instruction to tell the interpreter what to do by determining the value of:

```
([c] + c) % 94
```

when c is the code pointer. Although, after each instruction is executed the instruction gets encrypted using what is called *Crazy Operation* such that it will not tell the interpreter the same thing the next time it is called. 

Although it took **2 years** to find a way to do so, with the help of the Lisp program that used a local beam search, below is the standard "Hello World" program in Malbolge.

```
(=<`#9]~6ZY327Uv4-QsqpMn&+Ij"'E%e{Ab~w=_:]Kw%o44Uqp0/Q?xNvL:`H%c#DD2^WV>gY;dts76qKJImZkj
```

### Conclusion

So all-in-all, most Esoteric Programming Languages are there to just to poke fun at the very nature of various programming languages and are there for amusement. Although after learning about them, I am now able to think "At least I didn't have to program this in *CHICKEN*" after finishing up any challenges in my future as a programmer. :satisfied: :chicken: