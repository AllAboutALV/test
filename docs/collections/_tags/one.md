---
slug: tag_one
name: ONE
description: this is a demo tag to sse how tags might work
---
<body>
  <h3>tag</h3>
  <ul>
  {% assign pages = site.tags %}
  {% for doc in pages %}
  {% if doc.title != "Tags" %}
  <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
  {% endif %}
  {% endfor %}
  </ul>
  </body>
