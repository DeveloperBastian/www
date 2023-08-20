---
layout: default
---
### Developer Bastian

<img src="{{site.url}}/www/assets/images/lyra_weapon.png" style="display: block; margin: auto;" class="medium-zoom-image" />

### [Lyra Weapon Usage 01 - Import and bind to animations](#lyra-weapon-usage-import-and-bin)

## Infographics
[Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)

## Lyra Weapon Usage - Import and Bind
*	Import a weapon mesh from Sektchfab
*	Create Lyra weapon definitions
*	Bind to animations

### Outcome
The ability to use every one or two hand (melee) weapon

### Video - english - see link below for german
{% include youtube.html id="rLe4Gxx3nhE" %}

### Video Link german
*	[Tutorial de](https://youtu.be/0WIOMtV1KjM)


### Thoughts
*	Weapon meshes are easy to import. Import Skeletal Mesh and Static Mesh for it
*	The default Lyra weapon definition features 5 necessary config files - can be templated out of the Pistol directory of ShooterCore
*	The animations needed for each weapon are tricky to get - dozend of different animations would ne necessary. Here we just use the unarmed animation BP and link the upper torso with custome defined animations
*	A challenge is to get the left hand IK right for two hand weapons: We track a custom socket  transfor each frame, but have to do this in the main thread. This is very suboptimal and needs to get fixed at one point - but this is not possible in BP

### Steps (referring to infographic letters)
*	orange S: 			Import the Static and Skeletal weapon meshes
*	orange L-O, Q, R:	Copy all config files and adjust
*	orange P:			Modify the ABP_Mannequin_Base and the custome ABPs of the plugin: ABP_BA_BASE as child of ABP_Mannequin_Base and ABP_WeaponName per weapon (to define upper body animation and left hand IK if it is a two hand weapon)

***
