---
name: Cygames
subtitle: Project Awakening
external_url: 'https://projectawakening.com/en/'
image_path: /uploads/cygames-project-awakening-thumb.png
---

2017 to Present

Working as a Technical Artist on Project Awakening at Cygames in Shibuya, Tokyo.

&nbsp;

## Tool Development

##### StudioLibrary

Created a customized version of [StudioLibrary](https://www.studiolibrary.com/){: target="_blank"} for the character animators.

The artists had been using an internally created pose tool but wanted to switch to StudioLibrary.&nbsp; I created an importer and converter tool to change all the old poses to StudioLibrary poses. This let the artists seamlessly change tools and continue their work without interruption.

Support was added for Perforce to allow the artists to checkout and submit their poses to the repo directly from Maya. Perforce icons were added to all pose thumbnail previews to let artists know the current status of the files.

and creating poses from characters at locations other than the origin (Relative transform and rotation)

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