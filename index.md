---
title: Seattle Snowmass Summer Study 2022
subtitle: >
  July 17-26, 2022 at the University of Washington
hero_image: assets/images/uw-fountain.jpg
---

Welcome to the Seattle Community Summer Study Workshop home page!

The Seattle meeting is the culmination of the various workshops and Town Hall meetings that have taken place during 2020, 2021, and 2022 as part of Snowmass21. As we have throughout the Snowmass process, we aim for everyone's voice to be heard. Contributions and participation from the community in this workshop are critical for the success of Snowmass21 and they will occur as part of one or more working groups directed by conveners.

Feel free to [send us an email](snowmass-loc2022@uw.edu) if there is information you can't find from the set of drop-down menus above, or the news items below!

<div class="mainpage-news mainpage-core">
<h4>Recent News:</h4>

<div class="container-fluid">
  <div class="news row" style="display: flex; flex-direction: row; flex-wrap: wrap;">
    {% for post in site.posts limit:4 %}
       <div class="card news" style="width: 20rem; margin: 3px">
          <a href="{{post.url}}">
          <img class="card-img-top" src="{{post.postimage}}" alt="Card image cap" style="width: 18rem; display:block; margin-left: auto; margin-right: auto">
          </a>
          <div class="card-body d-flex flex-column">
            <div class="card-text card-title">
               <a href="{{post.url}}">{{post.title}}</a>
            </div>
            <div class="card-text card-body">
              {% if post.summary %}
                  {{ post.summary | markdownify }}
              {% else %}
                  {{ post.excerpt | strip_html }}
              {% endif %}
            <a href="{{post.url}}">Read more</a></div>
          </div>
       </div>
    {% endfor %}
  </div>
</div>

<a href="/news">View all past news items</a>
</div>

We acknowledge we are on Coast Salish territory, the traditional homeland of the Duwamish, Suquamish, Tulalip, and Muckleshoot nations and other Native peoples.
