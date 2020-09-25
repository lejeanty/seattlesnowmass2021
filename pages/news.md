---
permalink: /news/
title: All Snowmass 2021 Posts
---

<div class="mainpage-news mainpage-core">

<div class="container-fluid">
  <div class="news row">
    {% for post in site.posts%}
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
