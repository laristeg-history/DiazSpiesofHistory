---
layout: page
title: "Grant Applications"
permalink: /research/grants/
icon: fa-hashtag
---

I've sought grant support for three strands of research.

1. The bulk of my successful grant activity to date has been for [Net.Create](/items/01_netcreate.html), which is the most mature of my research products.
1. Prior to Net.Create, I started my [digital-humanities capacity-building grants](/items/04_DHCapacityBuilding.html) research strand with two early grants (Making the Arts & Humanities, Crowdsourcing the Digital Primary Source Index); an additional DH capacity building grant in progress and slated for submission in September 2023.
1. One [digital community-archiving grant](/items/02_communityarchive.html) ("Crossroads of America") is emblematic of my digital-history tool building goals for the next few years, with a follow-up grant in process for submission to the NEH in October of 2023.

<h2 class="subheadline">External Grants</h2>

<h3>Awarded</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'section', 'External' | sort: "date" | reverse %}
{% assign itemsAwarded = itemsSorted | where: 'type', 'Awarded' | sort: "date" | reverse %}
{% for item in itemsAwarded %}
{% include _citation_abstract.html %}
{% endfor %}
</div>

<h3>Not Funded</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'section', 'External' | sort: "date" | reverse %}
{% assign itemsAwarded = itemsSorted | where: 'type', 'Rejected' | sort: "date" | reverse %}
{% for item in itemsAwarded %}
{% include _citation_abstract.html %}
{% endfor %}
</div>

<h2 class="subheadline">Internal Grants</h2>
<h3>Awarded</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'section', 'Internal' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation_abstract.html %}
{% endfor %}
</div>
