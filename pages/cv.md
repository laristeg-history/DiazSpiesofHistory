---
layout: page
title: "Curriculum Vitae"
permalink: /CV/
icon: fa-hashtag
---

<div class="printonly">
<div class="posts grid-container text-center" style="margin-bottom:1em;">
<h2  class="subheadline" style="margin-bottom:0px;">Arlene Diaz</h2>
adiaz [at] iu.edu
</div>
</div>

<h3 class="subheadline">EDUCATION</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Education' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">RECORD OF PROFESSIONAL EXPERIENCE</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Appointments' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">HONORS AND AWARDS</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Honors and Awards' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">PUBLICATIONS</h3>
<div class="posts grid-container">
<h4 class="sans CV">Book</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Book' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Manuscript in Progress</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Manuscripts' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Refereed</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Refereed' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
<h4 class="sans CV">Non-Refereed</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Non-Refereed' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
<h4 class="sans CV">Book Reviews</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Book Reviews' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
<h4 class="sans CV">Podcasts</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Podcasts' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
<h4 class="sans CV">Participation in Documentaries</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Documentaries' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">CONFERENCE PAPERS AND TALKS</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Conference Papers and Talks' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">PUBLICATIONS IN THE SCHOLARSHIP OF TEACHING AND LEARNING</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Publications in SOTL' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">PRESENTATIONS IN THE SCHOLARSHIP OF TEACHING AND LEARNING</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Presentations in SOTL' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">COURSES TAUGHT</h3>
<div class="posts grid-container">
<h4 class="sans CV">Undergraduate</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Undergraduate' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Hraduate</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Graduate' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
</div>

<h3 class="subheadline">UNIVERSITY SERVICE (Indiana University)</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'University Service' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">PROFESSIONAL ACTIVITIES</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Professional Activities' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">LANGUAGES</h3>
<div class="posts grid-container">
<div class="grid-x margin-gutters padding-gutters citation newyear">
	<div class="cell small-12">
	<ul>
	<li>Spanish</li>
	<li>English</li>
	<li>Portuguese</li>
	</ul>
	</div>
</div>
</div>{% assign previous_i = "" %}

<h3 class="subheadline">PROFESSIONAL ASSOCIATIONS</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Professional Associations' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>
