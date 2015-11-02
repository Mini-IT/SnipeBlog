---
layout: page
title: Welcome to Snipe Server Blog!
tagline: Supporting tagline
---
{% include JB/setup %}

{% for post in site.posts offset: 0 limit: 50 %}
<li>
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p><small><strong>{{ post.date | date: "%B %e, %Y" }}</strong> . {{ post.category }} </small></p>
{{ post.content }}
</li>
{% endfor %}
