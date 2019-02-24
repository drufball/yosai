---
layout: page
title: Compendium
permalink: /compendium/
---

The world of Yosai has three main eras where stories are set. Below are all of the stories I've written, ordered chronologically.

# Primitive Era
The 5 races struggle to establish themselves. The Grand Tournament doesn't yet exist. The biggest communities are villages of 100-300 people, with very little communication between them.

{% for post in site.posts %}
  {% if post.era == "primitive" %}
  - [{{post.title}}]({{ post.url | relative_url }})
  {% endif %}
{% endfor %}


# The Grand Tournament Era
The Grand Tournament has fuelled an expansion in the civilizations of the 5 races. New towns and cities are established every 50 years when a new Champion is chosen. Communities are generally a few thousand people, with a few larger cities of 20,000. Communication exists but it's slow and error-prone.

{% for post in site.posts %}
  {% if post.era == "tournament" %}
  - [{{post.title}}]({{ post.url | relative_url }})
  {% endif %}
{% endfor %}

# Megacity Era
All of Yosai is covered in a single, sprawling metropolis. Advanced, magic-powered technologies exist. The gods are a more distant force.

{% for post in site.posts %}
  {% if post.era == "megacity" %}
  - [{{post.title}}]({{ post.url | relative_url }})
  {% endif %}
{% endfor %}