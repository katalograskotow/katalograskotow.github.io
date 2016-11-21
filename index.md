---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

  <nav class="purple">
    <div class="nav-wrapper">
      <a href="#!" class="brand-logo center"><i class="material-icons">mood</i>Katalog ras kotow</a>
      <ul class="left hide-on-med-and-down">
        <li><a href="http://localhost:4000/about/">Informacje o stronie</a></li>
        <li lass="active"><a href="badges.html">Rasy</a></li>
        <li c><a href="collapsible.html">Konktakt</a></li>
      </ul>
    </div>
  </nav>
<div class="card-panel purple lighten-3">
  <span class="white-text text-darken-2 "><h4>Posty:</h4></span>
  </div>


{% for posts in site.posts %}
<div class="col s12 m6 offset-m2 l3 offset-l3">
 <div class="card-panel purple lighten-5 z-depth-2">
   <div class="row valign-wrapper">
     <div class="col s3">
       <img src="http://image.shutterstock.com/z/stock-vector-cute-sad-grumpy-cat-in-material-design-style-vector-illustration-406208077.jpg" alt="" class="circle responsive-img"> <!-- notice the "circle" class -->
     </div>
     <span class="black-text">
      {{posts.date}}
     </span>
    <div class="col s10">
       <span class="black-text">
        <h4>{{posts.title}}</h4>
       </span>
       <span class="black-text truncate">
        {{posts.text}}
       </span>
         <li><a href="{{posts.url}}">Przejdź do posta</a></li>
     </div>
   </div>
 </div>
</div>
{% endfor %}


<div class="card-panel purple lighten-3">
    <span class="white-text text-darken-2">Copyright by Anna Topola</span>
  </div>
