---
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: assets/images/journal.jpg
intro: 
  - excerpt: ''
excerpt: "Bacon ipsum dolor sit amet salami ham hock ham, hamburger corned beef short ribs kielbasa biltong t-bone drumstick tri-tip tail sirloin pork chop."
---

{% include feature_row id="intro" type="center" %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in  site.posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>