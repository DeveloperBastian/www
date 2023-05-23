---
layout: default
---
### Developer Bastian

![Developer Bastian](/assets/images/english.png)

### [Lyra Tagged Actors - How to change Skin](#how-to-change-a-skin-using-tagged-actors)
### [Workflow from Sketchfab to AccuRig to Unreal and how to reskin in game](#workflow-from-sketchfab-to-accurig-to-unreal-and-how-to-reskin-in-game)


# How to change a skin using Tagged Actors
*	Reskin our Lyra character from Manny to Quinn
*	Use a Paragon character as new skin 
*	Use a free asset from the marketplace - a detailed pirate from the great collection of [Maksim Bugrimov](https://www.unrealengine.com/marketplace/en-US/profile/Bugrimov+Maksim)
*	Use a MetaHuman as skin

## Outcome
An easy way to reskin your Lyra character within literally seconds

## Video - english - see link below for german
{% include youtube.html id="iBne_Sgu6N8" %}

### Video Link german
*	[Tutorial de](https://youtu.be/BY4Yc_7kjMU)

## Infographics
[Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)

## Thoughts
This is quite straightforward:
*	The only class you need is a BP based on the TaggedActor BP
*	There are two examples available from Lyra: B_Quinn and B_Manny. We reuse copys of these for our new characters - depending of we use male or female designs
*	The ABP retargeting process is easy now, using the ABP_UE4_Mannequin_Retarget via rightclick/"Retarget Animation Assets"/"Duplicate and Retarget Animation Assets"

## Steps (referring to infographic letters)
*	J-K: 	Open the "Duplicate and Retarget Animation Assets" window, select your OK Retargeter and your new skeletal mesh as target to create an new ABP
*	I: 		copy either B_Manny or B_Quinn as your new TaggedActor BP and set it to your new ABP and the imported Skeletal Maseh
*	E: 		Update your CharParts BP

***

# Workflow from Sketchfab to AccuRig to Unreal and how to reskin in game
*	Export FBX from a humanoid [SketchFab](https://sketchfab.com/3d-models/categories/characters-creatures?date=week&sort_by=-likeCount) skin
*	Always check the license of the work you use and attribute accordingly
*	Use [Realusion AccuRig](https://www.reallusion.com/auto-rig/accurig/) to rig your humanoids character
*	Import into Unreal and create a ABP and Tagged Actor
*	Create a BP Actor togrant a reskin ability
*	Create a reskin ability that changes Character Parts in game

## Video - english - see link below for german
{% include youtube.html id="t2mPy8xjS8M" %}

### Video Link german
*	[Tutorial de](https://youtu.be/YV0t8eqE47A)
