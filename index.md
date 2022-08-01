---
layout: default
title: Open Sourcerer
---
# <img src="assets/images/wizard-64x64.png" alt="Wizard with a hoodie" width="64" height="64"> Open Sourcerer

This is a work in progress. Stay tuned.

{% if jekyll.environment != "production" %}
## Blog Posts
<ul>
  {% for post in site.posts %}
    <li>
      <h2>{{ post.date | date_to_string }} <a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

## Highlighted

- [Martin Fowler](https://martinfowler.com){:target="_blank"}

## Authors

{% for author in site.staff %}
### <a href="{{site.baseurl}}{{ author.url }}">{{ author.name }}</a>

***{{ author.position }}***

{{ author.content | markdownify }}

{% endfor %}

{% endif %}