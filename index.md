---
layout: page
title: Drop City Caps
tagline: Supporting tagline
---
{% include JB/setup %}

<ul class="posts home">
  {% for post in site.posts %}
    <li><a href="{{ site.baseurl }}{{ post.url }}">     	{% if post.thumbnail %}
	<img src="{{ site.baseurl }}{{ post.thumbnail }}" />
	{% else %}
	<img src="{{ site.baseurl }}/assets/global/200px.png" />
    {% endif %}
    <h3>{{ post.title }}</h3>
    {{ post.date | date_to_string }}
    <h4>{{post.country}}</h4>
</a></li>
  {% endfor %}
</ul>


