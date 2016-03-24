---
layout: post
title: Teaching Kids
---
{% for post in site.categories.kids %}

## [{{ post.title }} ]({{ post.url }})
{{ post.date | date_to_string }}
  {{ post.excerpt }}
[read more]({{ post.url }})
{% endfor %}
