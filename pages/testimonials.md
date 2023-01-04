---
layout: default
title: Testimonials - Radical College Strategies
permalink: /Testimonials/
---

<section50short> 
<h2>Testimonials</h2>

<div class="section50left test">

  {% for comp in site.testimonialsL %}  
  <h4>{{ comp.from }} </h4>
  {{ comp.content }} 
  {% endfor %}

</div>

<div class="section50right test">

  {% for comp in site.testimonialsR %}  
  <h4>{{ comp.from }} </h4>
  {{ comp.content }} 
  {% endfor %}
  
</div>

</section50short>

<section50short> 
    {%- include buttons.html -%}
</section50short>

{%- include footer.html -%}
