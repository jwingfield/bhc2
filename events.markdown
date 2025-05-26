---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Events
---

# Upcoming Events

{% for event in site.data.bhc-events %}
  ## {{event.Date | date: "%a %-d %B %Y"}} at {{event.Time | date: "%H:%M" }}
  ## {{event.Event}}  
  {{event.Details}}
{% endfor %}
