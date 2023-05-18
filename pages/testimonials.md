---
layout: default
title: Testimonials - Radical College Strategies
permalink: /Testimonials/
---

<section50short> 
  <h2>2023 Results</h2>

  <p style="margin-left: 70px;">Through our <b>unique strategy and approach</b>, we were able to get majority of our Class of 2027 students 
  to <br> Top-5 STEM colleges which were <b>way above their trajectory</b>. Our students are on their way to <b>CMU, <br>UC Berkeley, Cornell, UIUC, UC San Diego, UT honors.</b> Bon Voyage!</p>

  <h2>Meet our Graduates</h2>

  <!--div class="section50left test"> 
    <br> <h3 style="margin:0px;">Jai Singh</h3> <h4 style="margin:0px;">CMU Class of 2027: Computer Engineering</h4>

        <ul class="yes" style="font-size:14px;margin-left:80px">Accepted into:
        
        <li>Carnegie Mellon University</li>
        <li>Cornell University</li>
        <li>UT Austin Honors Program</li>
        </ul>
  </div>

  <div class="section50right test">
  <iframe src="https://www.youtube.com/embed/rM7I2bVjvH4" class="center" scrolling="no" allowfullscreen="" width="450" height="225" frameborder="0" sandbox="allow-forms allow-scripts allow-pointer-lock allow-same-origin allow-top-navigation"></iframe>
  </div>

</section50short> 
<br>
<section50short!--> 
  <div class="section50left test">
  <!--iframe src="https://youtu.be/Ipwl09HyAzY" class="center" scrolling="no" allowfullscreen="" width="450" height="225" frameborder="0" sandbox="allow-forms allow-scripts allow-pointer-lock allow-same-origin allow-top-navigation"></iframe-->

  <iframe src="https://www.youtube.com/embed/Ipwl09HyAzY" width="450" height="260" class="center" scrolling="no" allowfullscreen="" frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"></iframe>

  </div>

  <div class="section50right test">
    <h3 style="margin:0px;">Ria Sethi</h3> <h4 style="margin:0px;">Major: Pediatric Dentistry</h4>

        <ul class="yes" style="font-size:14px;">Accepted into:
        
        <li style="margin-top:10px">UC Berkeley</li>
        <li style="margin-top:10px">University of Washington, Seattle</li>
        <li style="margin-top:10px">University of the Pacific's reputed BS/DDS accelerated program</li>
        </ul>
        <p style="font-size:14px; font-style: italic;">"I thought I would be attending ... community college and transferring" </p> 
        <p style="font-size:14px; font-style: italic;">"Radical took my profile from <b>B level to A+</b>"</p>
  </div>
</section50short> 

<section50short> 
  <div class="section50left test">

    {% for comp in site.testimonials_ca_L %}  
    <h4>{{ comp.from }} </h4>
    {{ comp.content }} 
    {% endfor %}

  </div>

  <div class="section50right test">

    {% for comp in site.testimonials_ca_R %}  
    <h4>{{ comp.from }} </h4>
    {{ comp.content }} 
    {% endfor %}
    
  </div>

</section50short> 

<section50short> 

  <h2>Meet our Mentoring Students</h2>

  <div class="section50left test">

    {% for comp in site.testimonials_hs_L %}  
    <h4>{{ comp.from }} </h4>
    {{ comp.content }} 
    {% endfor %}

  </div>

  <div class="section50right test">

    {% for comp in site.testimonials_hs_R %}  
    <h4>{{ comp.from }} </h4>
    {{ comp.content }} 
    {% endfor %}
    
  </div>

</section50short>

<section50short> 
    {%- include buttons.html -%}
</section50short>

{%- include footer.html -%}
