---
title: GitHub
---

{%- for repo in site.github.public_repositories -%}
<p>
<a href="{{ repo.html_url }}">{{ repo.name }}</a>
<div class="description-style">{{ repo.description }}</div>
{%- for topic in repo.topics -%}
<div class="topic-style">{{ topic }}</div>
{%- endfor -%}
</p>
{%- endfor -%}
