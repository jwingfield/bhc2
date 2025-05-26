---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Events
---

# Upcoming Events

{% for Event in site.data.bhc-events %}
  <ul>
    <li><em>{{Event}}</em></li>
      <li>{{Date | date: "%a %-d %B %Y"}} {{Time | date: "%H:%M" }}</li>
    <li>>{{Details}}</li>
  </ul>

{% endfor %}
