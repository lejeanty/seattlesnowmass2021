---
title: Team
permalink: /about/team/
---

# Team


<div class="container-fluid">
  <div class="row" style="display: flex; flex-wrap: wrap">
    {% for member in site.data.people  %}
        {% assign person = member[1] %}
        {% include standard_person_card.md %}
    {% endfor %}
  </div>
</div>
<br/>
