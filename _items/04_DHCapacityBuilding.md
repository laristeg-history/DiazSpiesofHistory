---
layout: item
title: Digital Humanities Capacity-Building Research
author: "Kalani Craig"
shortdesc: This strand of research draws on journey-mapping and digital-pedagogy research to understand which approaches to faculty and graduate-student digital arts and humanities training are most effective.
externalurl: 
embedurl: 
group: research
categories: [ Small Scale, Current, Future ]
tags: [  ]
---


## Full Funding & Publication List
{: .subheadline }

{% assign itemsProject = site.data.publications | where: 'project', 'Digital Humanities Professional Development' | sort: "date" | reverse %}

{% assign itemsSorted = itemsProject | where: 'section', 'Grants' | sort: "date" | reverse %}
{% if itemsSorted and itemsSorted.size != 0 %}
<h3>Grants</h3>
<div class="posts grid-container">
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign previous_i = "" %}{% assign itemsSorted = nil %}
</div>
{% endif %}

{% assign itemsSorted = itemsProject | where: 'group', 'Digital History Publications' | sort: "date" | reverse %}
{% if itemsSorted and itemsSorted.size != 0 %}
<h3>Digital History Publications</h3>
<div class="posts grid-container">
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign previous_i = "" %}{% assign itemsSorted = nil %}
</div>
{% endif %}

{% assign itemsSorted = itemsProject | where: 'group', 'Text-Based Publications' | sort: "date" | reverse %}
{% if itemsSorted and itemsSorted.size != 0 %}
<h3>Text Based Publications</h3>
<div class="posts grid-container">
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign previous_i = "" %}{% assign itemsSorted = nil %}
</div>
{% endif %}

{% assign itemsSection = itemsProject | where: 'group', 'Presentations' | sort: "date" | reverse %}
{% if itemsSection and itemsSection.size != 0 %}
<h3>Presentations</h3>
<div class="posts grid-container">
{% assign itemsSorted = itemsProject | where: 'section', 'Peer-reviewed Conference Proceedings' | sort: "date" | reverse %}
{% if itemsSorted and itemsSorted.size != 0 %}
<h3>Peer-reviewed Conference Proceedings</h3>
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign previous_i = "" %}{% assign itemsSorted = nil %}
{% endif %}

{% assign itemsSorted = itemsProject | where: 'section', 'Invited Talks & Workshops' | sort: "date" | reverse %}
{% if itemsSorted and itemsSorted.size != 0 %}
<h3>Invited Talks & Workshops</h3>
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign previous_i = "" %}{% assign itemsSorted = nil %}
{% endif %}

{% assign itemsSorted = itemsProject | where: 'section', 'Conference Presentations' | sort: "date" | reverse %}
{% if itemsSorted and itemsSorted.size != 0 %}
<h3>Conference Presentations</h3>
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign previous_i = "" %}{% assign itemsSorted = nil %}
{% endif %}
</div>
{% endif %}