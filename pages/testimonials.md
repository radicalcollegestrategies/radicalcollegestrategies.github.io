---
layout: default
permalink: /testimonials/
---

<section50short> 
<h2>Testimonials</h2>

{% for comp in site.testimonials %}  

  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  <!--
  {% if mod == 0 %}
  <div class="section50right test">
  {% else %}
  <div class="section50left test">
  {% endif %}
  -->
  <div class="section50left test">

  <h4>{{ comp.from }} </h4>

  {{ comp.content }} 

  </div>

<!--
  {% if mod == 0 %}
  </section50short>
  <section50short> 
  {% endif %} -->

{% endfor %}
</section50short>
<br>
<br>
