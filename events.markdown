---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: event
title: Events
---

# Upcoming Events

<ul>
    {% for Event in site.data.bhc-events %}
    <li>
        <ul>
          <li><em>{{Event}}</em></li>
          <li>{{Date}} {{Time}}</li>
          <li>>{{Details}}</li>
        </ul>
    </li>
    {% endfor %}
</ul>