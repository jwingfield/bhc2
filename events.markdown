---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Bradford Heritage Connections Events
---

# Upcoming Events

<ul>
    {% for Event in site.data.bhc-events %}
    <li>
        {{Event}}
        {{Date}} {{Time}}
        {{details}}
   </li>
    {% endfor %}
</ul>

