---
layout: item
title: Net.Create
author: "Kalani Craig and Joshua Danish with Inquirium"
shortdesc: "Net.Create is an open-source network-analysis tool that offers simultaneous multi-user network-data entry, accommodates duplicate and ambiguous network data, provides live visualizations of up-to-the-minute entries from other team members, and is structured around historiographically driven citational and interpretive practices."
externalurl: http://www.netcreate.org
embedurl: 
group: research
categories: [ Large Scale, Past, Current, Future ]
tags: [  ]
---

## Net.Create as Historical Research

While there are several research implications for historians documented in the *Journal of Digital History* article, "[Designing Our Digital Past: Anchoring Digital-History Tool Development in the Historical Method Through Design-Based History Research](https://journalofdigitalhistory.org/en/notebook-viewer/JTJGcHJveHktZ2l0aHVidXNlcmNvbnRlbnQlMkZrYWxhbmljcmFpZyUyRmRiaHJfamRoMjAyMyUyRm1hc3RlciUyRndvcmslMkZhdXRob3JfZ3VpZGVsaW5lX3RlbXBsYXRlLmlweW5i)", the single most important contribution Net.Create makes to digital-history research is in the preservation of citations and research notes. No other network analysis tool offers built-in citation preservation to its users. The connections documented in other network analysis tools can be analyzed but not traced back to the primary sources from which they came, and so Net.Create provides a historiographic-debate platform as well as a network-analysis platform.

## My Role

I started Net.Create as a solo researcher in Fall of 2015 and was personally responsible for the first three rounds of software develoopment and methods design (Fall 2015 through Spring 2018).

With internal funding from IU, I identified a research team of educational researchers and an external software development firm with whom to work ([Inquirium](https://www.inquirium.net)). Since then, I have led the Net.Create team in designing new features, identifying and documenting methods for using those features in history research environments, and developing activities for classroom use of Net.Create.

## Current Status

Net.Create is currently available for free for MacOS users or for ~$5/month at Digital Ocean.

All of the DBHR features described in the *Journal of Digital History* article, "[Designing Our Digital Past: Anchoring Digital-History Tool Development in the Historical Method Through Design-Based History Research](https://journalofdigitalhistory.org/en/notebook-viewer/JTJGcHJveHktZ2l0aHVidXNlcmNvbnRlbnQlMkZrYWxhbmljcmFpZyUyRmRiaHJfamRoMjAyMyUyRm1hc3RlciUyRndvcmslMkZhdXRob3JfZ3VpZGVsaW5lX3RlbXBsYXRlLmlweW5i)" are included in the current version of Net.Create.

### Resources and Guides

The current version of Net.Create uses NodeJS (v10.22.0) and React installed in either a MacOS environment or in a Digital Ocean droplet.

- [Technical documentation](https://github.com/netcreateorg/netcreate-2018/blob/master/README.md)
- [Installation documentation](https://netcreate.org/documentation/)
- [Quick-Start User Guide](https://netcreate.org/userguide/)

## Future Plans

Net.Create's next steps include another series of grant-funded features identified in our last DBHR include:

- a 1-click process that bypasses some of the more technical requirements in the current installation process
- Integrated data provenance. We have it but it's in logs, and we'd like to make that more accessible to the team. Provenance supports better researcher positionality (MMATCH as part of the Net.Create DBHR process)
- Integrated commenting. This lets the team have a staged historiographic debate in an asynch collaboration environment without directly changing the node/edge data
- Private comments. This lets each member of the team take separate notes as part of their own historian's work.

## Examples of Net.Create in use

- http://theraptlab.org/projects/netcreate_examples <!--explain-->
- https://camullenphd.github.io <!--explain-->
- http://samplenetworks.kalanicraig.com/?dataset=gesta#/ <!--explain-->

## Full Funding & Publication List
{: .subheadline }

Net.Create has been funded by NSF awards #[1848655](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1848655) and #[2241705](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2241705) and by Lumina Foundation.

{% assign itemsProject = site.data.publications | where: 'project', 'Net.Create' %}

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

