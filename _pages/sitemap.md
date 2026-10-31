---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of pages on this site. An [XML version]({{ base_path }}/sitemap.xml) is also available.

<h2>Pages</h2>
<ul>
{% for post in site.pages %}
  {% unless post.path contains '404' or post.url == '/sitemap/' %}
  <li><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></li>
  {% endunless %}
{% endfor %}
</ul>
