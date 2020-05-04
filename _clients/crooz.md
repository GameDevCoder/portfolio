---
name: Crooz
subtitle: 'Final Fantasy - Grandmasters, ACR Drift <br/> 2014 / 1 ~ 2017 / 7'
external_url: 'https://crooz.co.jp/'
image_path: /images/clients/crooz/ffgm/Final-Fantasy-Grandmasters_thumb.jpg
---

## ![](/images/clients/crooz/crooz-logo-large.jpg){: width="1800" height="971"}

# CROOZ

## Employment Overview

From January 2014 up to October 2016, I worked at [Crooz](https://crooz.co.jp/) in Roppongi, Tokyo on various game projects. One of them was Final Fantasy Grandmasters.

From November 2016, the game project and the team were sold off to another company which underwent a name change and was rebranded as Mighty Games. I continued providing updates and maintenance on the project until July 2017.<br>&nbsp;

# Unity Mobile Game Project

## [Final Fantasy Grandmasters](https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters)

## [![](/images/clients/crooz/ffgm/Final-Fantasy-Grandmasters.jpg){: width="983" height="793"}](https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters)

### Overview

From June 2014 up to October 2016,&nbsp; I worked as **Lead Technical Artist** on **Final Fantasy - Grandmasters**.

The mobile game was developed using Unity4 and later, Unity 5.

The game and it's development were discussed in a presentation at &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; [Unite 2016 Tokyo](https://www.youtube.com/watch?v=h5bqn6BpX-I){: target="_blank"}.

### Graphics Development

#### Material Animation

I developed critical core technology for the game's magic effect system. It allowed the artists to create all the effects in Maya using animation of material properties like Color, Alpha, UV Translation, UV Rotation, UV Scaling and UV Offsets.

The core technology consisted of:

* A custom Maya FBX exporter
* A custom Unity FBX importer (Asset Post Processor)
* A Custom Unity script and shader for Material Animation

I created a custom Maya FBX exporter that handled exporting all the material animation curve data which was marked as "Custom Unity Data".

I also created a custom importer for Unity that handled importing all of the material animation data from the custom FBX.

The importer also automatically created the Unity Animation Clips and Animation Controller, all set up and ready to use.

Finally, a custom script and shader that I also developed was attached to the imported magic effect's Unity GameObject to make it all work.

&lt;a screenshot showing that the magic effects were made in Maya&gt;

![Maya was used to create all the magic effects in FFGM](/images/clients/crooz/unite-2016-tokyo-2/ffgm_maya_effect_produciton.png "FFGM Magic Effect Production"){: width="640" height="359"}

#### Character Shaders

I developed various shaders for the game's characters including a skin tone shader. It blended 2 colors for surface and subsurface coloring. A texture mask was used to shade only the skin areas.

&lt;a screenshot showing the character skin shader with various color tones&gt;

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_shader_chara_skin.jpg){: width="1944" height="1296"}

#### Crystal Shader

I worked together with the Art Director to create a shiny crystal effect for a blue crystal in the game. It used a variant of the surface / subsurface coloring used in the character shaders.

&lt;a screen shot of the crystal shader and the textures used&gt;

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_shader_crystal.jpg){: width="1944" height="1296"}

#### Post Effects

During my time on the project I created post effects optimized for mobile which included : Outline glow with bloom as well as specular and fresnel lighting effects.

&nbsp;

### Tools Development

#### Importers and Exporters for Material Animation

* I created a custom **Maya FBX exporter** for exporting material animation properties to Unity. The material animation properties included: Color, Alpha, UV Translation, UV Rotation, UV Scaling and UV Offsets.
* I also created a custom **Unity FBX importer** for importing material animation data from Maya and also automatically created the Unity animation resources like : Animation Clips and an Animation Controller with the Animation States already setup.

&nbsp;

#### Productivity Tools for rapid creation of Unity assets

##### Prefab Creator Tool

