---
title: "ТИМ"
bg: yellow
color: ink
fa-icon: user
iconclr: '#a8201b'
titleclr: '#a8201b'
---

<div class="team">
<div class="row" style="justify-content:center;"> 

{% for person in site.data.committee.people %}
<div class="col-md-4">
<center>
<div class="team-player">


{% if person.image %}
<img src="img/organization/{{ person.image }}" alt="{{ person.name }}" class="img-raised img-circle" style="width:194px;height:194px;border-radius: 50%;">
{% else %}
<div class="photo-placeholder" aria-label="{{ person.name }}"><i class="fa fa-user"></i></div>
{% endif %}
    <h4 class="title" style="color: #2b211c;">{{ person.name }}<br>
        <small class="text-muted" style="color: #a8201b;">{{ person.title }}</small>
    </h4>
    <p class="description" style="color: #2b211c;"> {{ person.affiliation }}</p>
</div>
</center>
</div>
  {% endfor %}
  </div>
</div>
