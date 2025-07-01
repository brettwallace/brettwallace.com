---
layout: home
author_profile: true
---

<nav>
  <ul>
    {% for page in site.pages %}
      {% if page.path contains '_pages/' %}
        <li><a href="{{ page.url }}">{{ page.title | default: page.name }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</nav>