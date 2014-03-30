---
title: Home
layout: default
---

{% for post in site.posts %}

<div class='article'>
  <div class='stack3of5'>
    <h2 class='stackContent'>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
  </div>

  <div class='stack2of5'>
    <p class='stackContent date'>{{ post.date | date_to_string }}</p>
  </div>

  <div class='stackContent'>
    {{ post.content }}
  </div>

</div>

{% endfor %}
