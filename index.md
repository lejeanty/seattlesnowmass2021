---
title: Seattle Snowmass Summer Study 2021
subtitle: >
  July 11-20, 2021 in Seattle (COVID Willing)
hero_image: assets/images/uw-fountain.jpg
---

<div class="mainpage-news mainpage-core">
<h4>News and Featured Stories:</h4>

<div class="container-fluid">
  <div class="news row">
    {% for post in site.posts limit:4 %}
       <div class="card news" style="width: 30rem">
          <a href="{{post.url}}">
          <img class="card-img-top" src="{{post.postimage}}" alt="Card image cap">
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

<a href="/news.html">View all past news items</a>
</div>
