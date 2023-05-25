---
layout: item
title: Digital-History Scholarship of Teaching and learning
author: "Kalani Craig"
shortdesc: Published scholarship on how students learn history through digital methods, and how students learn digital methods in the classroom, has shaped some of my DBHR practices by providing different audiences whose different historical training surfaces different digital-tool-design needs
externalurl: 
embedurl: 
group: research
categories: [ Small Scale, Past, Current, Future ]
tags: [  ]
---

## Design-Based History Research in Digital History Pedagogy

As part of my DBHR practice, I've explored the ways that students work with and learn from digital-history tools and methods in the classroom. These digital-pedagogy research lines contribute new knowledge to the discipline of history in two ways.

First, history students are often learning history and digital tools in parallel. Working with digital tools that are designed from the ground up to scaffold their history learning makes for better historical thinking and higher levels of student engagement mean more budding historians entering a pipeline of practicing historians who can put their skills to use both in and outside of the university.

Second, classrooms offer larger-scale pilot testing environments. A digital tool that can support 100 students easily will function far more effectively for small teams of historians than a digital tool that has had limited testing on a smaller scale.

## Full Funding & Publication List
{: .subheadline }

{% assign itemsProject = site.data.publications | where: 'project', 'Digital History Pedagogy' | sort: "date" | reverse %}

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

## Examples 

### Black Death Agent Based Modeling

This agent-based modeling simulation of deaths from bubonic plague rendering takes my digital-tool-building into the classroom and offers a path to digital public history.

The Black Death that broke out in 1348 in medieval Europe and North Africa was caused by a bacteria (Y.Pestis), not a virus. The 1348 outbreak we all learned about in middle school wasn’t the first. It also wasn’t the last. An outbreak in the early 20th century that started in China hit Hawaii in 1899-1900 and San Francisco in 1900-1904. There were 1000 documented cases of plague in the US between 1900 and 2012, and the U.S. sees an average of 10 new cases each year, mostly in the southwest (New Mexico, Colorado and Arizona). In all of these pandemics, medical responses were shaped by social, cultural and economic norms that governed how people fit plague into their world view.

The walls around sixth-century Constantinople are roughly the square mileage of our college town but with different population densities (150K and 500-800K respectively). We used that to make context more salient in an educational intervention in a college-level introductory history course of 94 people organized into 16 tables of 6 students each:

- Students used GoogleMaps or GPS-enabled smartphones to track a day of walking in Bloomington. We then used Google Maps to provide comparisons with Constantinople’s context by asking them to trace 5 walking paths in Constantinople as a group, using the types of people they had encountered in their primary sources as a guide to creating each individual walking path and the intersections between all 5. We overlaid all of the groups' Constantinople walking paths on each other to mimic the density of their college-town walking paths in order to discuss parallels and differences with their modern college town.
- Students then interacted with an epidemiological simulation that compared population densities in Bloomington and Constantinople but also added social and cultural variables that affected medical response.
- We measured learning gains based on pre-post tests about factors that would affect the rate, speed, and response to spread of plague. Successful students in the post-test understood that Constantinople’s dense urban population and its role as a trading and government center in late Antiquity would result in much faster plague spread, a contrast with student belief that fast modern transportation would lead to faster plague spread even in less urban areas.

#### Study Outcomes

- [Read the 2015 paper](https://www.kalanicraig.com/publications/AERA-dh-and-presentism/)
- [Try the revised 2017 and 2018 activities](https://www.kalanicraig.com/workshops/black-death-maps-simulation/)