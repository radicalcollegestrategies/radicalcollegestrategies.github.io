---
layout: default
permalink: /testimonials/
---

<section50short>
<h1>Testimonials</h1>
</section50short>
<br>

<section50short> 

{% for comp in site.testimonials %}  

  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}
  <div class="section50right test">
  {% else %}
  <div class="section50left test">
  {% endif %}

  <h3>{{ comp.from }} </h3>

  {{ comp.content }} 

  </div>
{% endfor %}

</section50short>
