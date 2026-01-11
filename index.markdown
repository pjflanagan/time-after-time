---
layout: page
title: Home
description: Watch Mods
image: ""
---

# Time After Time Watch Mods

This is a collection of customized watches (mostly Seiko's) that I've made. I work mostly with second hand parts sourced from all over. I am dedicated to transparency about the construction and components. If you're interested in owning a unique timepiece, please check out my available listings.

## Available Watches
<div>
  {% for post in site.posts %}
    {% if post.status == 'available' %}
    <div>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      - {{ post.description }}
    </div>
  {% endfor %}
</div>

## Past Watches
<div>
  {% for post in site.posts %}
    {% if post.status != 'available' %}
    <div>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      - {{ post.description }}
    </div>
  {% endfor %}
</div>
