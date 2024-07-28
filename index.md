---
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: "/assets/images/Journal.jpg"
excerpt: - > 
Ingredients
1. A Byte of Coding advice
1. A Bit of humorous anecdote
1. A Heap of unsolicited advice

---


{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in  site.posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>