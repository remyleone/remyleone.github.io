---
title: Home
layout: default
---

Recent Blog Posts
=================

{% for post in site.posts limit:7 %}

{{ post.date | date_to_string }} <a href="{{ post.url }}">{{ post.title }}</a> _{{ post.teaser }}_

{% endfor %}


Want more? Go checkout [Archives](/archives).
