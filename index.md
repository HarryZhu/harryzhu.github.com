---
layout: index
title: 

---

{% include JB/setup %}

<!--
  {% for post in site.posts %}
  <div class="post">
  <h1>
  <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a><br />
</h1>

  <span class="t-meta">{{ post.date | date_to_string }}</span>
  <hr class="t-border">
  <div class="content">
  {{ post.content }}
  </div>
  </div>
  <hr>
  <br><br><br><br><br><br><br><br><br><br><br><br>
  {% endfor %}
-->

  {% for post in site.posts %}
  <div class="post">
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <span class="t-meta">({{ post.date | date: "%Y-%m-%d" }}}</span>
  {{ post.content }}
  </div>
  <hr />
  {% endfor %}


