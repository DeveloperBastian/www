---
layout: default
---
### Developer Bastian

![Developer Bastian](/assets/images/abilities_en.png)

# Lyra Gameplay Abilities 01 - Create and KeyBind[abilities.html](#lyra-gameplay-abilities-and-enhanced-input)
# Lyra Gameplay Abilities 02 - Listen and detect gameplay tag changes in other actors[abilities.html](#lyra-gameplay-abilities-subscripe-to-tag-changes)

## Infographics
[Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)

## Lyra Gameplay Abilities and Enhanced Input
*	Create a simple gameplay ability
*	Extend the Enhanced Input to allow for localized keybindings

## Outcome
A starter to Gameplay abilities - not multi user friendly at this point, just a very basic proof of concept

## Video - english - see link below for german
{% include youtube.html id="S9gZdC_4DOI" %}

## Video Link german
*	[Tutorial de](https://youtu.be/L2pJ7EZgras)


# Thoughts
*	Gameplay Abilities are essential for modern Unreal game development as they decouple pawn from actions. This allows for modular development and avoids blown up character BPs
*	In this tutorial, we focus on how to bind abilities to your Pawn class via a Lyra Ability Set. Furtermore, we dive shortly into the Enhanced Input System to extend the Lyra input bindings with a framework for localized, plugin specific bindings

# Steps (referring to infographic letters)
*	orange E, U, T: 	Create a gameplay ability, add it to the Pawn class
*	orange F-I:			Create a localized Enhanced Input mapping. Bind a gameplay input tag with an gameplay ability via a Lyra Input Config

***

## Lyra Gameplay Abilities Subscripe to Tag changes
*	Create a gameplay tag debugging function
*	Create a material with an exposed parameter to make it glow from a BluePrint
*	Create a listener to gameplay tag changes on all character BPs and react to these

## Outcome
Diving deeper into gameplay abilities and how to use them to communicate between actors

## Video - english - see link below for german
{% include youtube.html id="6m9wgOr8new" %}

## Video Link german
*	[Tutorial de](https://youtu.be/BQVGnqnVfJY)

## Key Concepts
###	Dump Tags: A debug function	to show active gameplay tags per tick
![Lyra Gameplay Tag - Debugging function BluePrint](/assets/images/abilities02_dump_tags.png)

###	How to listen and react to Lyra gameplay tag changes in other actors. This is automatically multi-threaded, easily replicated and extremely low on resources - recommended as standard pattern to organize your in game communication
![Subscribe to changes in gamepay tags of other actors](/assets/images/abilities02_sunscripe_to_gameplay_tag_changes.png.png)