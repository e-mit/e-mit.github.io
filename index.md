---
title: GitHub
---

{% for repo in site.github.public_repositories %}
  {% assign repo_name = repo.full_name | split: "/" | last %}
  [{{ repo_name }}]({{ repo.html_url }})
  {{ repo.description }}
{% endfor %}
