---
layout: item
title: Mixed Method Approaches to Collaborative History (MMATCH)
author: "Kalani Craig with Arlene Diaz"
shortdesc: Mixed Method Approaches to Collaborative History (MMATCH) is a mixed-methods approach that started with my own work in computational text analysis and has developed into a collaboration process that emphasizes transparency and positionality. The five-step MMATCH methodology systematically navigates a revision and integration process of writing that moves between traditional close-reading historical analysis and new analytical methods. As part of that systematic process, it simultaneously accommodates the voices of multiple authors.
externalurl: 
embedurl: 
group: research
categories: [ DBHR, Digital Tool Building, Digital Pedagogy ]
tags: [  ]
---

Mixed Method Approaches to Collaborative History (MMATCH) is a mixed-methods approach that started with my own work in computational text analysis and has developed into a collaboration process that emphasizes transparency and positionality. The five-step MMATCH methodology systematically navigates a revision and integration process of writing that moves between traditional close-reading historical analysis and new analytical methods. As part of that systematic process, it simultaneously accommodates the voices of multiple authors.

### MMATCH and Computational Text Analysis as a DBHR Project

The world of text mining—particularly low-barrier-to-entry topic modeling with MALLET and work with AntConc or NTLK—opens up a whole variety of analytical options for scholars interested in pursuing computational text analysis. The reality of the data landscape for digital humanists, though, is that many digitized and transcribed texts have very restrictive copyright and usage guidelines that limit applications of text mining, hGIS and network-theoretical approaches. In these instances, full-text download and off-the-shelf analysis are often not an option.  In these cases, in-text citations become an absolutely vital part of the digital analysis. However, readily available topic modeling tools like MALLET strip the citation data scholars, digital and analog alike, need to participate in a scholarly debate.

This citational concern was the initial platform for a Workflow for Paywalled Texts that documents the cleaning and treatment of digitized texts that preserves the original word order and citations so that scholars of both traditional and digital-methods persuasions can recreate the process.

Work with other historians and humanists at Indiana University on citation preservation in computational text analysis fostered several collaborations, one of which became the full articulation of MMATCH in an article submitted in 2022 and forthcoming in 2023.

## Full Funding & Publication List

<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'project', 'Computational Text Analysis' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
