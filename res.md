---
layout: default
title: Research
permalink: /res/
description: Published Research
---
# Publications and Research Presentations
<p><i>Click on entries to expand details.</i></p>

## Software and Datasets
<ol reversed outside style="padding-left: 0em" type="1" start=1>
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

## Dissertation

<div style="padding-left: 0em" >
<div  style="padding-left: 0.5em"> 
<details>
<summary>Founding Science on the Lifeworld: Promises and Problems of a Phenomenological Philosophy of Natural Science. Dec. 2022, <i>King's College London</i>
</summary>

<p>
This dissertation investigates whether an account of scientific knowledge from the phenomenological tradition can offer a reconciliation of scientific and manifest images. I pursue this question in three parts: I) a study of the concept “lifeworld”, II) an examination of Husserl’s connection between truth and evidence, and III) an account of the metaphysics for scientific discovery.
</p>

<p>
Part I motivates the problem and offers a historical and systematic reconstruction of Husserl’s notion of the lifeworld. Sellars spelled out a conflict between the conceptual schemes of everyday life and scientific theory and argued for the priority of the scientific image. Phenomenology investigates the manifest image, but one might worry that this requires a rejection of the scientific image. I focus on Husserl to develop an account that instead reconciles manifest and scientific images. Although the lifeworld is often associated with a late turn in Husserl’s philosophy, it grows naturally out of the notion of horizonal intentionality and builds on Avenarius’ natural concept of the world. I resolve ambiguities in Husserl’s account by distinguishing concrete (egocentric) lifeworld, shared lifeworld, and the eidos “lifeworld”.
</p>

<p>
Understanding phenomenology as the systematic study of the lifeworld ex- plains why philosophers who reject Husserl’s official methodology are nevertheless recognizable as phenomenologists. Part II discusses Husserl’s notorious correlation between truth and possible evidence. From this arise three challenges for a reconciliation with the scientific image: first, from an epistemic restriction of truth, second from a semantic restriction through verificationism, and third, from logical problems with truth as knowability. Chapter 4 traces Husserl’s notion of truth back to Brentano and Bolzano, from where I develop a new realist interpretation. Chapter 5 discusses Husserl’s semantic restriction of meaning and shows that he is more liberal than the logical empiricists. Chapter 6 turns to the logical challenge from the Church-Fitch or knowability paradox.
</p>

<p>
Part III returns to current debates in the philosophy of science. In the final chapter 7, I extend the account developed to a Phenomenological Structural Realism. Unlike existing forms of structural realism, the phenomenological version maintains a strict distinction between perceptual and mathematical structures and thereby avoids a collapse between mathematical and physical reality.
</p>


</details>
</div>
</div>
<p>
</p>

## Research Articles

<ol reversed outside style="padding-left: 0em" start={{ site.data.research_articles.size }}>
{% for row in site.data.research_articles reversed %}
<li style="padding-left: 0.5em"> 
<details>
<summary>{{row.year}}, {{ row.authors }}: {{row.title}}. <i>{{row.venue}} </i> (<a href="{{ row.url}}">{{ row.urltext }}</a>). {{ row.extra}}
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
<ol reversed outside style="padding-left: 0em" start={{ site.data.book_reviews.size }}>
{% for row in site.data.book_reviews reversed %}
<li style="padding-left: 1em"> 
<!-- <details> -->
<!-- <summary> -->
 {{row.year}}, {{ row.authors }}: {{row.title}}, <i>{{row.venue}} </i>, <a href="{{ row.url}}">{{ row.urlstr }}</a>. {{ row.extra}}
<!-- </summary> -->
<!-- {{ row.abstract }} {{ row.abstract_extra }} -->
<!-- </details> -->
</li>
{% endfor %}
</ol>

## Presentations

<ol reversed outside style="padding-left: 0em" start={{ site.data.presentations.size }}>
{% for row in site.data.presentations reversed %}
<li style="padding-left: 1em"> 
<details>
<summary>{{row.date}}: {{row.title}}
</summary>

{{row.collaborators}}

{{ row.occasion }}
</details>
</li>
{% endfor %}
</ol>

