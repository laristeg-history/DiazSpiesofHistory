---
layout: item
title: Mixed Method Approaches to Collaborative History (MMATCH)
author: "Kalani Craig with Arlene Diaz"
shortdesc: Mixed Method Approaches to Collaborative History (MMATCH) is a mixed-methods approach that blends close reading and new historical methods by emphasizing transparency and collaboration. The five-step MMATCH methodology systematically navigates a revision and integration process of writing that moves between traditional close-reading historical analysis and new analytical methods. As part of that systematic process, it simultaneously accommodates the voices of multiple authors.
externalurl: 
embedurl: 
group: research
categories: [ DBHR, Digital Tool Building, Digital Pedagogy ]
tags: [  ]
---

Mixed Method Approaches to Collaborative History (MMATCH) is a mixed-methods approach that blends close reading and new historical methods by emphasizing transparency and collaboration. The five-step MMATCH methodology systematically navigates a revision and integration process of writing that moves between traditional close-reading historical analysis and new analytical methods. As part of that systematic process, it simultaneously accommodates the voices of multiple authors. MMATCH is rooted in my computational-text-analysis digital history work.

### MMATCH and Computational Text Analysis as a DBHR Project

http://kalanicraig.com/AHRDiachronicConversation/indexmarkdown.html

## Full Funding & Publication List

<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'project', 'Computational Text Analysis' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
