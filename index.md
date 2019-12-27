---
layout: default
---

# Welcome to the home of the new Pixel Power Podcast

I will soon migrate the old site to this new GitHub hosted pages site. This will allow more interactivity as I can then incoporate a forum. This new site will also allow me to receive higher search results and make it easier to maintain and manage show notes and content. Come back in 2020 to see the upgrade.

<h1>Search Episodes</h1>
Looking for a specific show or contents in the awesome show notes? Use the Google Search feature below:

<form method="get" action="http://www.google.com/search" target="_blank">
<input type="hidden" name="sitesearch" value="stevencombs.com" />
<input type="text" name="q" size="60" maxlength="255" placeholder="Enter search string..." />
</form>
<br>

<h1>Latest Posts</h1>
{% for post in site.posts limit:10 %}
<li style='list-style-type: none;'>
{{ post.date | date: "%B %d, %Y" }}<br>
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
{{ post.content |truncatehtml | truncatewords: 40 }}
{% endfor %}
