---
layout: default
---
### Developer Bastian

![Developer Bastian](/assets/images/lyra.png)

# Targets of this tutorial

Installation of 
*	Visual Studio Community
*	Unreal Engine 5.x
*	Unreal Lyra

# Outcome

Ability to compile and start Lyra

# Video - english - see link below for german
{% include youtube.html id="frpAzIuGLDU" %}

# Video Link german
*	[Tutorial de](https://www.youtube.com/watch?v=rdFjPHC-rlg)

# Infographics
[Infographics](https://github.com/DeveloperBastian/Unreal-Lyra-Concepts/blob/main/infographics/Unreal%20Lyra.pdf)

# Thoughts

As promised, we will not use any C++ coding in our approach. Still, we need to have a working coding environment in place for several reasons
*	Lyra needs to recompile quite often and stumbles if there is not environment available
*	we want to debug workflows to understand how different parts of Lyra are connected
*	we **will** come to a point where defining a new functionality is easier in coding than Blueprints - but at that point we will have learned enough to know what we are doing (fingers crossed...)

# Steps
- Download & install Visual Studio Community
  - [Download link de](https://visualstudio.microsoft.com/de/vs/community/)
  - [Download link en](https://visualstudio.microsoft.com/en/vs/community/)
- Install Unreal Engine & Lyra
- Set up VS to be usable as debugger
  - Search the plugin "[Visual Studio Integration Tool](https://www.unrealengine.com/marketplace/en-US/product/visual-studio-integration-tool)" from the marketplace. Install into your engine and enable this plugin in your project
  - Go to your engine installation folder. Go to "/engine/extras/UnrealVS/". Select your VS version and install the Visual Studio extension from there
- Generate Visual Studion solution file from the Unreal project: "Menu/Tools/Create (later: Refresh) Visual Studio Project"
- Open your project in VS, right click on "LyraStarterGame" in your project explorer. First choose "Clean", afterwards choose "Build"

