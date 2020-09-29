---
layout: post
title:  "The move from Google Sites to GitHub Pages"
date:   2019-12-29 08:00:00 -0500
author: "Steven B. Combs, Ph.D."
comments: true
category:
  - site-news
tags:
  - jekyll
  - atom
  - html
  - css
  - github
---

During the 2019 Christmas break, I moved the Pixel Power Podcast podcast site from Google Sites to GitHub Pages. The process was more involved than I anticipated. I decided journal the process as a blog post. This is not a step-by-step list of tasks necessary to move a site from one platform to another but simply the documentation of my tools, processes, and challenges.

![Working in Atom](/images/posts/2019-12-29-sites-to-github/atom-screenshot.png)

## Equipment and Applications
Before I document the website platform conversion process, below is a list of the devices and applications I used. My workflow is scattered across multiple devices; which will likely surprise some readers.

### Lenovo ThinkCentre (Intel i5)
The Lenovo is an all-in-one unit. After I upgraded the hard drive to a solid-state drive this computer is an awesome Linux box with an [Ubuntu Mate](https://ubuntu-mate.org/) install.

  * [Atom](https://www.atom.io) - Open source editor. By itself Atom is an awesome tool, but when you add packages, you can customize Atom to become an amazing blogging tool.
  * [Chrome Browser](https://www.google.com/chrome/) - This is the Pixel Power Podcast, of course I use this browser and install it on all my devices to keep things synced.
  * [Google Photos](https://photos.google.com) - I do all my image editing within Google Photos. I don't really have a need to do more than this tool provides.
  * [G Suite](https://gsuite.google.com/) - Has all the tools I need to create show notes, artwork, logos, and any other visual media needed for the podcast
  * [Jekyll](https://jekyllrb.com/) - GitHub Pages uses the Jekyll platform to host web pages.

### 2019 Mac mini (Intel i3)
This Mac mini was purchased for the podcast. I record, edit, and post the podcast from this computer.

  * [Atom](https://www.atom.io) - I use a [sync-settings](https://atom.io/packages/sync-settings) package to ensure all devices have the same packages and settings.
  * [Chrome Browser](https://www.google.com/chrome/)
  * [Google Photos](https://photos.google.com)
  * [G Suite](https://gsuite.google.com/) - With all of these tools and files in the cloud, I have access to everything, everywhere, on any device.
  * [Jekyll](https://jekyllrb.com/) - To preview changes on a local machine before you commit to GitHub pages, install Jekyll on your Linux, Mac or PC (Crostini not supported at this time under Chrome OS)
  * [GitHub Desktop](https://desktop.github.com/) - I can configure Atom push changes to GitHub pages, but I really enjoy using this Mac desktop client and my only wish is that it were available on Linux.

### Pixelbook (Intel i5)
I wish I could use a Chrome OS device exclusively for everything. For 90% of my tasks, these devices work; however, video and audio creation is still a struggle; thus the Mac mini in my inventory. Maybe when Crostini gets out of beta and has better hardware support this will change.

  * [Crostini](https://chromium.googlesource.com/chromiumos/docs/+/master/containers_and_vms.md) (Linux Beta) - Atom (and for other Linux apps I may want to use later) requires this Linux Debian distribution.
  * [Atom](https://www.atom.io) - How cool is it that I can run Atom on all platforms?
  * [Chrome Browser](https://www.google.com/chrome/) - It's the only browser available on the Chrome OS, so it makes sense to use it on the Linux and Mac machines as well.
  * [Google Photos](https://photos.google.com)
  * [G Suite](https://gsuite.google.com/)
  * [Caret](https://thomaswilburn.net/caret/) - A native text editing application for Chrome OS. Not as robust as Atom but when I just need to edit files and blog posts, this is the app I fire up on my Pixelbook or Pixel Slate (see image below)

![Caret Text Editor](/images/posts/2019-12-29-sites-to-github/caret-screenshot.png)

## Steps and Commentary
As mentioned early, the steps below are not detailed but just a rough outline of the process with notes I've captured for myself that might be helpful later or for other readers. Do not expect to follow these steps and create a GitHub pages site or migrate from another platform to GitHub pages; however, some of the information could be useful if you are curious or stuck.

### Setup the Site

1. Create a GitHub account. I already had one for my blog at <https://www.stevencombs.com>.
2. Create a [new repository](https://github.com/new).
3. Identify the repository as a GitHub page and make required settings.
4. Link website URL to GitHub pages.
5. Modify the `CNAME` in the `_config.yml` file.
6. Connect domain name to my registrar, I use [Hover](https://www.hover.com).

### Prepare Git and GitHub

Connecting a custom domain name to GitHub pages should be one of the last things you do. I did not follow my own advice because I knew it would take some time for the domain to propogate from the Google Sites to the GitHub pages. During that time I would begin moving content over. I was surprised that the process only took an hour or so.

1. While waiting for steps 4 and 6 above to sync on the "interwebs", identify a theme to use for the site. I chose the [minimal theme](https://github.com/orderedlist/minimal) for its ease of modification.
2. Pull the repository to a Google Drive folder (that syncs across the many devices I noted above) using GitHub desktop on the Mac.
3. Open Atom and add the folder from step 8 as a project folder.
4. Configure Atom to push, pull, and commit to GitHub repository using the instructions provided in the Atom GitHub tab.

### Configure Jekyll Site

Configure the Jekyll site using the steps below. There are many steps I do not list. I recommend you read [Getting Started with GitHub pages](https://guides.github.com/features/pages/) and consider the steps below bonus content.

1. Modify the `_layout` files and the `index.md` file.
2. Add additional `_config.yml` file. You can view [my file on GitHub](https://github.com/stevencombs/ppp.github.io/blob/master/_config.yml).
3. Modify the default CSS to match my color and branding. You can view my draft [Pixel Power Podcast style guide on Google Docs](https://docs.google.com/document/d/1nzEAKBPQP1CRGe2iVODfYNj4pKrPLHLEWGdM5Ui-X8w/edit?usp=sharing).
4. Embed two [Google Fonts](https://fonts.google.com) for use on the site. I had problems with this and will come back to it at a later time.
5. Create a directory structure for file and images. I could use a files manager application, but Atom has all the tools built-in and allows me to stay in a single app to manage, write, and post to the site. I chose to put all images in `images/posts/YYYY-MM-DD` folders and files. Using this structure will allow me to quickly search for images that match posts since they are all tied to the same date.

### Copy Content from Google Sites

Once the Jekyll site is configured, begin the very manual and very laborious task of moving content from Google Sites pages to Jekyll posts.

1. Create a `template.md` file in the `_drafts` folder. This file will be duplciated before each new post and used as a template to ensure consistency between all posts. I found myself modifying it regularly to add additional features or corrections to streamline my flow. [View my template on GitHub](https://raw.githubusercontent.com/stevencombs/ppp.github.io/master/_drafts/template.md).
2. Duplicate the `template.md` file in Atom (simply right-click on the file and choose the Duplicate option). Keep this file in the `_drafts` folder until is complete and has been read and edited at least twice.

It was a great chance to clean up some errors and correct consistency. Be sure and go back and look at previous episode pages for new content.

Added an RSS feed to the Jekyll site. Thanks to Joel Glovier for [these simple instructions](https://joelglovier.com/writing/rss-for-jekyll).

## Feeback

Use the following methods to share feedack on this post:

* Send an email to <steven@pixelpowerpodcast.com>
* Leave a voice message by clicking [here](https://anchor.fm/pixelpowerpodcast/message)
* Join the conversation on [Reddit](https://www.reddit.com/r/pixelpowerpodcast/)
* Tweet using [#pixelpowerpodcast](https://twitter.com/search?q=%23pixelpowerpodcast&src=typed_query)
