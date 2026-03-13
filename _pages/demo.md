---
permalink: /demo/
title: "Demo"
excerpt: ""
author_profile: true
---

## Demo

{% assign demos = site.data.demos %}
{% if demos and demos.size > 0 %}
{% for d in demos %}
### {{ d.title }}

{% if d.date %}{{ d.date }}{% endif %}

{% if d.description %}
{{ d.description }}
{% endif %}

{% if d.video_url %}- Video: [{{ d.video_url }}]({{ d.video_url }}){% endif %}
{% if d.slides_url %}- Slides: [{{ d.slides_url }}]({{ d.slides_url }}){% endif %}
{% if d.code_url %}- Code: [{{ d.code_url }}]({{ d.code_url }}){% endif %}

{% endfor %}
{% else %}
_暂无 Demo 数据。请编辑 `_data/demos.yml` 添加条目。_
{% endif %}
