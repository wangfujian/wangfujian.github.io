---
permalink: /publications/
title: "Publications"
excerpt: ""
author_profile: true
---

## Publications

{% assign pubs_by_year = site.data.publications %}
{% if pubs_by_year and pubs_by_year.size > 0 %}
{% for block in pubs_by_year %}
### {{ block.year }}

{% if block.items and block.items.size > 0 %}
{% for p in block.items %}
- **{{ p.title }}**  
  {{ p.authors }}  
  _{{ p.venue }}_  
  {% if p.links %}
  {% assign l = p.links %}
  {% if l.pdf %}[PDF]({{ l.pdf }}){% endif %}
  {% if l.doi %}{% if l.pdf %} · {% endif %}[DOI]({{ l.doi }}){% endif %}
  {% if l.arxiv %}{% if l.pdf or l.doi %} · {% endif %}[arXiv]({{ l.arxiv }}){% endif %}
  {% if l.code %}{% if l.pdf or l.doi or l.arxiv %} · {% endif %}[Code]({{ l.code }}){% endif %}
  {% if l.project %}{% if l.pdf or l.doi or l.arxiv or l.code %} · {% endif %}[Project]({{ l.project }}){% endif %}
  {% endif %}
{% endfor %}
{% else %}
_该年份暂无论文条目。_
{% endif %}

{% endfor %}
{% else %}
_暂无论文数据。请编辑 `_data/publications.yml` 添加条目。_
{% endif %}
