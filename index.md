---
layout: index
title: 

---

{% include JB/setup %}


<ol class="index-list">
  {% for post in site.posts %}
  <li><a href="{{ post.url }}">{{ post.title }}</a>  <span class="t-meta">{{ post.date | date: "%Y-%m-%d" }} </span>{% if post.tagline %}<span class="t-slug"><br /><small>{{post.tagline}}</small></span>{% endif %}<hr></li>

    {% endfor %}
</ol>

