---
layout: default
---

# Welcome to the home of the new Pixel Power Podcast

I will soon migrage the old site to this new GitHub hosted pages site. This will allow more interactivity as I can then incoporate a forum. This new site will also allow me to receive higher search results and make it easier to maintain and manage show notes and content. Come back in 2020 to see the upgrade.

## Latest Posts
{% for post in site.posts limit:15 %}
	<li style='list-style-type: none;'>
	<div><a href="{{ post.url }}">{{ post.title }}</a> – {{ post.date | date: "%B %d, %Y" }}</div>
	<div>{{ post.content |truncatehtml | truncatewords: 40 }}</div>
	</li>
	{% endfor %}