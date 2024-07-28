---
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: "/assets/images/Journal.jpg"
excerpt: Take a Byte of coding advice, throw in a Bit of humorous anecdote and mix with heap of unsolicited advice.

---


{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in  site.posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>