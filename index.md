---
layout: home
title: "WinBig"
---

# Welcome to WinBig 🎯

Welcome to **WinBig** — your place for simple and easy-to-understand
information about Big Draws.

## 📰 Latest Information

Explore our latest articles and guides.

{% for post in site.posts %}
<article>
  {% if post.image %}
  <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" style="width:100%; max-height:450px; object-fit:cover; border-radius:12px;">
  {% endif %}

  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>

  <p>{{ post.excerpt | strip_html | truncate: 200 }}</p>
</article>
{% endfor %}

## 🎯 Big Draw Guide

Learn how draws generally work, what to check before participating,
and where to find official information.

> Always check the official rules and applicable laws for the particular draw.
