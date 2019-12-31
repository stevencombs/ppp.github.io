---
layout: default
---

# Welcome to the home of the new Pixel Power Podcast

Each episode of the podcast and each blog post helps listeners and readers get the most out of your Google-powered devices and apps such as the Pixelbook, Pixel Slate, and Pixel phones.

![OG Pixel Phone](/images/design/og-pixel.jpg)

<h2>Search</h2>
Looking for a specific shows or content? Use the Google search feature below:

<form method="get" action="http://www.google.com/search" target="_blank">
<input type="hidden" name="sitesearch" value="pixelpowerpodcast.com" width="500px" />
🔍 <input type="text" name="q" size="50" maxlength="255" placeholder="Enter search string… " />
</form>
<br>

<h2>Latest Episodes and Posts</h2>
{% for post in site.posts limit:100 %}
<li style='list-style-type: none;'>
{{ post.date | date: "%B %d, %Y" }}<br>
<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
{{ post.content |truncatehtml | truncatewords: 40 }}
{% endfor %}
