---
layout: default
---
### Developer Bastian

![Unreal Engine 5](/www/assets/images/unreal5.webp)

# Unreal Journey

## A **non-programming approach** to a Survival game based on Unreal Engine and Lyra

I started my Unreal journey mid 2022 and quickly got confused and overwhelmed about the right way to do things. After 6 months, here some learnings:

*	It is easy to get quick results with the Unreal Engine, but they will not scale easily - neither in multiplayer size nor in networking capabilities.   
*   The engine seem to have grown very organically, so I observe a wild mix of concepts that are not really seamlessly fitting into each other.
*   The most advanced concept in terms of scalability and especially segregation of layers such as game logic, animation, networking etc is Unreal Lyra.
*   [Unreal Lyra](https://docs.unrealengine.com/5.0/en-US/lyra-sample-game-in-unreal-engine/) is doing a great job in abstracting layers, but renders nearly all blueprints on the marketplace useless as these do not support said segregation. Also, there is no concept to seel e.g. Gameplay Actions on the Marketplace - this is an extreme oversight from Epics as it would solve the situation that you get a BP from the Marketplcace only to see that it overlaps with many concepts within your own development. 


### Unreal Lyra

Lyra gives you great features out of the box, but is purely documented and not really easy to reuse currently - at least on my current level of understanding.
This pages will document my journey into building a simple survival like "Walking Simulator" using Lyra as a base but only using a **Blueprint** approach - so no programming C++ at all.

Having said that, I **will** show how to set up a programming environment in the background - simply because Lyra actually relies on that and it will be anyway a logical next step on my - and possibly yours - gameplay development path.

**A remark here to all non (C++) developers in regards to Unreal**: 
Epics does a great job to keep the code itself readible and easy to understand. You do actually not need extremely advanced C++ concepts to just understand and reuse the code - so the pure C++ part of it should not really be seen as a blocker - that knowledge you can get easily within a single C++ course.

That makes the challenge in learning to develop Unreal not "I have to learn C++", but "I have to learn "Unreal": The thousends of classes, interfaces, macros, exceptions to "normal" C++ will make your leaning curve long, frustrating and challenging. Here my impression is at least 2 years of effort before being really able to develop stable solutions for Unreal Engine.


