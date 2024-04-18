# 《30 days to make OS by yourself》source code —— OSASK

[Chinese version](README.md)

Welcome to this work daily to record how I made an OS in 30 days.

## How to run? 
1. create a folder called "run" under folder "tolset".
2. copy the source code from "https://github.com/winnerineast/YOS" into "run".
3. to run "!cons_**.bat" to build.
4. to run "make run" to run it before day 27th.
5. to run "make run_full" to run it starting from day 27th.


## system screenshot

![Screen](Screen.png)

## Content Index

### Week One（day 1 - day 7）

The first thing to think about at the beginning is how to write a "program that runs as soon as the power is turned on". This part is a bit difficult to write in C, so it is mainly written in assembly language.

After this step, the next step is to write a program that reads the operating system from disk. At this point, even if the computer is turned on, it will not automatically read in all the operating system, it can only read the first 512 bytes of content on the disk, so we have to write the rest of the loading program. This program should also be written in assembly language.

Once this step is completed, future programs can be written in C. We will then learn to develop the program for displaying the screen using C as soon as possible. At the same time, we can slowly familiarize ourselves with the C syntax. At this point we seem to be doing what we want to do, but in fact we are not yet free to manipulate the C language.

Next, in order to realize the ambition of "moving the mouse", we have to set up the CPU in detail and master the writing of interrupt handlers. From the overall view of the book, this part of the level is quite high part, I also feel a little bad to put here, but from the organization of the book, these contents must be put here, so I have to ask you to put up with a little. Here, CPU specifications and the complex specifications of the computer will bring us all kinds of trouble. And the fact that the development language is both C and assembly creates even more confusion. At this time, we didn't feel like we were doing what we wanted to do at all, and it seemed like we were "at the mercy of others".

After this painful period, the first week is over.


- [Day 1：Computer Architect to Assembling](https://github.com/yourtion/30dayMakeOS/releases/tag/Day01)
- [Day 2：Assembling and Makefile Introduction](https://github.com/yourtion/30dayMakeOS/releases/tag/Day02)
- [Day 3：Work on 32bit mode and import into C code](https://github.com/yourtion/30dayMakeOS/releases/tag/Day03)
- [Day 4：C Language and Graphics Trying](https://github.com/yourtion/30dayMakeOS/releases/tag/Day04)
- [Day 5：Font and Text Display with GDT IDTInitialization](https://github.com/yourtion/30dayMakeOS/releases/tag/Day05)
- [Day 6：Compile and Interrupt](https://github.com/yourtion/30dayMakeOS/releases/tag/Day06)
- [Day 7：FIFO and Mouse Control](https://github.com/yourtion/30dayMakeOS/releases/tag/Day07)

### Week Two（Day 8 - Day 14）

A week of hard work is still very meaningful, and looking back, we will find that we still have a lot to gain. At this point we have basically mastered the syntax of the C language, and even the level of assembly language can reach the requirements of this book.

So now we can get down to the business of developing a decent operating system. But this time we have another algorithmic headache. Even if you have mastered the syntax of a programming language, if you don't know good algorithms, you still can't develop the operating system you want.

So this week we slowly developed the OS while learning the algorithms. By this stage, though, we could feel largely unencumbered by technical problems.

- [Day 8：Mouse Control and 32bit Mode Switch](https://github.com/yourtion/30dayMakeOS/releases/tag/Day08)
- [Day 9：Memory Management](https://github.com/yourtion/30dayMakeOS/releases/tag/Day09)
- [Day 10：Stack Processing](https://github.com/yourtion/30dayMakeOS/releases/tag/Day10)
- [Day 11：Create Windows](https://github.com/yourtion/30dayMakeOS/releases/tag/Day11)
- [Day 12：Timer（1）](https://github.com/yourtion/30dayMakeOS/releases/tag/Day12)
- [Day 13：Timer（2）](https://github.com/yourtion/30dayMakeOS/releases/tag/Day13)
- [Day 14：High resolution display and keyboard input](https://github.com/yourtion/30dayMakeOS/releases/tag/Day14)

### Week Three（Day 15 - Day 21）
Now that we are quite technologically advanced, we can develop our own operating systems as we wish. The first step is to support multitasking, then develop a command line window, and after that we can get to work on applications.

By the end of the week, we'll be able to come up with a piece of software that we can call an operating system, even if it's not quite complete enough.

- [Day 15：Multitasks（1）](https://github.com/yourtion/30dayMakeOS/releases/tag/Day15)
- [Day 16：Multitasks（2）](https://github.com/yourtion/30dayMakeOS/releases/tag/Day16)
- [Day 17：Commandline](https://github.com/yourtion/30dayMakeOS/releases/tag/Day17)
- [Day 18：dir](https://github.com/yourtion/30dayMakeOS/releases/tag/Day18)
- [Day 19：Application](https://github.com/yourtion/30dayMakeOS/releases/tag/Day19)
- [Day 20：API](https://github.com/yourtion/30dayMakeOS/releases/tag/Day20)
- [Day 21：Protection](https://github.com/yourtion/30dayMakeOS/releases/tag/Day21)

### Week Four（Day 22 - Day 28）
At this stage, we can add all sorts of features to the operating system to our heart's content, as well as develop a large number of decent applications.

At this stage, we can already do very well, and this is probably the period when we are the happiest. There is very little to explain in this section, and the author doesn't have to painstakingly write all those textual explanations, so he can concentrate on programming (laughs).

By the way, speaking of text, I just remembered that we can make our operating system display text during this period.

- [Day 22：Write application in C](https://github.com/yourtion/30dayMakeOS/releases/tag/Day22)
- [Day 23：Graphics Processing](https://github.com/yourtion/30dayMakeOS/releases/tag/Day23)
- [Day 24：Windows Operation](https://github.com/yourtion/30dayMakeOS/releases/tag/Day24)
- [Day 25：Add Commandline Windows](https://github.com/yourtion/30dayMakeOS/releases/tag/Day25)
- [Day 26：Move Windows around](https://github.com/yourtion/30dayMakeOS/releases/tag/Day26)
- [Day 27：LDT and Library](https://github.com/yourtion/30dayMakeOS/releases/tag/Day27)
- [Day 28：File Operation and Text Display](https://github.com/yourtion/30dayMakeOS/releases/tag/Day28)


### Another two days（Day 29 - Day 30）

Bonus application with fun.

- [Day 29：Compress and Simple Application](https://github.com/yourtion/30dayMakeOS/releases/tag/Day29)
- [Day 30：Advanced Application](https://github.com/yourtion/30dayMakeOS/releases/tag/Day30)
