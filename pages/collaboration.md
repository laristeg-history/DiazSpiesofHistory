---
layout: page
title: "Research Collaboration Record"
permalink: /research/collaboration/
icon: fa-hashtag
---

<h3>Awarded Grants</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'section', 'External' | sort: "date" | reverse %}
{% assign itemsAwarded = itemsSorted | where: 'type', 'Awarded' | sort: "date" | reverse %}
{% for item in itemsAwarded %}
{% include _citation_collaboration.html %}
{% endfor %}
</div>

<h3>Digital History Publications</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Digital History Publications' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation_collaboration.html %}
{% endfor %}
</div>

<h2 class="subheadline">Text-Based Publications</h2>
<h3>Peer Reviewed Journal Article</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'section', 'Refereed Articles' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation_collaboration.html %}
{% endfor %}
</div>

<h3>Peer Reviewed Conference Proceedings</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'section', 'Internal' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation_collaboration.html %}
{% endfor %}
</div>
