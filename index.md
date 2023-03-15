---
layout: default
---
### Developer Bastian

![Unreal Engine 5](/www/assets/images/unreal5.webp)

# Unreal Journey

## A **non-programming approach** to a Survival game based on Unreal Engine and Lyra

I started my Unreal journey mid 2022 and quickly got confused and overwhelmed about the right way to do things. 
After 6 months, I decided to document my way to a simple survival multiplayer game, fully based on Unreal Lyra - as recommended as a basis for new games.

This will be a **Blueprint-only** approach, no C++ required. Having said that, I **will** show how to set up a programming environment in the background - simply because Lyra actually relies on that and it will be anyway a logical next step on my - and possibly yours - gameplay development path.
Expect more than a year dedication into learning this. Or follow my BP only approach here and let's find out together how far that can get us...

## Documentation
I will document everything

*   here on this website
*	on a summary [Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)
*	on the [Youtube channel] (https://www.youtube.com/@bastiandev/videos)
*	on my [Discord channel] (https://discord.gg/ZTHqvZNEqB)
*	on the [Unreal forum] (https://forums.unrealengine.com/u/bastiandev)
*	on [Twitter] (https://twitter.com/BastianDevelop)

## Why using Unreal Lyra?
The most advanced concept in terms of segregation of  layers seems to be is Unreal Lyra - also see [X157](https://x157.github.io/UE5/LyraStarterGame/Pros-and-Cons) for a technial discussionto use it or not
*   So [Unreal Lyra](https://docs.unrealengine.com/5.0/en-US/lyra-sample-game-in-unreal-engine/) is doing a great job in abstracting layers, but now renders nearly all blueprints on the marketplace useless as these do not support said segregation. On the other side, there is no concept to sell these components - e.g. Gameplay Actions - on the Marketplace: This is an extreme oversight from Epics as it would solve the situation that you get a BP from the Marketplace only to see that it overlaps with many concepts within your own development. 

Why do I put so much focus on seperation of game logic, visuals and helper functions? That is the only way to keep things scalable (in terms of team work and technology) and easily adapt to cloud services from my experience. 
This is where the [Gameplay Ability - GAS](https://docs.unrealengine.com/5.1/en-US/using-gameplay-abilities-in-unreal-engine/) feature comes into play: Lyra heavily utlized this, but adds so much quality features to it that we now finally can design GAS driven gameplay without doing any programming - just reusing Lyra BPs and concepts.

## Lyra as toolbox
Lyra for me is a toolbox that extends and abstracts the GAS concepts to make them much more user friendly while ensuring scalability and multiplayer. This makes it a great starting point for new games - I honestly don't understand Epic stopping half way and not making this a standard abstracted set of template with better documentation.
And of course supporting this in the marketplace - due to the abstraction level you actually could sell Gameplay Actions that can be connected to all game elements without overwriting any existing logic.




