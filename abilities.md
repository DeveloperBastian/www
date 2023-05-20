---
layout: default
---
### Developer Bastian

<img src="{{site.url}}/www/assets/images/abilities_en.png" style="display: block; margin: auto;" class="medium-zoom-image" />

### [Lyra Gameplay Abilities - Create and KeyBind](#lyra-gameplay-abilities-and-enhanced-input)
### [Lyra Gameplay Abilities 01 - Listen and detect gameplay tag changes in other actors](#lyra-gameplay-abilities-subscripe-to-tag-changes)
### [Lyra Gameplay Abilities 02 - Create an Gameplay Ability Template and understand its components](#lyra-gameplay-abilities-components-and-template)
### [Lyra Gameplay Abilities 03 - Get an Ability through interation with your environment](#lyra-gameplay-abilities-through-the-environment)
### [Lyra Gameplay Abilities 04 - Understanding Cues, Effects and Cooldowns](#effects-cues-and-cooldowns)

## Infographics
[Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)

## Lyra Gameplay Abilities and Enhanced Input
*	Create a simple gameplay ability
*	Extend the Enhanced Input to allow for localized keybindings

### Outcome
A starter to Gameplay abilities - not multi user friendly at this point, just a very basic proof of concept

### Video - english - see link below for german
{% include youtube.html id="S9gZdC_4DOI" %}

### Video Link german
*	[Tutorial de](https://youtu.be/L2pJ7EZgras)


### Thoughts
*	Gameplay Abilities are essential for modern Unreal game development as they decouple pawn from actions. This allows for modular development and avoids blown up character BPs
*	In this tutorial, we focus on how to bind abilities to your Pawn class via a Lyra Ability Set. Furtermore, we dive shortly into the Enhanced Input System to extend the Lyra input bindings with a framework for localized, plugin specific bindings

### Steps (referring to infographic letters)
*	orange E, U, T: 	Create a gameplay ability, add it to the Pawn class
*	orange F-I:			Create a localized Enhanced Input mapping. Bind a gameplay input tag with an gameplay ability via a Lyra Input Config

***

## Lyra Gameplay Abilities Subscripe to Tag changes
*	Create a gameplay tag debugging function
*	Create a material with an exposed parameter to make it glow from a BluePrint
*	Create a listener to gameplay tag changes on all character BPs and react to these

### Outcome
Diving deeper into gameplay abilities and how to use them to communicate between actors

### Video - english - see link below for german
{% include youtube.html id="6m9wgOr8new" %}

### Video Link german
*	[Tutorial de](https://youtu.be/BQVGnqnVfJY)

### Key Concepts
####	Dump Tags: A debug function	to show active gameplay tags per tick
![Lyra Gameplay Tag - Debugging function BluePrint](/assets/images/abilities02_dump_tags.png)

####	How to listen and react to Lyra gameplay tag changes in other actors. This is automatically multi-threaded, easily replicated and extremely low on resources - recommended as standard pattern to organize your in game communication
![Subscribe to changes in gamepay tags of other actors](/assets/images/abilities02_sunscripe_to_gameplay_tag_changes.png)

***

## Lyra Gameplay Abilities Components and Template
*	Add Gameplay Cues, Gameplay Effects and Gameplay Costs to an Ability
*	Create a better Blueprint Debug function
*	Dance to death: Apply health costs for dancing

### Outcome
A more complete template for our Gameplay Ability System

### Video - english - see link below for german
{% include youtube.html id="Xy8ac79mwes" %}

### Video Link german
*	[Tutorial de](https://youtu.be/9wQtZi9TMc4)

### Key Concepts
####	Gameplay Cues are connected via Gameplay Tags to Gameplay Abilities
####	Gameplay Cues Notifier point to Sound Waves, Niagara effects, Force Feedback effects or Camera Shakes
####	Gameplay Effects add costs to abilities - we use the Lyra health system to apply health costs while dancing
####	How to listen and react to Lyra gameplay tag changes in other actors. This is automatically multi-threaded, easily replicated and extremely low on resources - recommended as standard pattern to organize your in game communication

***

## Lyra Gameplay Abilities through the Environment
*	Bind in Lyra ShooterCore throughthe Visual Studio plugin file
*	Grant your character the GA_Interact from ShooterExplorer
*	Build a BP Actor derived from Lyra World Collectable
*	Use a BP Interface to launch an external URL while interacting

### Outcome
Understanding the usage of the GA_Interact and how to understand Gameplay Ability interactions as properties of the environment, not the character

### Video - english - see link below for german
{% include youtube.html id="vPkahUXpTK8" %}

### Video Link german
*	[Tutorial de](https://youtu.be/RoAFZHc9lzI)

### Key Concepts
*	GA_Interact scans for Lyra World Collectible
*	When found, an Gameplay Ability is granted to scanning actor and can be executed on keypress
*	Use BP Interfaces whenever possible to avoid the resource costs of storing full BPs in memory on the server

***

## Effects, Cues and Cooldowns
*	Build a teleporter that has a cooldown
*	Steer the cooldown widgets through game messages
*	Build a Gameplay Ability for teleporting
*	Think about client or server based actions

### Outcome
An understanding how to use game messsages to steer widget behaviour and how to use gameplay tags to trigger effects and cues

### Video - english - see link below for german
{% include youtube.html id="W2LNrvK4Yis" %}

### Video Link german
*	[Tutorial de](https://youtu.be/ysFsjkEPnFE)

### Key Concepts
*	Unreal game messaging system - publisher and subscriber patterns explored
*	Understanding the role of  Gameplay tags to trigger events 
*	Sending gameplay events to actors





https://youtu.be/8nVXALXJ24o