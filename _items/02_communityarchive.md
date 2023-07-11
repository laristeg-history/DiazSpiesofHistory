---
layout: item
title: Community Archive Digital Projects
author: "Kalani Craig with IDAH, CRRES, Marisa Hicks Alcaraz and Jazma Sutton"
shortdesc: My digital-tool design work for community archiving and digital exhibits speaks to a need to support archiving projects in a minimal-computing environment that requires limited expertise and money to set up and guides contributors through specific historical-thinking tasks. 
externalurl: http://community-archive.kalanicraig.com
embedurl: 
group: research
categories: [ Large Scale, Past, Current, Future ]
tags: [  ]
---

Every day, we make history. It’s in what we eat, what we say, what we post to social media. It’s also in our homes, our backpacks and our classrooms. My digital-tool design work for community archiving and digital exhibits speaks to a need to support archiving projects in a minimal-computing environment that requires limited expertise and money to set up and guides contributors through specific historical-thinking tasks. 

## Digital Community Engagement as Historical Research

My work in digital community archiving started in the classroom, as part of a curricular-development project focused on undergraduate research experiences. In early 2019, I led a classroom of first-year researchers through the process of a History Harvest. That, in turn, led to a series of questions about the tools most commonly used for History Harvests.

The two primary considerations for an ethically shaped community archive are the archive's longevity, and community control and ownershiip of an archive. Both shape the access future historians have to community-driven archives, the former by making access over a longer term possible and the latter by shaping future historians' work based on community-driven principles of what should and should not be preserved. The latter makes it more likely that communities will fully engage with the interpretation and preservation of their own history.

With these disciplinary considerations in mind, I applied my experience with Net.Create's DBHR process to the evaluation of community archiving workflows and identified several community and researcher needs:

- a low-cost approach to physical preservation tasks. A photo lightbox made of cardboard, tissue paper, and desk lamps made it possible to use smartphones instead of expensive DSLRs. This made preservation of more objects more likely.
- a low-cost approach to the web-site creation portion of a digital exhibit. This makes for a more stable archive and a larger archive (since larger web sites with more images are often associated with higher costs)
- a long-term digital-preservation strategy that results in a static site rather than a dynamically generated site. In less technical terms, that means a site that doesn't use databases or heavy programming to generate the page for each item in a community archive. Static sites have a much longer life span and are less likely to need regular updates to be maintain their legibility.

I worked to identify templating needs with the Center for Research on Race, Ethnicity and Society, the Asian Culture Center at Indiana University Bloomington, Jazma Sutton and the Remembering Freedom descendant community in Greenville and Longtown, Ohio, and ImaginX en Movimiento (IXeM, co-founded by Marisa Hicks-Alcaraz). Feedback from these, and other, partners, and observations made over several completed History Harvests, allowed for the revision of these tool features and workflow approaches that would encourage historical thinking, thoughtful archival practices, and community contributions.

### My Role

Like Net.Create, the current version of the Community-Archive template is built around several Design-Based History Research adaptations.

Initially, I adapted an existing static-site template ([https://www.wowthemes.net/mediumish-free-jekyll-template/](Mediumish)) and used Jekyll and Github Pages to generate a digital-exhibit website for the first-year-research-project History Harvest in Spring of 2019. I then revised that theme adaptation in Fall of 2019, with the spring 2019 and a summer user-group test in mind. A third theme adaptation in Spring of 2020 to begin the Remembering Freedom web site, provided a clear platform for testing and an initial list of revision needs.

One primary revision priority came out of those three initial tests. Our adaptation of an existing website theme allowed us to build digital-exhibit information requirements for metadata, oral histories, and argument-driven histories into a digital exhibit. However, these themes were overly complex because they were designed to serve any website need any random internet user might have. In order to provide a digital-exhibit platform anyone could use, we needed something purpose-built for community histories.

I started building a Community-Archive Jekyll Theme template from scratch in winter of 2022 and completed a test version in early summer of 2022. In the year since, I have revised it three times in response to new and ongoing community-archive projects, digital exhibits, and other related digital-humanities-scholarship and digital-public history needs, *including this dossier*.

### Current Status

The Community-Archive Jekyll Theme was made available for use by any member of the public at https://community-archive.kalanicraig.com in October of 2022. Version 4.0 is still officially labeled as a "beta" or test release, largely because it needs more widespread testing with external partners, but the example site at https://github.com/idahatiu/idahatiu.github.io has already been "forked", or used, by 8 people since October and there are 5 more community-archive projects in the work.

### Resources and Guides

A Quick-Start guide provides a fast way to get a community archive going; estimated start-up time for first-time users is about an hour. The theme documentation provides more detail for digital historians and digital humanists seeking to customize the theme for their own use.

- [Quick-Start User Guide](https://community-archive.kalanicraig.com/quickstart)
- [Theme documentation](https://community-archive.kalanicraig.com/docs)

### Future Plans

In addition to historians and art historians outside of IU who have worked with the Community-Archive Jekyll Theme, I'm engaged in planning for several upcoming community-archive or digital-history-exhibit projects, which will provide several rounds of public-history-driven revisions with
- La Casa (IU's Latine student organization which celebrates its 50th anniversary in October)
- Asian Cultural Center (IU's Asian/Pacific Islander student organization which celebrates its 25th anniversary in October)
- MARCH, a consortium of digital public historians and media-studies scholars in the Midwest seeking a grant from the NEH to hold a train-the-trainer community-archiving workshop in Summer of 2024

## Examples of Version 4.0 (beta) in action

Release of version 4.0 is scheduled for late summer 2023, after comprehensive pilot testing in the IDAH Summer Incubator and full theme documentation development.

- **This dossier!** One of my goals has been to advance digital-history and digital-humanities scholarly communication. Using the Community-Archive Jekyll Theme for this dossier provides an additional use-case example for other academics struggling to present their digital scholarship.
- [A Sample Collection](https://idahatiu.github.io): This example collection was built by members of the IDAH staff independently to serve as a platform for community partners to use as an example/template site with fewer moving parts than the full Community-Archive Jekyll Theme itself.
- [Home Bound](https://homeboundatiu.github.io): Home Bound is an art exhibition curated by featuring artworks that each visualize aesthetic concepts of “home.” 

## Full Funding & Publication List
{: .subheadline }

{% assign itemsProject = site.data.publications | where: 'project', 'History Harvest' %}

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

