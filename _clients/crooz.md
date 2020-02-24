---
name: Crooz
subtitle: '2014 - 2017 : Final Fantasy Grand Masters'
external_url: 'https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters'
image_path: /images/clients/crooz/ffgm/Final-Fantasy-Grandmasters_thumb.jpg
---

![](/images/clients/crooz/crooz-logo-large.jpg){: width="1800" height="971"}

2014 to 2017

## [![](/images/clients/crooz/ffgm/Final-Fantasy-Grandmasters.jpg){: width="983" height="793"}](https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters)

## [Final Fantasy Grandmasters](https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters)

### Overview

From the summer of 2014 up to the fall of 2016,

I worked as Lead Technical Artist on **Final Fantasy - Grandmasters** at [Crooz](https://crooz.co.jp/) in Roppongi, Tokyo.

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

![](/images/clients/crooz/unite-2016-tokyo-2/ffgm_prefab_creator_batch_tool_2.jpg){: width="1735" height="981"}

&nbsp;

#### Productivity Tools for quick, easy previewing of Unity Models and Animation

&nbsp;

* Created unity asset preview and batch management tool for:&nbsp;
* Rapid creation of new prefabs from FBX assets.&nbsp;
* Rapid creation of Animation Controllers from FBX assets.&nbsp;
* Updating unity prefabs when FBX model geometry or animations changed. Scripts attached to the prefabs were preserved.&nbsp;
* Setting shader parameters / custom asset parameters. - Previewing unity models (with post effects)&nbsp;
* Previewing animation playback from Animation Controllers &nbsp; (With support for selectable animation layers & states, playback possible WITHOUT entering Unity's play-mode)&nbsp;
* Magic effect animation preview support included playback of material animation.&nbsp;
* Character model preview support included ability to change equipment and weapons.&nbsp;
* Enemy animation preview support included playback of magic effects for attacks. Map model preview support included battle simulation

&nbsp;

&nbsp;

##### &nbsp;

&nbsp;

&nbsp;

&nbsp;

### [Unreal Engine](https://www.unrealengine.com/en-US/)

#### Materials And Shading

I helped with materials and shading development in Unreal Engine 4. Specifically, the improvement of character hair shading for the main character. I also helped with debugging and fixing materials on the Playstation 4.

&nbsp;

&nbsp;

![](/uploads/anubis-zone-of-the-enders-large.jpg){: width="616" height="353"}

## [Anubis Zone of the Enders M∀RS](https://www.konami.com/games/zoe_mars/as/en/)

(Developed by Konami in conjunction with Cygames)

### Localization

Some of my time at Cygames was spent working on localization efforts for the PS4 release of Anubis Zone of the Enders - M∀RS.

My tasks included proof reading and editing the games English text, reviewing in-game spoken English dialog and written English text displayed in the game's UI.

I also helped enter localized game text for the French, German, Italian and Spanish languages using an in-house localization editor tool.

&nbsp;

&nbsp;

![](/uploads/cygames-logo-technical.jpg){: width="600" height="336"}

## Internal Development

### Maya Log Aggregator

I Implemented a logging system for Maya that can collect logs from multiple running instances of Maya (2015, 2016, 2017) and aggregate them into a single comprehensive log file. I used the Python version of [ZMQ](https://zeromq.org) ([PyZMQ](https://zeromq.org/languages/python/)) recompiled for Maya to accomplish the task.

### Tool Logging Server

Created a python based logging server for receiving logging information from internal tools (Maya, Photoshop etc). The logs were collected for metrics to determine the usage rates and failure rates for our in-house tools. The metrics were visually displayed as various graphs and charts.

The server was initially put together with [Flask AppBuilder](https://flaskappbuilder.pythonanywhere.com/), [CherryPY](https://cherrypy.org/) (as the WSGI server), [JINJA2](https://palletsprojects.com/p/jinja/) templates, [SQL Alchemy](https://www.sqlalchemy.org/) and a [Postgres Database](https://www.postgresql.org/).

The tool logging server was later reimplemented with [Kibana](https://www.elastic.co/kibana) and [FluentD](https://www.fluentd.org/). I also included [Slack](https://slack.com/) integration via webhooks so that we could have logs with critical errors sent to our developer Slack channel.

&nbsp;

### Improvement of Development Operations

I conducted information research for improving quality of code and developer documentation. Some of the results include:

* Source Code Analysis Tools
  * [SonarLint](https://www.sonarlint.org/)
  * [SonarQube](https://www.sonarqube.org/)
* Coding Styles and Coding Style Tools
  * [Unibeautify](https://unibeautify.com/)
* Source Code Documentation Generation Tools
  * Javascript : [Sphinx-JS](https://github.com/mozilla/sphinx-js), [TypeDoc](https://typedoc.org/)
  * Python: [Sphinx](https://www.sphinx-doc.org/en/master/) , [PyCharm Doc Generation](https://www.jetbrains.com/help/pycharm/generating-reference-documentation.html)
  * C/C++: [Doxygen](https://www.doxygen.nl/)
* Source Code Documentation Integrations for Confluence
  * [Sphinx For Confluence](https://github.com/sphinx-contrib/confluencebuilder)
  * [Doxygen For Confluence](https://docs.appfusions.com/display/DOXYGEN/Home)

&nbsp;

### Research and Development

#### Graphics

&nbsp;Investigated implementing Ambient Occlusion rendering techniques for an unspecified Unity mobile title.

## &nbsp;