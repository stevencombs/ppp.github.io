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

Over the Christmas break, I decided to move the podcast site from Google Sites to GitHub pages. It turned out to be a more involved than I anticipated. I decided to capture the overarching tasks of this process in a blog post. This is not a step-by-step on how to move a site from one platform to another, but simply the documentation of my tools, processes, and challenges.

![Working in Atom](/images/posts/2019-12-29-sites-to-github/atom-screenshot.png)

## Equipment and Applications
Before I document the website platform conversion process, below is a list of the devices and applications used. My workflow is scattered across multiple devices; which will likely surprise some readers.

### Lenovo (Intel i5)
The Lenovo is a handme down all-in-one unit. After I upgraded the hard drive to a solid-state drive this computer is an awesome Linux box with an [Ubuntu Mate](https://ubuntu-mate.org/) install.

  * [Atom](https://www.atom.io) - Open source editor. By itself Atom is an awesome tool, but when you add packages, you can customize Atom to become an amazing blogging tool.
  * [Chrome Browser](https://www.google.com/chrome/) - This is the Pixel Power Podcast, of course I use this browser and install it on all my devices to keep things synced.
  * [Google Photos](https://photos.google.com) - I do all my image editing within Google Photos. I don't really have a need to do more than this tool provides.
  * [G Suite](https://gsuite.google.com/) - Has all the tools I need to create show notes, artwork, logos, and any other visual media needed for the podcast
  * [Jekyll](https://jekyllrb.com/) - GitHub Pages uses the Jekyll platform to host web pages.

### Mac mini (Intel i3)
This is a brand new Mac mini and purchased for podcasting. I record, edit, and post the podcast from this computer.

  * [Atom](https://www.atom.io) - I use a [sync-settings](https://atom.io/packages/sync-settings) package to ensure all devices have the same packages and settings.
  * [Chrome Browser](https://www.google.com/chrome/)
  * [Google Photos](https://photos.google.com)
  * [G Suite](https://gsuite.google.com/) - Having all these tools and files in the cloud ensures I have access to everything, everywhere, on any device.
  * [Jekyll](https://jekyllrb.com/) - To preview changes on a local machine before you commit to the live server, install Jekyll on your Linux, Mac or PC (Crostini not supported at this time under Chrome OS)
  * [GitHub Desktop](https://desktop.github.com/) - I can configure Atom push changes to GitHub pages, but I really enjoy using this Mac desktop client and my only wish is that it were available on Linux.

### Pixelbook (Intel i5)
I wish I could use Chrome OS devices exclusively for everything I do. For 90% of my tasks, these devices work; however, video and audio creation is still a struggle; thus the Mac mini in my inventory. Maybe when Crostini gets out of beta and has better hardward support this will change.

  * [Crostini](https://chromium.googlesource.com/chromiumos/docs/+/master/containers_and_vms.md) (Linux Beta) - Atom (and for other Linux apps I may want to use later) requires this Linux Debian distribution.
  * [Atom](https://www.atom.io) - How cool is it that I can run Atom on all platforms?
  * [Chrome Browser](https://www.google.com/chrome/) - It's the only browser available on the Chrome OS, so it makes sense to use it on the Linux and Mac machines as well.
  * [Google Photos](https://photos.google.com)
  * [G Suite](https://gsuite.google.com/)
  * [Caret](https://thomaswilburn.net/caret/) - A native text editing application for Chrome OS. Not as robust as Atom but when I just need to edit files and blog posts, this is the app I fire up on my Pixelbook or Pixel Slate (see image below)

![Caret Text Editor](/images/posts/2019-12-29-sites-to-github/caret-screenshot.png)

## Steps and Commentary

1. Create a GitHub account. I already had one for my blog at <https://www.stevencombs.com>.
2. Create a [new repository](https://github.com/new).
3.


Manual process to convert individual episode pages which is why moving to Jekyll was a great idea. Markdown means this task would be easier in the future (hopefully I will not ever need to do this again!).

## Feeback

Use the following methods to share feedack on this post:

* Sending an email to [steven@pixelpowerpodcast.com](mailto:steven@pixelpowerpodcast.com)
* Leave a voice message by clicking [here](https://anchor.fm/pixelpowerpodcast/message)
* Join the conversation on [Reddit](https://www.reddit.com/r/pixelpowerpodcast/)
* Tweet using [#pixelpowerpodcast](https://twitter.com/search?q=%23pixelpowerpodcast&src=typed_query)
