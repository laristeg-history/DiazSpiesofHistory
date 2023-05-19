---
layout: item
title: Community Archive Digital Projects
author: "Kalani Craig with IDAH, CRRES, Marisa Hicks Alcaraz and Jazma Sutton"
shortdesc: My digital-tool design work for community archiving and digital exhibits speaks to a need to support archiving projects in a minimal-computing environment that requires limited expertise and money to set up and guides contributors through specific historical-thinking tasks. 
externalurl: http://community-archive.kalanicraig.com
embedurl: 
group: research
categories: [ DBHR, Digital Tool Building, Digital Pedagogy, Digital Public History ]
tags: [  ]
---

Every day, we make history. It’s in what we eat, what we say, what we post to social media. It’s also in our homes, our backpacks and our classrooms. My digital-tool design work for community archiving and digital exhibits speaks to a need to support archiving projects in a minimal-computing environment that requires limited expertise and money to set up and guides contributors through specific historical-thinking tasks. 

## A DBHR Accounting of my Digital Community Archiving Tool-Design work

### My Role

I worked to identify templating needs with ImaginX en Movimiento (IXeM) co-founded by Marisa Hicks-Alcaraz, the Center for Research on Race, Ethnicity and Society, the Asian Culture Center at Indiana University Bloomington, and Jazma Sutton and the Remembering Freedom descendant community in Greenville and Longtown, Ohio. Feedback from partners, and observations made over several completed History Harvests, generated a list of features that would encourage historical thinking, thoughtful archival practices, and community contributions.

I used that list to build a new version of the Community-Archive Jekyll Theme from scratch in winter and spring of 2022. Since then, I have revised it several times in response to new and ongoing community-archive projects, digital exhibits, and other related public history needs, *including this dossier*.

### Current Status

The Community-Archive Jekyll Theme is free and available for use by any member of the public at https://community-archive.kalanicraig.com . A Quick-Start guide demonstrates its use and theme documentation provides more detail for digital historians and digital humanists seeking to customize the theme.

### Future Plans

In addition to historians and art historians outside of IU who have worked with the Community-Archive Jekyll Theme, I'm engaged in planning for several upcoming community-archive or digital-history-exhibit projects, which will provide several rounds of public-history-driven revisions with
- La Casa (IU's Latine student organization which celebrates its 50th anniversary in October)
- Asian Cultural Center (IU's Asian/Pacific Islander student organization which celebrates its 25th anniversary in October)
- MARCH, a consortium of digital public historians and media-studies scholars in the Midwest seeking a grant from the NEH to hold a train-the-trainer community-archiving workshop in Summer of 2024

## Highlights & Examples

- This dossier!
- https://idahatiu.github.io
- https://homeboundatiu.github.io

## Full Funding & Publication List

<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'project', 'History Harvest' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
