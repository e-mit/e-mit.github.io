---
title: GitHub
---

{% for repo in site.github.public_repositories %}
  [{{ repo.name }}]({{ repo.html_url }}) \
  {{ repo.description }} \
  {% for topic in repo.topics %}
    {{ topic }} 
  {% endfor %}
{% endfor %}
