---
layout: post
title: Teaching Kids Project
---
Encouraging kids to create computer software and hardware by providing
support and curricula and inspiring grown-ups to help them. This was a very active project in the early years of our organization and we are now seeking a leader who would like to facilitate the project. If you
are interested, [email us](mailto:hello@bridgefoundry.org).

Who this is for:

* Teachers who want to help kids to understand a part of the world they live in
* Parents who want to teach their kids or encourage their schools to teach programming
* People who write code and want to share their love of software development
* Kids who want to help teach other kids

Here are some stories of volunteer projects and other notes about teaching kids:

{% for post in site.categories.kids %}

### [{{ post.title }} ]({{ site.github.url}}{{ post.url }})
{{ post.date | date_to_string }}
  {{ post.excerpt }}
[read more]({{ site.github.url }}{{ post.url }})
{% endfor %}
