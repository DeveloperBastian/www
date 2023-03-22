---
layout: default
---
### Developer Bastian

![Developer Bastian](/assets/images/english.png)

# Appearances: Targets of this tutorial
*	Reskin our Lyra character from Manny to Quinn
*	Use a Paragon character as new skin 
*	Use a free asset from the marketplace - a detailed pirate from the great collection of [Maksim Bugrimov](https://www.unrealengine.com/marketplace/en-US/profile/Bugrimov+Maksim)
*	Use a MetaHuman as skin

# Outcome
An easy way to reskin your Lyra character within literally seconds

# Video - english - see link below for german
{% include youtube.html id="iBne_Sgu6N8" %}

# Video Link german
*	[Tutorial de](https://youtu.be/BY4Yc_7kjMU)

# Infographics
[Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)

# Thoughts
This is quite straightforward:
*	The only class you need is a BP based on the TaggedActor BP
*	There are two examples available from Lyra: B_Quinn and B_Manny. We reuse copys of these for our new characters - depending of we use male or female designs
*	The ABP retargeting process is easy now, using the ABP_UE4_Mannequin_Retarget via rightclick/"Retarget Animation Assets"/"Duplicate and Retarget Animation Assets"

# Steps (referring to infographic letters)
*	J-K: 	Open the "Duplicate and Retarget Animation Assets" window, select your OK Retargeter and your new skeletal mesh as target to create an new ABP
*	I: 		copy either B_Manny or B_Quinn as your new TaggedActor BP and set it to your new ABP and the imported Skeletal Maseh
*	E: 		Update your CharParts BP

