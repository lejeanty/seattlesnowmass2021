<div class="card" style="width: 12rem;">
   <img class="card-img-top" src="{{person.photo | relative_url}}" alt="Card image cap">
   <div class="card-body d-flex flex-column">
      <div class="card-text">
         {% if person.website and person.website != blank %}
            <b><a href="{{person.website}}">{{person.name}}</a></b>
         {% else %}
            <b>{{person.name}}</b>
         {% endif %}
         <br>
         <div style="font-size: 0.7rem">
            <a href="mailto:{{person.email}}?subject = Seattle Snowmass 2021 Question">email</a>
         </div>
         {% if person.duties and person.duties != blank %}
            <div class="card-text" style="font-size: 0.75rem; font-style: italic">
               {% for duty in person.duties %}
                  {{site.data.duties[duty]}}{% if forloop.last %}{% else %},{% endif %}
               {% endfor %}
            </div>
         {% endif %}
         <div style="font-size: 0.75rem"><br>{{person.institution}}</div>
         <div class="card-text mt-auto"><i>{{person.title}}</i></div>
      </div>
   </div>
</div>
