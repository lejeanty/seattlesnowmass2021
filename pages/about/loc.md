---
permalink: /about/loc/
title: Local Organizing Committee
---

# Local Organizing Committee

<br/>
Please feel free to contact anyone you feel might be able to help you.
<br/>

<div class="container-fluid">
  <div class="row">
  {% for member in site.data.orgs.loc.personnel  %}
       {% assign person = site.data.people[member] %}
       {% include standard_person_card.md %}
  {% endfor %}
  </div>
</div>
<br/>
