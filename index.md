---
title: GitHub
---

{%- for repo in site.github.public_repositories -%}
<p>
<a class="link" href="{{ repo.html_url }}">{{ repo.name }}</a>
<div class="description">{{ repo.description }}</div>
{%- for topic in repo.topics -%}
<div class="topic">{{ topic }}</div>
{%- endfor -%}
</p>
{%- endfor -%}
