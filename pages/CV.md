---
layout: page
title: "Curriculum Vitae"
permalink: /CV/
icon: fa-hashtag
---

<div class="printonly">
<div class="posts grid-container text-center" style="margin-bottom:1em;">
<h2  class="subheadline" style="margin-bottom:0px;">Kalani Craig</h2>
kalani [at] kalanicraig.com
</div>
</div>

<h3 class="subheadline">Education</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Education' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">Appointments</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Appointments' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">Grants, Fellowships & Awards</h3>
<div class="posts grid-container">
<h4 class="sans CV">Grants</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Grants' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Awards</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Awards' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Fellowships</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Fellowships' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>


<h3 class="subheadline">Digital History Publications</h3>
<div class="posts grid-container">
<h4 class="sans CV">Digital History Tools</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Digital History Tools' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Digital History Exhibits</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Digital History Exhibits' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>

<h3 class="subheadline">Text-Based Publications</h3>
<div class="posts grid-container">
<p class="quiet"><em>* = graduate student at time of publication</em></p>
<h4 class="sans CV">Refereed Articles</h4>
{% assign newset = "" | split:"" %}
{% for item in site.data.publications %}
  {% if item.section == "Refereed Articles" %}
    {% assign newset = newset | push: item %}
  {% endif %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', 'in press' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', '' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Book Chapters</h4>
{% assign newset = "" | split:"" %}
{% for item in site.data.publications %}
  {% if item.section == "Book Chapters" %}
    {% assign newset = newset | push: item %}
  {% endif %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', 'in press' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', '' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Book Reviews</h4>
{% assign newset = "" | split:"" %}
{% for item in site.data.publications %}
  {% if item.section == "Book Reviews" %}
    {% assign newset = newset | push: item %}
  {% endif %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', 'in press' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', '' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Manuscripts in Preparation</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Manuscripts in Preparation' | sort: "date" %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Whitepapers & Service</h4>
{% assign newset = "" | split:"" %}
{% for item in site.data.publications %}
  {% if item.section == "Whitepapers & Service" %}
    {% assign newset = newset | push: item %}
  {% endif %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', 'in press' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', '' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>{% assign previous_i = "" %}

<h3 class="subheadline">Presentations</h3>
<div class="posts grid-container">
<h4 class="sans CV">Invited Talks & Workshops</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Invited Talks & Workshops' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Peer-reviewed Conference Proceedings</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Peer-reviewed Conference Proceedings' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Conference Presentations</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Conference Presentations' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Campus & Departmental Talks</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Campus & Departmental Talks' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Media Coverage</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Media Coverage' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>{% assign previous_i = "" %}

<h3 class="subheadline">Teaching & Learning</h3>
<div class="posts grid-container">
<h4 class="sans CV">COVID Instructional Training & Teaching Consults</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'COVID' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Undergraduate Courses Taught</h4>
{% assign courses_grouped = site.data.courses | where: 'courselevel', 'Undergraduate' | group_by: 'coursegroup' | sort: "date" | reverse %}
{% for group in courses_grouped %}
<p>{{group.name}}
{% for item in group.items %}
{{item.coursesemester}};
{% endfor %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Graduate Courses Taught</h4>
{% assign courses_grouped = site.data.courses | where: 'courselevel', 'Graduate' | group_by: 'coursegroup' | sort: "date" | reverse %}
{% for group in courses_grouped %}
<p>{{group.name}}
{% for item in group.items %}
{{item.coursesemester}};
{% endfor %}
{% endfor %}{% assign previous_i = "" %}

<h3 class="subheadline">Service & Professional Organizations</h3>
<div class="posts grid-container">
<h4 class="sans CV">National & International Service</h4>
{% assign newset = "" | split:"" %}
{% for item in site.data.publications %}
  {% if item.section == "National & International" %}
    {% assign newset = newset | push: item %}
  {% endif %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', 'present' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', '' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Peer Review</h4>
{% assign itemsSorted = site.data.publications | where: 'section', 'Peer Review' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">University Service</h4>
{% assign newset = "" | split:"" %}
{% for item in site.data.publications %}
  {% if item.section == "University" %}
    {% assign newset = newset | push: item %}
  {% endif %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', 'present' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
{% assign itemsSorted = newset | where: 'status', '' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}{% assign previous_i = "" %}
<h4 class="sans CV">Professional Organizations</h4>
<div class="grid-x margin-gutters padding-gutters citation newyear">
	<div class="cell small-12 medium-6">
	<ul>
	<li>American Historical Association</li>
	<li>Medieval Academy of America</li>
	<li>EPISCOPUS, Society for the Study of Bishops and Secular Clergy in the Middle Ages</li>
	</ul>
	</div>
	<div class="cell small-12 medium-6">
	<ul>
	<li>Society for Late Antiquity</li>
	<li>Phi Alpha Theta</li>
	</ul>
	</div>
</div>
</div>{% assign previous_i = "" %}

<h3 class="subheadline">Professional Qualifications</h3>
<div class="posts grid-container">
<div class="grid-x margin-gutters padding-gutters citation newyear">
	<div class="cell small-12 medium-6">
	<h4 class="sans CV">Languages</h4>
	<ul>
	<li>Fluent written and spoken Italian</li>
	<li>Fluent written French and Latin</li>
	<li>Intermediate reading comprehension in German</li>
	<li>Basic reading comprehension in Portuguese and Spanish</li>
	</ul>
	</div>
	<div class="cell small-12 medium-6">
	<h4 class="sans CV">Design, Programming & Editing</h4>
	<ul>
	<li>Expert Web design, database & programming (Python, PHP, CSS, SQL, HTML, Liquid, Jekyll/Github Pages, XML)</li>
	<li>Expert Adobe Creative Suite (Photoshop, Illustrator)</li>
	<li>Expert MS Office (Excel, PowerPoint, Word)</li>
	<li>Expert copy editor (AP style, Chicago style)</li>
	</ul>
	</div>
</div>
</div>{% assign previous_i = "" %}

<h3 class="subheadline">Relevant Professional Experience</h3>
<div class="posts grid-container">
{% assign itemsSorted = site.data.publications | where: 'group', 'Relevant Professional Experience' | sort: "date" | reverse %}
{% for item in itemsSorted %}
{% include _citation.html %}
{% endfor %}
</div>