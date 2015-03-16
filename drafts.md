---
layout: post
title: Draft Blog Posts
---
{% for post in site.posts %}
  {% if post.draft %}

## [{{ post.title }} ]({{ post.url }})
{{ post.date | date_to_string }}
  {{ post.excerpt }}
[read more]({{ post.url }})

  {% endif %}
{% endfor %}
