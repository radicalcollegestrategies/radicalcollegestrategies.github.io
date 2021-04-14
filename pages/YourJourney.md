---
layout: default
permalink: /YourJourney/
---
<sectionpd>
<h4 style="margin:10px;">8th-11th grade U.S. students in STEM:</h4>
<h2 style="margin-top:15px;margin-bottom:0px;color:black">3 ways <div style="display:inline;font-family:Courier New;font-size:44px;"><b>I</b></div> help students gain strategic advantage<br>to get into top-tier colleges</h2> 
<h3 style="margin-top:5px;color:black">without an insane workload</h3>

  <!-- src="/images/VideoIntro.png"  -->
  <img class="sectionpdPicture sectionpdLeft myimg" style="width: 400px;" 
   src="/images/StandOut.png" alt="IntroVideo" onclick="showPopup()">
  <div class="sectionpdContent sectionpdRight">
    <ul class="yes"><h3>In this short video you will learn:</h3>
    
    <li style="margin-bottom:20px">A model that clearly defines where to invest your time 'n effort</li>
    <li style="margin-bottom:20px">Differentiate yourself by focusing on impactful activities</li>
    <li>A proven strategy to get into MIT and other top-tier colleges</li>
    </ul>

    <br>

    <p style="text-align:center;">
    <button class="mybutton" style="color:white;" onclick="showPopup()">
    Get The Video
    </button>
    </p>

    <div class="popup">
        <div class="blocker" onclick="hidePopup()"></div>
        <div class="contents">

        <span onclick="hidePopup()" class="close-button topright">&times;</span>

        <form id="myForm" class="form-container" action="/Session/">
            <h3>Yes, Send Me the Free Video Now!</h3>

            <label for="email"></label>
            <input style="max-width:270px;margin-left:45px;" type="text" placeholder="Enter Email" name="email" required>
            <p style="font-size:12px;text-align: center;">We do not sell or share your info</p>
            <p style="text-align:center;">
            <button class="mybutton" style="color:white;" type="submit" class="mybutton">Send Me The Video</button>
            </p>
        </form>
        </div>
    </div>

    <div class="popup2">
        <div class="contents">
        <form id="myForm2" class="form-container">

          <p><h3>Thank You!</h3></p>
          <button class="mybutton" style="color:white;" type="submit" class="mybutton">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Submitting...&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</button>
        </form>
        </div>
    </div>

  </div>
</sectionpd>

<sectionpd id="other">
<h3 style="margin:10px;">All other students:</h3>
<p style="text-align:center">If you are in grades 7 or below, or a college student looking for some guidance:<br><a href="https://koalendar.com/e/radicalcollegestrategies" style="color:#0821af;">Book a free session here</a> to discuss your specific situation, and check out <a href="https://stemscholars.github.io" target="_blank" style="color: #0821af;">STEM Scholars</a> for high quality STEM activities.</p>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
</sectionpd>

<script>
const popup = document.querySelector('.popup');
const popup2 = document.querySelector('.popup2');

function showPopup() {
  popup.classList.add('open');
}
function hidePopup() {
  popup.classList.remove('open');
}

function showPopup2() {
  popup2.classList.add('open');
}

<!-- Google form:
https://medium.com/@dmccoy/how-to-submit-an-html-form-to-google-sheets-without-google-forms-b833952cc175 -->

var $form = $('form#myForm')
const url = 'https://script.google.com/macros/s/AKfycbxqG2lS_HAa1swJ31Xl3F912tJXzk26s0ASB5pwA2IikNo-ojSIF1hC74n88MUHPiZ8/exec'

$("#myForm").submit (function() { 
  showPopup2();
  $.ajax({
    url: url,
    method: "GET",
    dataType: "json",
    data: $form.serializeJSON(),
    async:false
  });
  
  /* .done(alert("Thank you!\n")); */

  document.getElementById("myForm").reset(); 
});

</script>

<div class="license" style="float:right">
<a href="/Privacy" target="_blank" style="color: #0821af;">Privacy Policy</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Terms" target="_blank" style="color: #0821af;">Terms</a>
<br>
<br>
</div>
