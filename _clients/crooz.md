---
name: Crooz
subtitle: '2014 - 2017 : Final Fantasy Grand Masters'
external_url: 'https://crooz.co.jp/'
image_path: /images/clients/crooz/ffgm/Final-Fantasy-Grandmasters_thumb.jpg
---

## ![](/images/clients/crooz/crooz-logo-large.jpg){: width="1800" height="971"}

# CROOZ

## Employment Overview

From January 2014 up to the late summer of 2016, I worked at **[Crooz](https://crooz.co.jp/)** in **Roppongi, Tokyo** on various game projects.<br>&nbsp;

# Unity Mobile Game Project

## [Final Fantasy Grandmasters](https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters)

## [![](/images/clients/crooz/ffgm/Final-Fantasy-Grandmasters.jpg){: width="983" height="793"}](https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters)

### Overview

From the summer of 2014 to the summer of 2016,&nbsp; I worked as **Lead Technical Artist** on **Final Fantasy - Grandmasters**.

From the fall of 2016, the game project and it's staff were transferred to another game development company where I continued to provide maintence and support on the project until the late summer of 2017.

The mobile game was developed using Unity4 and later, Unity 5.

### Graphics Development

#### Material Animation

I developed critical core technology for the game's magic effect system. It allowed the artists to create all the effects in Maya using animation of material properties like Color, Alpha, UV Translation, UV Rotation, UV Scaling and UV Offsets.

The core technology consisted of:

* A custom Maya FBX exporter
* A custom Unity FBX importer (Asset Post Processor)
* A Custom Unity script and shader

I created a custom Maya FBX exporter that handled exporting all the material animation curve data which was marked as "Custom Unity Data".

I also created a custom importer for Unity that handled importing all of the material animation data from the custom FBX and automatically created Unity animation clips and an animation controller from it.

Finally, a custom script and shader that I also developed was attached to the magic effect's Unity prefab to make it all work.

![Maya was used to create all the magic effects in FFGM](/images/clients/crooz/unite-2016-tokyo-2/ffgm_maya_effect_produciton.png "FFGM Magic Effect Production"){: width="640" height="359"}

#### Character Shaders

I developed various shaders for the game's characters including a skin tone shader. It blended 2 colors for surface and subsurface coloring. A texture mask was used to shade only the skin areas.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_shader_chara_skin.jpg){: width="1944" height="1296"}

#### Crystal Shader

I worked together with the Art Director to create a shiny crystal effect for a blue crystal in the game. It used a variant of the surface / subsurface coloring used in the character shaders.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_shader_crystal.jpg){: width="1944" height="1296"}

#### Post Effects

During my time on the project I created post effects optimized for mobile which included : Outline glow with bloom, specular and fresnel lighting effects.

&nbsp;

### Tools Development

#### Importers and Exporters for Material Animation

* Created a custom **Maya FBX exporter** for exporting material animation properties to Unity. The material animation properties included: Color, Alpha, UV Translation, UV Rotation, UV Scaling and UV Offsets.
* Created a custom **Unity FBX importer** for importing material animation data from Maya which also automatically created the Unity animation resources like : Animation Clips and an Animation Controller with the Animation States already setup.

&nbsp;

#### Productivity Tools for rapid creation of Unity assets

##### Prefab Creator Tool

I created a tool which allowed artists to easily create prefabs from FBX model assets in Unity. The artists could specify the prefab's name, file path and material shader. The tool was opened by right clicking on the FBX asset.

![](/images/clients/crooz/unite-2016-tokyo-2/Unity_Prefab_Creaton_Tool.png){: width="1104" height="190"}

##### Animation Controller Creator Tool

I also created a tool which allowed the artists to quickly create and setup Unity Animation Controllers from an animated FBX resource. The tool supported rapid creation and editing of Animation Layers, Animation States and Animation Parameters. The tool was opened by right clicking on an FBX animation asset in Unity.

![](/images/clients/crooz/unite-2016-tokyo-2/Unity_Animation_Controller_Creator_Tool.png){: width="855" height="419"}

##### &nbsp;

#### Automated Batching Tool for the mass, rapid creation of Unity prefabs

Building upon the previous tools mentioned above, I created a comprehensive all in one Unity prefab batch creation tool. Artists could drag and drop FBX assets from Unity onto the tool's asset list panel. It allowed the artists to create hundreds of prefabs at once. The settings for the prefabs could be applied to single, multiple, or all prefabs in the asset list.

The tool could also be used to mass update existing prefabs. A prefab's reference FBX model and animations would be automatically updated to the latest version. Any custom scripts attached to the prefab at the time of update would also be preserved.

\*\*Although not shown in this version, a preview pane was added to the right hand side of the batching tool. This allowed artists to quickly preview models with shaders and post effects before creating the prefab.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_prefab_creator_batch_tool_2.jpg){: width="1735" height="981"}

&nbsp;

#### Productivity Tools for quick previewing of Unity Model Animation

##### Animation Playback in Unity Editor

At this time to preview animations in Unity, you had to press the triangle "Play Button" and go into Playmode. This was actually a very lengthy process. The more assets we added to the game, the more time it took to get into Playmode.

To save time, I created a way to playback animations from Animation Controllers WITHOUT entering Unity's Playmode.

The Controller's Animation Layers and Animation States were selectable and each animation could be easily previewed.

The tool also featured standard media controls, scrubbing, time playback info and an animation loop option.

![](/images/clients/crooz/unite-2016-tokyo-2/Unity_Animator_Controller_Playback_Tool.png){: width="647" height="76"}

#### &nbsp;

#### Look Dev Tools for quick previewing of Unity Models

##### Magic Effect Previewer

Magic effect animation preview support included playback of material animation.&nbsp;

##### Character Previewer

Character model preview support included ability to change character type, gender, equipment and weapons. Playback of animation was also supported.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_chara_viewer_tool_2.jpg){: width="1654" height="952"}

##### Enemy Previewer

Enemy animation preview support included playback of attacks and attack effects.

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_enemy_viewer_tool_2.jpg){: width="1645" height="922"}

##### Map Previewer

Map model preview support included ability to change map type.

\*\*Although not shown in this version, a battle simulation mode allowed artists to preview the maps with characters and enemies at a battle location engaged in a mock battle situation.

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

Some of my time at Crooz was spent working on creating the GUI for various game screens using[NGUI](https://www.tasharen.com/?page_id=140), the most popular Unity UI system at the time.

### Gameplay Tuning

I also helped out testing and tuning the car racing gameplay. Various aspects of the race were checked (Collision issues, car path of CPU racer, fairness, bugs).