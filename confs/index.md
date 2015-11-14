---
layout: page
title: Conferences
---

{% for year in site.data.confs %}
{% assign conf = site.data.[year] %}

##{{ conf.info.year }} {{ conf.info.title }} 
 	
<img class="logo logo_in_list" src="/img/{{ conf.info.year }}/conf-logo.png">
 	
{{ conf.dest.long }}

[read more...](/confs/{{ conf.info.year }} "read more")

***

{% endfor %}