I created a tool which allowed artists to easily create prefabs from FBX model assets in Unity. The artists could specify the prefab's name, file path and material shader. The tool was opened by right clicking on an FBX asset.

![](/images/clients/crooz/unite-2016-tokyo-2/Unity_Prefab_Creaton_Tool.png){: width="1104" height="190"}

##### Animation Controller Creator Tool

I also created a tool which allowed the artists to quickly create and setup Unity Animation Controllers from an animated FBX resource. The tool supported rapid creation and editing of Animation Layers, Animation States and Animation Parameters. The tool was opened by right clicking on an FBX animation asset in Unity.

![](/images/clients/crooz/unite-2016-tokyo-2/Unity_Animation_Controller_Creator_Tool.png){: width="855" height="419"}

##### &nbsp;

#### Automated Batching Tool for the mass, rapid creation of Unity prefabs

Building upon the previous tools mentioned above, I created a comprehensive all in one Unity prefab creation batch tool. Artists could drag and drop FBX assets from Unity onto the tool's asset list panel. It allowed the artists to create hundreds of prefabs at once.

The asset panel featured a checkbox based selection system so that artists could selectively create prefabs with the desired settings.

The tool could also be used to mass update existing Unity prefabs. If a newer version of the prefab's FBX asset was imported into Unity, the prefab's model and animations could be automatically updated, matching the latest FBX version. &nbsp; Any custom scripts attached to the prefab at the time of update would also be preserved.

\*\*Although not shown in this version, a preview pane was added to the right hand side of the batching tool. This allowed artists to quickly preview models with shaders and post effects before creating the prefab.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_prefab_creator_batch_tool_2.jpg){: width="1735" height="981"}

&nbsp;

#### Productivity Tools for quick previewing of Unity Model Animation

##### Animation Playback in Unity Editor

At this time to preview animations in Unity, you had to press the triangle "Play Button" and go into Playmode. This was actually a very lengthy process. The more FBX assets we added to the Unity project, the more time it took to get into Playmode.

To save time, I created a way to playback animations from Animation Controllers WITHOUT entering Unity's Playmode.

The Controller's Animation Layers and Animation States were selectable and each animation could be easily previewed.

The tool also featured standard media controls, scrubbing, time playback info and an animation loop option.

![](/images/clients/crooz/unite-2016-tokyo-2/Unity_Animator_Controller_Playback_Tool.png){: width="647" height="76"}

#### &nbsp;

#### Look Dev Tools for quick previewing of Unity Models

##### Magic Effect Previewer

Magic Effect preview support included playback of the effect's animation.&nbsp;

##### Character Previewer

Character Model preview support included ability to change character type, character parts, gender, armor and weapons. Each model could be selectively disabled from rendering. Playback of animation was also supported.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_chara_viewer_tool_2.jpg){: width="1654" height="952"}

##### Enemy Previewer

Enemy Model preview support included playback of animation layers and states as well as effects that were timed with the animations.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_enemy_viewer_tool_2.jpg){: width="1645" height="922"}

##### Map Previewer

Map Model preview support included the ability to change the map type.

\*\*Although not shown in this version, a battle simulation mode allowed artists to preview the maps with characters and enemies setup at a battle location engaged in a mock battle situation.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_map_viewer_tool_2.jpg){: width="1774" height="1014"}

##### &nbsp;

&nbsp;

## Unity Mobile Game Project

### ACR Drift

![](/images/clients/crooz/acr-drift/acr-drift-splash.jpg){: width="1900" height="1267"}

### Overview

From January 2014 up to May 2014,&nbsp; I worked as a **Technical Artist** on the mobile game title "ACR Drift".

The title was developed using Unity 4.

### Graphical User Interfaces

Some of my time at Crooz was spent working on creating the GUI for various game screens using [NGUI](https://www.tasharen.com/?page_id=140), the most popular UI system for Unity at the time.

### Gameplay Tuning

I also helped out with gameplay testing, especially the car racing. Various aspects of the race were checked (Collision issues, car path of CPU racer, fairness, bugs).