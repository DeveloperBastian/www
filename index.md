---
layout: default
---
### Developer Bastian

![Unreal Engine 5](/www/assets/images/unreal5.webp)

# Unreal Journey

## A **non-programming approach** to a Survival game based on Unreal Engine and Lyra

I started my Unreal journey mid 2022 and quickly got confused and overwhelmed about the right way to do things. After 6 months, here some learnings:

*   The engine seem to have grown very organically, so I observe a wild mix of concepts that are not really seamlessly fitting into each other.
*	It is easy to get quick results with the Unreal Engine, but I miss a clear seperation of game logic, animations, enabling features (networking, scaling, ...) 
*   The most advanced concept in terms of segregation of these layers seems to be is Unreal Lyra - also see [X157](https://x157.github.io/UE5/LyraStarterGame/Pros-and-Cons) for a technial discussionto use it or not
*   So [Unreal Lyra](https://docs.unrealengine.com/5.0/en-US/lyra-sample-game-in-unreal-engine/) is doing a great job in abstracting layers, but now renders nearly all blueprints on the marketplace useless as these do not support said segregation. On the other side, there is no concept to sell these components - e.g. Gameplay Actions - on the Marketplace: This is an extreme oversight from Epics as it would solve the situation that you get a BP from the Marketplace only to see that it overlaps with many concepts within your own development. 

Why do I put so much focus on seperation of game logic, visuals and helper functions? That is the only way to keep things scalable (in terms of team work and technology) and easily adapt to cloud services from my experience. 
This is where the [Gameplay Ability - GAS](https://docs.unrealengine.com/5.1/en-US/using-gameplay-abilities-in-unreal-engine/) feature comes into play: Lyra heavily utlized this, but adds so much quality features to it that we now finally can design GAS driven gameplay without doing any programming - just reusing Lyra BPs and concepts.

### Unreal Lyra

Lyra for me is a toolbox that extends and abstracts the GAS concepts to make them much more user friendly while ensuring scalability and multiplayer. This makes it a great starting point for new games - I honestly don't understand Epic stopping half way and not making this a standard abstracted set of template with better documentation.
And of course supporting this in the marketplace - due to the abstraction level you actually could sell Gameplay Actions that can be connected to all game elements without overwriting any existing logic.

So we face a great concept, with lacking documentation: This pages will document my journey into building a simple survivalgame-like "Walking Simulator" using Lyra as a base but using a **Blueprint-only** approach - so no programming C++ at all.

Having said that, I **will** show how to set up a programming environment in the background - simply because Lyra actually relies on that and it will be anyway a logical next step on my - and possibly yours - gameplay development path.

**A remark here to all non (C++) developers in regards to Unreal**: 
Epics does a great job to keep the code itself readible and easy to understand. You do actually not need extremely advanced C++ concepts to just understand and reuse the code - so the pure C++ part of it should not really be seen as a blocker - that knowledge you can get easily within a single C++ course.

That shifts the challenge into **"Learning the Unreal API/Classes/Macros"** from the more simple **"I have to learn C++"**: The thousends of classes, interfaces, macros, exceptions to "normal" C++ will make your leaning curve long, frustrating and challenging.

Expect more than a year dedication into learning this. Or follow my BP only approach here and let's find out together how far that can get us...


