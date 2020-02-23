---
name: Crooz
subtitle: Final Fantasy Grand Masters
external_url: 'https://finalfantasy.fandom.com/wiki/Final_Fantasy_Grandmasters'
image_path: /uploads/cygames-project-awakening-thumb.png
---

![](/images/clients/crooz/crooz-logo-large.jpg){: width="1800" height="971"}

2014 to 2016

Worked as Lead Technical Artist on **Final Fantasy - Grandmasters** at [Crooz](https://www.cygames.co.jp/en/) in Roppongi, Tokyo.

## ![](/images/clients/crooz/ffgm/FF-Grandmasters_wide.jpg){: width="600" height="337"}

## [Project Awakening](https://projectawakening.com/en/)

### Tool Development

#### [StudioLibrary](https://www.studiolibrary.com/){: target="_blank"}

StudioLibrary is a free tool for managing poses and animation in Autodesk Maya.

I created a customized version of StudioLibrary for the character animators.

The artists had been using an internally created pose tool but wanted to switch to StudioLibrary.&nbsp; I created an importer and converter tool to change all the old poses to StudioLibrary poses. This let the artists seamlessly change over to StudioLibrary and continue their work without interruption.

For file versioning support, I added [Perforce](https://www.perforce.com/) integration to StudioLibrary to allow the artists to update, checkout and submit their poses to the Perforce repo directly from Maya. Perforce icons were added to all pose thumbnail previews to let artists know the current status of the files.

Poses in StudioLibrary are created at the origin. But sometimes artists need to apply poses to characters in other locations. Support was added to make it possible to apply StudioLibrary poses to characters at world locations other than the origin.

##### &nbsp;

#### [Pyblish](https://pyblish.com/){: target="_blank"}

Pyblish is a free tool for checking and verifying that art assets comply with the established project guidelines for production. It can be used in various DCC software including Autodesk Maya.

The 3D art team had naming convention rules for the objects that make up the 3D game models. To help the artists check, validate and rapidly fix invalid model objects, I implemented a custom version of Pyblish.

Plugins were created for collecting and testing the various model object parts like :

* Main Model
* LOD Models
* Collision Models
* Rig Joints
* Materials and Textures

The objects were checked for proper naming and for proper object parenting (hierarchy check). Invalid objects showed up in red in the Pyblish validation result window.

In addition to the above plugins, I also added a name and hierarchy editing tool created with [Qt for Python](https://doc.qt.io/qtforpython/) (Pyside2) and [Yaml](https://yaml.org/).&nbsp; It included an object rule editor and object rule presets for each of the different model parts mentioned above. This editing tool could be opened directly from the Pyblish validation result window with a right click.

Any objects that had failed validation either due to incorrect naming or incorrect object parenting would be displayed in the tool.

Artists could use the tool to rapidly edit object names and hierarchy directly, or select an object rule preset and quickly apply a fix automatically.

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