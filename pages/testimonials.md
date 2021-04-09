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
    <p style="text-align:center;"><a href="/YourJourney" class="mybutton" style=" color:white">Begin Your Journey</a></p>
</section50short>

<div class="license" style="float:right">
<a href="/Privacy" target="_blank" style="color: #0821af;">Privacy Policy</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Terms" target="_blank" style="color: #0821af;">Terms</a>
<br>
<br>
</div>
