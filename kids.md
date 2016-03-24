---
layout: post
title: Teaching Kids
---
{% for post in site.categories.kids %}

## [{{ post.title }} ]({{ site.github.url}}{{ post.url }})
{{ post.date | date_to_string }}
  {{ post.excerpt }}
[read more]({{ site.github.url }}{{ post.url }})
{% endfor %}
