---
layout: default
---
### Developer Bastian

<img src="{{site.url}}/www/assets/images/animations_en.png" style="display: block; margin: auto;" class="medium-zoom-image" />

### [Animation from Mixamo](#mixamo-animations)

## Infographics
[Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)

## MixamoToUE - a fast way to get a Mixamo to UE5 retargeter
*	You can create your rig yourself for retargeting Mixamo animations - or just just the excellent [project](https://github.com/manosmiras/MixamoToUE) posted by manosmiras
*	Just select the XBot in Mixamo, export the animations and drop them into the MixamoToUE project, selecting the XBot skeleton
*	Then right click the animations, "Retarget Animation Assets"->"Duplicate and Retarget Animation Assets"
*	Select the XBot rig and retarget your animations - then migrate to your plugin folder
*	Go to your plugin, rightclick your animations and "Replace Skeleton" to your Mannequin 5 skeleton

### Python for automation
*	Enable both basic Python and the "Python Foundation Packages"
*	Define the path to find your scripts in
*	In this case, execute "AddAnimationNotifierTracks.py" to add notifier tracks to your animations

### Video - english - see link below for german
{% include youtube.html id="S9gZdC_4DOI" %}

### Video Link german
*	[Tutorial de](https://youtu.be/L2pJ7EZgras)

### Thoughts
*	Python is a powerful way to automate the Unreal Editor - definitely something we will dive into further
*	Cudos to Adobe(R) - the [license](https://helpx.adobe.com/creative-cloud/faq/mixamo-faq.html) for Mixamo animations is extremely open in usage and it is a great source for starting our animation journey
