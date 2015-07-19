---
layout: page
title: Posts
permalink: /posts/
---

{% for post in site.posts %}
  [{{post.title}}]({{ post.url | prepend: site.baseurl }}) 
  {{post.excerpt}}
{% endfor %}