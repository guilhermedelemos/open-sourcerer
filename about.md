---
layout: default
title: About
permalink: /about
---

# About 

This is a work in progress.

# Special Thanks

- [Sorcerer icons created by Freepik - Flaticon](https://www.flaticon.com/free-icons/sorcerer "sorcerer icons"){:target="_blank"}
- [Jekyll](https://jekyllrb.com/){:target="_blank"}
- [GitHub Pages](https://pages.github.com/){:target="_blank"}

{% if jekyll.environment != "production" %}
# Metadata

- Environment: {{ jekyll.environment }}
- Version: {{ site.version }}
- Title: {{ site.title }}
- E-mail: {{ site.email }}
- Description: {{ site.description }}
- Twitter: {{ site.twitter_username }}
- GitHub: {{ site.github_username }}
- URL: {{ site.url }}
- Base URL: {{ site.baseurl }}
- Time Zone: {{ site.timezone }}
- Encoding: {{ site.encoding }}
{% endif %}
