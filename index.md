---
layout: default
---

# Welcome to the Pixel Power Podcast

Each episode of the podcast and each blog post helps listeners and readers get the most out of your Google-powered devices and apps such as the Pixelbook, Pixel Slate, and Pixel phones.

Subscribe now at [Anchor.fm](https://anchor.fm/pixelpowerpodcast), [Pocket Casts](https://pca.st/RsNl), [Google Podcast](https://podcasts.google.com/?feed=aHR0cHM6Ly9hbmNob3IuZm0vcy83ZDgyNmI4L3BvZGNhc3QvcnNz), [iTunes](https://podcasts.apple.com/us/podcast/pixel-power-podcast/id1444466814), or searching for _Pixel Power Podcast_ in your favorite podcast client.

![OG Pixel Phone](/images/design/og-pixel.jpg)

<hr>

<h2>Search</h2>
Looking for a specific shows or content? Use the Google search feature below:

<p>
  <form method="get" action="http://www.google.com/search" target="_blank">
    <input type="hidden" name="sitesearch" value="pixelpowerpodcast.com" width="500px" />
    🔍 <input type="text" name="q" size="50" maxlength="255" placeholder="Enter search string… " />
  </form>
</p>

<hr>

<h2>Latest Episodes and Posts</h2>
{% for post in site.posts limit:100 %}
<li style='list-style-type: none;'>
{{ post.date | date: "%B %d, %Y" }}<br>
<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
{{ post.content |truncatehtml | truncatewords: 40 }}
{% endfor %}

<hr>
