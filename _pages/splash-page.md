---
title: "Splash Page"
layout: splash
permalink: /splash-page/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/journal.jpeg
  actions:
    - label: "Download"
      url: "#test-link"
intro: 
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
---

{% include feature_row id="intro" type="center" %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in  site.posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>