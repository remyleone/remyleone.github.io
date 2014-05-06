---
title: Home
layout: default
---

Blog posts
==========

{% for post in site.posts %}

{{ post.date | date_to_string }} <a href="{{ post.url }}">{{ post.title }}</a> _{{ post.teaser }}_

{% endfor %}
