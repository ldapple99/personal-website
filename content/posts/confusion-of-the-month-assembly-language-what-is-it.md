---
layout: blog
title: "Confusion of the Month: x86 Assembly Languages - What are they?"
date: 2023-02-16T23:40:54.579Z
thumbnail: /images/uploads/img_0762.jpeg
categories: Confusion of the Month
tags:
  - Assembly
---
## **Hello & Happy February everyone!** :gift_heart:

In my Computer Systems course, this month has been dedicated towards learning and understanding lower-level Assembly Language (specifically x86-64). Although it initially confused me, as I started learning more and more about assembly I realised all of the wonderful benefits it can bring. In the Computer Systems course I am currently in, we used assembly paired with GDB (General GNU Project Debugger) to determine and debug simple programs in C. And although assembly is generally not used to directly debug programs, being able to grasp what assembly is and gain the the knowledge on how to use it can provide a plethora of benefits, including but not limited to:
- better understanding how programs often work at lower-levels
- being able to write smoother performing algorithms
- gaining more knowledge on how Input/Ouput Operations and Buffering actually works
- having the capability of writing more back-end for the compiler
- and many, many more.

Now, I think I should start clearing up something that *I* was initially confused on. What are the differences between Assembly Languages, x86 Assembly Languages, and the x86-64 Assembly Language? (*It's a lot to wrap my head around* :sweat_smile:):

- **Assembly Languages (ASM)**: is *any* programming language that is low-level and has a lot of simularity between it and the machine language that is processed by the Central Processing Unit (CPU) <sup>1</sup>

- **x86 Assembly Languages**: assembly languages that generate x86 machine code for the x86 class of processors. Often these assembly languages use the Intel or AT&T syntax (*in my course, we used the AT&T syntax, but now I am interesting in learning more about it's differnces from the Intel syntax*) (2)

- **x86-64 Assembly Language (x64 or AMD64)**: is the 64 bit version of the x86/IA32 version mentioned above. This is the language for processors that is common in most computers (3) (4)

After clearing up that little confusion, I would've ideally dug deep into what each different type of instruction much like how they were covered in class, such as the jmp (jump), mov (move), and lea (load effective address). If I had, this would turn into more of a chapter in a book than a meer blog post. **But** I can most definitally give a brief cover of some of the more major ones! :smile:

- **jmp (Jump)**: jmp 'jumps' to a new line in the instruction stream, it is often occompanied by a cmp (compare | conditional) that determines if the jump occurs. (4) I like to think of it as little teleportations you see in video games (as you continue down your pathway you will be entering this castle, *but* you'll need 3 stars to jump to this painting to a new level - *any Mario 64 fans out there?* :european_castle:) (5)

- **mov (Move)**: mov 'moves' (*or I more think of it as copies*) over information from the first argument of the instruction over to the second. This is often used to transfer information from two registers. (Following the same video game theme: suppose a character wants to give their friend the same potion they currenly have, so they decide to cook up an identical potion and provide it to their friend) 

- **lea (Load Effective Address)**: Although very simular to mov, lea copies the values of the source itself to the second argument. (So in the case, imagine the character providing the friend with a *recipe* to make the same potion)

- **test (Test)**: This instruction performs a logical AND between the two arguments and sets a flag value (Zero Flag (ZF), Sign Flag (SF), or Parity Flag (PF)) depending on the results. (*I'm racking my head to try and think of a fun video-game way to describe this so if you, the reader, can think of one, please let me know!* :smile:)

- **push and pop (Push & Pop)**: push and pop are instructions that relate to the *stack* (an array-like data structure that is used for temporary storage, I tend to think of stacks as a stack of books in a bookshop). The push instruction 'pushes' data *onto* the stack (so think of a character stacking another layer of ice cream on their ice cream cone). This therefore means that we need a way to remove information from the stack, and this is exactly what the pop instruction does! It 'pops' the information *off of* the stack! (So in this case, a character would scoop off the top-layer of ice cream :icecream:)

- **call (Call)**: The call instruction is often used to 'call' a function. To do this it pushes the return address onto the stack that was previously mentioned, and points the Extended Instruction Pointer (EIP) to the destination. (So the character decides they want to take a break to start racing around the ice cream shop instead of continuing to layering ice cream on their waffle cones. They therefore place a paper holder on top of the ice cream that informs them of where they go at the end of being in the ice cream shop and they call their friends to help them race around the shop :checkered_flag:)

Although there are a plethora of instructions like these that I have skipped over for now, these are the ones that played the largest role during my time working with x86-64 Assembly. Hopefully after reading through this post you have gained a better understanding of what assembly is and perhaps demystified some points that may have confused you like they had for me. If you have any comments or concerns, please and always feel free to contact me using any of the methods below!

Now I think I'll get back to my studies until my new post next month, *but I think I might find myself some ice cream and listen to some nostalgic gaming soundtracks on the way to doing so*. :ice_cream::space_invader:

#### References

> 1. “Assembly Language.” Wikipedia, Wikimedia Foundation, Feb. 2023, https://en.wikipedia.org/wiki/Assembly_language. 
> 2. “x86 assembly language.” Wikipedia, Wikimedia Foundation, Feb. 2023, https://en.wikipedia.org/wiki/X86_assembly_language. 
> 3. Woos, Doug. X86-64 Assembly Language Reference, https://cs.brown.edu/courses/csci1260/spring-2021/lectures/x86-64-assembly-language-reference.html. 
> 4. Bryant, Randal, and David Richard O'Hallaron. Computer Systems: A Programmer's Perspective. 3rd ed., Pearson, 2016. 
> 5. *Super Mario 64*. Nintendo, 1996