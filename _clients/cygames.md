---
name: Cygames
subtitle: Project Awakening
external_url: 'https://www.cygames.co.jp/en/'
image_path: /uploads/cygames-project-awakening-thumb.png
---

![](/uploads/cyagames-logo-2.png){: width="800" height="414"}

2017 to Present

Currently working as a Technical Artist on **Project Awakening - Arise** at [Cygames](https://www.cygames.co.jp/en/) in Shibuya, Tokyo.

## [![](/uploads/cygames-project-awakening.png){: width="1200" height="630"}](https://projectawakening.com/en/)

## [Project Awakening](https://projectawakening.com/en/)

#### Tool Development

##### [StudioLibrary](https://www.studiolibrary.com/){: target="_blank"}

StudioLibrary is a free tool for managing poses and animation in Autodesk Maya.

I created a customized version of StudioLibrary for the character animators.

The artists had been using an internally created pose tool but wanted to switch to StudioLibrary.&nbsp; I created an importer and converter tool to change all the old poses to StudioLibrary poses. This let the artists seamlessly change over to StudioLibrary and continue their work without interruption.

For file versioning support, I added [Perforce](https://www.perforce.com/) integration to StudioLibrary to allow the artists to update, checkout and submit their poses to the Perforce repo directly from Maya. Perforce icons were added to all pose thumbnail previews to let artists know the current status of the files.

Poses in StudioLibrary are created at the origin. But sometimes artists need to apply poses to characters in other locations. Support was added to make it possible to apply StudioLibrary poses to characters at world locations other than the origin.

##### &nbsp;

##### [Pyblish](https://pyblish.com/){: target="_blank"}

Pyblish is a free tool for checking and verifying that art assets comply with the established project guidelines for production. It can be used in various DCC software including Autodesk Maya.

The 3D art team had naming convention rules for the objects that make up the 3D game models. To help the artists check, validate and rapidly fix invalid model objects, I implemented a custom version of Pyblish.

Plugins were created for collecting and testing the various model object parts like :

* Main Model,
* LOD Models,
* Collision Models,
* Rig Joints,
* Materials and Textures etc..

The objects were checked for proper naming and for proper object parenting (hierarchy check). Invalid objects showed up in red in the Pyblish validation result window.

In addition to the above plugins, I also added a name and hierarchy editing tool created with PyQt / Pyside2 and Yaml.&nbsp; It included an object rule editor and object rule presets for each of the different model parts mentioned above. This editing tool could be opened directly from the Pyblish validation result window with a right click.

Any objects that had failed validation either due to incorrect naming or incorrect object parenting would be displayed in the tool.

Artists could use the tool to rapidly edit object names and hierarchy directly, or select an object rule preset and quickly apply a fix automatically.

#### Unreal Engine

##### Materials And Shading

I helped with materials and shading development in Unreal Engine 4. Specifically, the improvement of character hair shading for the main character. I also helped with debugging and fixing materials on the Playstation 4.

&nbsp;

![](/uploads/anubis-zone-of-the-enders-large.jpg){: width="616" height="353"}

## Anubis Zone of the Enders M∀RS

(Developed by Konami in conjuction with Cygames)

### Localization

Some of my time at Cygames was spent working on localization efforts for the PS4 release of Anubis Zone of the Enders - M∀RS.

My tasks included proof reading and editing the games english text, reviewing in-game spoken English dialog and written English text displayed in the game's UI.

I also helped enter localized game text for the French, German, Italian and Spanish languages using an in-house localization editor tool.

&nbsp;

![](/uploads/cygames-logo-technical.jpg){: width="600" height="336"}

## Internal Development

#### Maya Log Aggregator

I Implemented a logging system for Maya that can collect logs from multiple running instances of Maya (2015, 2016, 2017)and aggregate them into a single comprehensive log file. I used PyZMQ (Python version of ZMQ), recompiled for Maya to accomplish the task.

#### Tool Logging Server

Created a python based logging server for receiving logging information from internal tools (Maya, Photoshop etc). The logs were collected for metrics to determine the usage rates and failure rates for our in-house tools. The metrics were visually displayed as various graphs and charts.

The server was initially put together with Flask AppBuilder (Python Server), CherryPY (as the WSGI server), REST API, JINJA2 templates,SQL Alchemy and a Postgres Database.

The tool logging server was later reimplemented with Kibana and FluentD. I also included Slack integration via webhooks so that we could have logs with critical errors sent to our developer Slack channel.

#### Improvement of Development Operations

Researched information for multiple areas of development including:

* Coding Styles and Automated Implementations
  * Unibeautify
* Source Code Documentation Tools
  * Javascript : [Sphinx-JS](https://github.com/mozilla/sphinx-js), [TypeDoc](https://typedoc.org/)
  * Python: [Sphinx](https://www.sphinx-doc.org/en/master/)
  * C/C++: [Doxygen](https://www.doxygen.nl/)

\+ Source Code Documentation Integrations (Sphinx For Confluence, Doxygen For Confluence)+ Source Code Analysis Tools (Lint Tools, SonarQube, Coverity)

#### Graphics Research and Development

&nbsp;- Ambient Occlusion Rendering Techniques For Mobile -Investigated rendering techniques for implementing Ambient Occlusion for an unspecified mobile title.

## &nbsp;

## Features

* Created a customized version of StudioLib
* Pre-styled components
* Configurable footer
* Optimised for editing in [CloudCannon](https://cloudcannon.com/)
* SEO tags
* Google Analytics
* [Donorbox](https://donorbox.org/)
* [MailChimp](https://mailchimp.com/)

## Setup

1. Add your site details in `_config.yml`.
2. Add your Google Analytics to `_config.yml`.
3. Get a workflow going to see your site's output (with [CloudCannon](https://app.cloudcannon.com/) or Jekyll locally).

## Develop

Cause was built with [Jekyll](https://jekyllrb.com/) version 3.3.1, but should support newer versions as well.

Install the dependencies with [Bundler](https://bundler.io/)\:

~~~bash
$ bundle install
~~~

Run `jekyll` commands through Bundler to ensure you're using the right versions:

~~~bash
$ bundle exec jekyll serve
~~~

## Editing

Cause is already optimised for updating pages, company details and footer elements in CloudCannon.

## SEO Tag

This site uses the [jekyll-seo-tag](https://github.com/jekyll/jekyll-seo-tag) plugin. You should at least set a title in front matter on each page. Have a look at the [project page](https://github.com/jekyll/jekyll-seo-tag) for more options.

## Google Analytics

[Google Analytics](https://www.google.com/analytics/) is a third party website analytics tool. To install:

1. Add your Google Analytics key to `_config.yml`
2. Run your site in production `JEKYLL_ENV=production`. This is the default in CloudCannon and GitHub Pages.

## Donorbox

[Donorbox](https://donorbox.org/) is a third party embeddable donation form for websites. To install:

1. Set up a campaign on Donorbox
2. Copy the embed code from the Dashboard screen
3. Paste it into `donation_embed` in `_config.yml`

## Mailchimp

[Mailchimp](https://mailchimp.com/) is a third party embeddable newsletter for websites. To install:

1. Set up a campaign on Mailchimp
2. Find the embed code for the sign up form
3. Copy the `<form>`'s action url
4. Paste it into `newsletter_action` in `_config.yml`

### Company details

* Reused around the site to save multiple editing locations.
* Set in the *Data* / *Company* section.