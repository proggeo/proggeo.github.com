---
layout: page
title: Proggeo blog
tagline:
---
{% include JB/setup %}

## Posts

<ul class="posts">
  {% for post in site.posts %}
    <li>
      <h1><a href="{{ BASE_PATH }}{{ post.url }}">{{post.title}}</a></h1>
      <p>{{post.content | slice: 0,300}}...</p>
    </li>    
    <span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
  {% endfor %}
</ul>

