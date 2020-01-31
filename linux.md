---
layout: default
permalink: /linux
tags:
  - linux
  - chromeos
  - howto
  - vm
  - termux
  - commands
  - commandline
  - terminal
---

# Linux on Chrome OS

During the months of April and May of 2019, I recorded a four-part series of Pixel Power Podcast episodes where I discuss the install and use of Linux on Chrome OS via Google's Crostini virtual machine (VM) system.

The shows received a great response and this page consolidates all four original episode's audio, each episode's comprehensive show notes, and additional bonus information and resources that were not included in the episodes or were covered with little depth.

Earlier in April of 2019, I also recorded an episode describing how to use the Linux terminal Android app, [Termux](https://termux.com), on the Pixel Phone. This page also collects that episode and the resources mentioned.

I plan to keep this page updated and include new resources as they become available. It is my hope this page becomes a useful resource for those users new to Crostini, Termux, and Linux on Chrome OS.

## Linux on Chrome OS Episodes

### Episode Audio

- [0021: Part 1 - Installation and virtual machine review](/021) [2019-04-22]
- [0022: Part 2 - Linux applications installations](/0022) [2019-04-29]
- [0024: Part 3 - File management and hardware devices](/0024) [2019-05-19]
- [0025: Part 4 - Linux terminal commands](/0025) [2019-05-26]

### Episode Show Notes

- [0021: Part 1 - Installation and virtual machine review](https://docs.google.com/document/d/1AHhXEgUDgTeoHnSHq0n46R6FUXaJZVPyIMKWQPg-atI/edit?usp=sharing) [2019-04-22]
- [0022: Part 2 - Linux applications installations](https://docs.google.com/document/d/1kPbzHYavLEZoJyspYjncVw0oF9QjJn-4I00nacZZ5aU/edit?usp=sharing) [2019-04-29]
- [0024: Part 3 - File management and hardware devices](https://docs.google.com/document/d/1Meghu4O_XsYgy_Q2bg5J4l29yAGAnhapnO4qDGSHK7Y/edit?usp=sharing) [2019-05-19]
- [0025: Part 4 - Linux terminal commands](https://docs.google.com/document/d/1_6VOA8tSHkb9wu7xyomtnLp27-WdDPNMZf7T6MXlpy0/edit?usp=sharing) [2019-05-26]

If you enjoyed these episodes or learned something new, consider supporting the podcast. Whether a [one time tip](https://www.paypal.me/stevencombs) or [a monthly subscription](https://anchor.fm/pixelpowerpodcast/support) of your choosing, your support will allow me continue to bring you future shows and the comprehensive show notes you have come to know and love.

![Episode Album Art](/images/design/linux-on-chromeos.png)

<hr>

## Crostini Resources

- [Reddit Crostini Subreddit](https://www.reddit.com/r/Crostini/) - The place to go online to ask questions, join the discussion, and read the latest updates
- [Reddit Crostini Wiki](https://old.reddit.com/r/Crostini/wiki/index) - The best online resource for everything Crostini
- [Running Custom Containers on Chrome OS](https://chromium.googlesource.com/chromiumos/docs/+/master/containers_and_vms.md) - Google's source for using Crostini
- [Linux on Chromebooks 2019 Google I/O Presentation](https://www.youtube.com/watch?v=pRlh8LX4kQI) - Watch and learn what's new with Crostini

<hr>

## Termux Resources

- Pixel Power Podcast Termux Episode: [0026: Termux on Pixel Phone](/0026) [2019-06-09]
- [Termux on the Google Play Store](https://play.google.com/store/apps/details?id=com.termux&hl=en_US) - Grab a copy and it works on both Pixel phone and Pixelbook
- [Termux Homepage](https://termux.com/) - Home of the Android terminal emulator
- [Termux Wiki](https://wiki.termux.com/wiki/Main_Page) - Everything you need to know about using Termux on your Android phone
- [Termux SubReddit](https://www.reddit.com/r/termux/) - Community designed to help new and advanced users alike
- [Termux Facebook Page](https://www.facebook.com/termux/) - Official Facebook page for the app with tips, news, and assistance

<hr>

## Additional Reading

If you really want to learn Linux commands, I highly recommend the book below:

- The Linux Command Line: A Complete Introduction
- William E. Shots, Jr.
- Paperback: 504 pages
- Publisher: No Starch Press; 2 edition (March 7, 2019)
- It’s an awesome read and wonderful resource to have on your desk.

[Get a copy on Amazon for around $20](https://amzn.to/39zpSMm).

[![The Linux Command Line](https://images-na.ssl-images-amazon.com/images/I/51-T4ZwKduL._SX376_BO1,204,203,200_.jpg)](https://amzn.to/39zpSMm)

<hr>

## Error Resolutions

This area shares tips and trick to resolve errors you may encounter with the Crostini VM.

### Expired Key Signatures

In January of 2020, Chrome OS 80 (beta) came to our Pixelbooks and Slates with expired signatures keys for the Crostini repositories that contain Crostini tools and utilities. This error bewildered many when they saw the following error message when issuing the `sudo apt update` command and the following appeared:

```
W: GPG error: https://storage.googleapis.com/cros-packages/81 buster Release: The following signatures couldn’t be verified because the public key is not available: NO_PUBKEY 78BD65473CB3BD13
E: The repository ‘https://storage.googleapis.com/cros-packages/81 buster Release’ is not signed.
N: Updating from such a repository can’t be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
```

While you can wait for Google to update the signature keys, and all other software will receive updates, the command below will correct the error:

```
sudo apt-key adv --refresh-keys --keyserver keyserver.ubuntu.com
```

<hr>

## Crowd-Sourced Linux on Pixelbook App Compatibility List

Check out my open for comments and additions [Linux application compatibility Google Sheet](https://docs.google.com/spreadsheets/d/1Roo_GXUewJamb6_OUVbdYW2w5o9XJLXYW392s8TAA-Y/edit?usp=sharing). On this page you can view the applications that work with Crostini as well as; how to install the applications, which density setting optimizes the experience, and useful notes. Be sure to add your own information by leaving a comment. You can view a small window into the document below:

<p><iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vR-0z0oZFgd1DYnDW4yCOy3hzY-OuFCi1I9wcXGtm3us9IJqkwyZwAQgXtAk33RzoQMo4yH88IydVkj/pubhtml?widget=true&amp;headers=false" width="500px" height="700px" scrolling="yes"></iframe></p>

<hr>

## Feeback

Use the following methods to share feedack on this episode:

* Send an email to <steven@pixelpowerpodcast.com>
* Leave a voice message by clicking [here](https://anchor.fm/pixelpowerpodcast/message)
* Join the conversation on [Reddit](https://www.reddit.com/r/pixelpowerpodcast/)
* Tweet using [#pixelpowerpodcast](https://twitter.com/search?q=%23pixelpowerpodcast&src=typed_query)

<div id="amzn-assoc-ad-b81e3a4c-a2a4-4d9a-a47b-7d707c42cb86"></div><script async src="//z-na.amazon-adsystem.com/widgets/onejs?MarketPlace=US&adInstanceId=b81e3a4c-a2a4-4d9a-a47b-7d707c42cb86"></script>
