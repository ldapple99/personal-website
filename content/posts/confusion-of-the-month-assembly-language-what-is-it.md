---
layout: blog
title: "Confusion of the Month: x86 Assembly Languages - What are they?"
date: 2023-02-16T23:40:54.579Z
thumbnail: /images/uploads/img_0762.jpeg
categories: Confusion of the Month
tags:
  - Assembly
---
**Hello & Happy February Everyone!** :snowflake:

In my Computer Systems course, this month has been dedicated towards learning and understanding lower-level Assembly Language (specifically x86-64). Although it initially confused me, as I started learning more and more about assembly I realised all of the wonderful benefits it can bring. In the Computer Systems course I am currently in, we used assembly paired with GDB (General GNU Project Debugger) to determine and debug simple programs in C. And although assembly is generally not used to directly debug programs, being able to grasp what assembly is and gain the the knowledge on how to use it can providde a plethora of benefits, including but not limited to:
- better understanding how programs often work at lower-levels
- being able to write smoother performing algorithms
- gaining more knowledge on how Input/Ouput Operations and Buffering actually works
- having the capability of writing more back-end for the compiler
- and many, many more.

Now, I think I should start clearing up something that *I* was initially confused on. What are the differences between Assembly Languages, x86 Assembly Languages, and the x86-64 Assembly Language? (*It's a lot to wrap my head around* :sweat_smile:):

- **Assembly Languages (ASM)**: is *any* programming language that is low-level and has a lot of simularity between it and the machine language that is processed by the Central Processing Unit (CPU) (1)
- **x86 Assembly Languages**: assembly languages that generate x86 machine code for the x86 class of processors. Often these assembly languages use the Intel or AT&T syntax (*in my course, we used the AT&T syntax, but now I am interesting in leraning more about it's differnces from the Intel syntax*) (2)
- **x86-64 Assembly Language (x64 or AMD64)**: is the 64 bit version of the x86/IA32 version mentioned above. This is the language for processors that is most common in most computers (3)



#### References

> 1. “Assembly Language.” Wikipedia, Wikimedia Foundation, Feb. 2023, https://en.wikipedia.org/wiki/Assembly_language. 
> 2. “x86 assembly language.” Wikipedia, Wikimedia Foundation, Feb. 2023, https://en.wikipedia.org/wiki/X86_assembly_language. 
> 3. Woos, Doug. X86-64 Assembly Language Reference, https://cs.brown.edu/courses/csci1260/spring-2021/lectures/x86-64-assembly-language-reference.html. 
> 4.  