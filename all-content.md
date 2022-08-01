---
layout: default
title: Index of All content
permalink: /index-all-content
---

<h1>Posts</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    </li>
  {% endfor %}
</ul>

<h1>Categories</h1>
<ul>
{% for category in site.categories %}
  <li>{{ category[0] }}</li>
{% endfor %}
</ul>

<h1>Tags</h1>
<ul>
{% for tag in site.tags %}
  <li>{{ tag[0] }}</li>
{% endfor %}
</ul>

<h1>Topics</h1>
<ul>
  <li>Testing</li>
</ul>

<h1>Staff</h1>
<ul>
  {% for author in site.staff %}
    <li>
      <h2><a href="{{site.baseurl}}{{ author.url }}">{{ author.name }}</a></h2>
    </li>
  {% endfor %}
</ul>
