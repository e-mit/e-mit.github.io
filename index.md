---
title: GitHub
---

{% for repo in site.github.public_repositories %}
  [{{ repo.name }}]({{ repo.html_url }}) \ 
  {{ repo.description }} \ 
  {{ repo | json }} \ 
  {% for topic in repo.topics %}
    {{ topic | json }} 
  {% endfor %}
{% endfor %}
