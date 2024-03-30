---
title: "Week 11"
date: 2024-03-17T21:29:49+01:00
draft: false
---

# Refactoring
So, this will be my first entry that's actually been on time in awhile.

I spent the entire week refactoring the zombie enemy's blueprint logic into C++. Overall this was a straightforward process, what made it difficult is just figuring out some of the unique things that must be done in order to translate otherwise "simple" nodes into C++.

One notable example is how timers are utilized in BP vs C++. In BP, timers are fairly straightforward since blueprints has essentially aabstracted much of the boilerplate code away. But in C++, in order to get a timer to work, several steps are required.

However, like most things that I encounter, it seems really daunting at first. But after wrestling with the idea for awhile, I think it's become more comfortable.

Another major area of paint (something that took me several hours) was ensuring that pointers were all checked prior to using them. I had gotten sloppy and as such my game kept crashing. Lesson learned: when using pointers, always check to see if they are valid.

# Next Up
For this next week I would like to translate the apply damage logic from BP to C++. After that I will probably try and implement a simple version of the zombie dfense game.

Not entirely sure which systems I will try to include, but ideally I would add at leaast a few more in alignment with the game project I have with my partner-in-gamedev so that I get the practice in. Until next time!

P.S. I've been using my glove80 this entire time, and while I am far more productive on a "normal" keyboard, I am definitely becoming more proficient with this guy.