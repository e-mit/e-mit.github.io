---
title: GitHub
---

{% for repo in site.github.public_repositories %}
  [{{ repo.name }}]({{ repo.html_url }})  
  {{ repo.description }}  
  {%- for topic in repo.topics -%}
  <div class="topic-style">
  {{ topic }}
  </div>
  {%- endfor -%}
{% endfor %}
