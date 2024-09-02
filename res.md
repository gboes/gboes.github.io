---
layout: default
title: Research
permalink: /res/
description: Published Research
---
# Publications and Research Presentations
<p>Click on lines to open details.</p>

## Software and Datasets
<ol reversed outside style="padding-left: 0em" type="1">
<li style="padding-left: 0.5em"> 
<details>
<summary><span style="color:#3c6cf6">e</span>dhiphy and <a href="https://edhiphy.org/?gb">edhiphy.org</a>
</summary>

<span style="color:#3c6cf6">e</span>dhiphy
offers enriched data for the history of philosophy.
I am developing the database and the web application <a href="https://edhiphy.org/?gb">edhiphy.org</a>. 
While the database is aimed at researchers, the web application can also be used heuristically as a tool for education.
</details>
</li>
</ol>
 
## Research Articles

<ol reversed outside style="padding-left: 0em">
{% for row in site.data.research_articles %}
<li style="padding-left: 0.5em"> 
<details>
<summary>{{ row.authors }}, {{row.year}}: {{row.title}}. <i>{{row.venue}} </i> (<a href="{{ row.url}}">{{ row.urltext }}</a>). {{ row.extra}}
</summary>

{{ row.abstract_pre}}
{% if row.abstract %}<p>Abstract: <br>
{{ row.abstract }} 
</p>
{% endif %}
{{ row.abstract_post}}
</details>
</li>
{% endfor %}
</ol>

## Critical Notices and Book Reviews
<ol reversed outside style="padding-left: 0em">
{% for row in site.data.book_reviews %}
<li style="padding-left: 1em"> 
<!-- <details> -->
<!-- <summary> -->
{{ row.authors }}, {{row.year}}: {{row.title}}, <i>{{row.venue}} </i>, <a href="{{ row.url}}">{{ row.urlstr }}</a>. {{ row.extra}}
<!-- </summary> -->
<!-- {{ row.abstract }} {{ row.abstract_extra }} -->
<!-- </details> -->
</li>
{% endfor %}
</ol>

## Presentations

<ol reversed outside style="padding-left: 0em">
{% for row in site.data.presentations %}
<li style="padding-left: 1em"> 
<details>
<summary>{{ row.date }}: {{row.title}}
</summary>

{{row.collaborators}}

{{ row.occasion }}
</details>
</li>
{% endfor %}
</ol>

