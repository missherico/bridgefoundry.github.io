---
layout: post
title: Latest News
---
{% for post in site.posts %}
  {% unless post.draft %}

## [{{ post.title }} ]({{ post.url }})
{{ post.date | date_to_string }}
  {{ post.excerpt }}
[read more]({{ post.url }})

  {% endunless %}
{% endfor %}
