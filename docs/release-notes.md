---
layout: default
title: Release notes
navigation_weight: 7
---
# Release notes
  
{% for post in site.posts %}
   {% if post.excerpt != post.content %}
## [{{ post.date | date: "%m/%d/%Y, %r (%Z)" }}]({{ site.baseurl }}{{ post.url }})
   {% else %}
## {{ post.date | date: "%m/%d/%Y, %r (%Z)" }}
   {% endif %}
   {{ post.excerpt }}
{% endfor %}
