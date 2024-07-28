---
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: "/assets/images/Journal.jpg"
excerpt: Take a byte of coding advice, throw in a bit of a humorous anecdote and mix with a heap of unsolicited advice.

---


{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in  site.posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>