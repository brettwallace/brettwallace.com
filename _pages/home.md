---
layout: home
author_profile: true
---

<nav>
  <ul>
    {% assign pages_list = site.pages | where_exp: "p", "p.path contains '_pages/'" %}
    {% for page in pages_list %}
      {% if page.title %}
        <li><a href="{{ page.url }}">{{ page.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</nav>