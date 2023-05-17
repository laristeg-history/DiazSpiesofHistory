---
layout: item
title: Net.Create
author: "Kalani Craig and Joshua Danish with Inquirium"
shortdesc: "Net.Create is an open-source network-analysis tool that offers simultaneous multi-user network-data entry, accommodates duplicate and ambiguous network data, provides live visualizations of up-to-the-minute entries from other team members, and is structured around historiographically driven citational and interpretive practices."
externalurl: http://www.netcreate.org
embedurl: 
group: research
categories: [ DBHR, Digital Tool Building, Digital Pedagogy ]
tags: [  ]
---

Net.Create is an open-source network-analysis tool that offers simultaneous multi-user network-data entry, accommodates duplicate and ambiguous network data, provides live visualizations of up-to-the-minute entries from other team members, and is structured around historiographically driven citational and interpretive practices.

## My Role

I started Net.Create as a solo researcher in Fall of 2015 and was responsible for the first three rounds of software and methods design (Fall 2015 through Spring 2018). With internal funding from IU, I identified a research team of educational researchers and an external software development firm with whom to work. Since 2018, I have led the Net.Create team in designing new features, identifying and documenting methods for using those features in history research environments, and developing activities for classroom use of Net.Create.

## Current Status

Net.Create is currently available for free for MacOS users or for ~$5/month at Digital Ocean. All of the features described in [The Journal of Digital History DBHR article](https://journalofdigitalhistory.org/en/notebook-viewer/JTJGcHJveHktZ2l0aHVidXNlcmNvbnRlbnQlMkZrYWxhbmljcmFpZyUyRmRiaHJfamRoMjAyMyUyRm1hc3RlciUyRndvcmslMkZhdXRob3JfZ3VpZGVsaW5lX3RlbXBsYXRlLmlweW5i) are included in the current version of Net.Create.

## Future Plans

Net.Create's next steps include another series of grant-funded features identified in our last DBHR include:

- a 1-click process that bypasses some of the more technical requirements for software installation
- Integrated data provenance. We have it but it's in logs, and we'd like to make that more accessible to the team. Provenance supports better researcher positionality (MMATCH as part of the Net.Create DBHR process)
- Integrated commenting. This lets the team have a staged historiographic debate in an asynch collaboration environment without directly changing the node/edge data
- Private comments. This lets each member of the team take separate notes as part of their own historian's work.

## Examples of Net.Create in use

- http://theraptlab.org/projects/netcreate_examples
- https://camullenphd.github.io

## Full Funding & Publication List

<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'project', 'Net.Create' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
