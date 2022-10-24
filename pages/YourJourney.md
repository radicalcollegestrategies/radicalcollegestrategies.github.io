---
layout: default
permalink: /YourJourney/
---
<sectionpd>
<h3 style="margin:10px;">Grades 8-11 STEM students (U.S. only):</h3>
<h2 style="margin-top:15px;margin-bottom:0px;color:black">3 ways <div style="display:inline;font-family:Courier New;font-size:44px;"><b>I</b></div> help students gain strategic advantage<br>to get into top-tier colleges</h2> 
<h3 style="margin-top:5px;color:black">without an insane workload</h3>

  <!-- src="/images/VideoIntro.png"  -->
  <img class="sectionpdPicture sectionpdLeft myimg" style="width: 400px;" 
   src="/images/StandOut.png" alt="IntroVideo" onclick="showPopup()">
  <div class="sectionpdContent sectionpdRight">
    <ul class="yes"><h3>In this short video you will learn:</h3>
    
    <li style="margin-bottom:20px">A model that clearly defines where to invest your time 'n effort</li>
    <li style="margin-bottom:20px">Differentiate yourself by focusing on a few impactful activities</li>
    <li>A proven strategy to get into MIT and other top-tier colleges</li>
    </ul>

    <p style="margin-left:40px;color:red">Sorry, there are currently no slots available for new students. <br> Please check back in December 2022.</p>

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
<h3>Middle School</h3>
<p> If your middle schooler falls in one of the following categories, please <a href="https://calendly.com/geeta-radical/middle-school"  target="_blank" style="color:#0821af;">book a free session here</a>:
    <ul>
    <li>Students looking to gain clarity on what to major in. I help them explore activities in different areas so they can identify their major before they enter high school.</li>
    <li>Students looking to gain an early advantage in USA Computing Olympiad, math competitions, science fair and other national STEM events</li>
    </ul>

Others, please <b>contact me in the spring of 8th grade</b> to turbocharge your high school experience!</p>

<h3>Seniors (College Applications)</h3>
<p>For college applications, I exclusively help students who have been working with me over the years. I typically don't take on rising seniors as new students, but if you have a very strong STEM profile, please <a href="https://docs.google.com/spreadsheets/d/1U_qaVM32ebqJxPkqoVopKzgctz7m_cgjuawbRcKJ5Zw/edit#gid=1398217924" target="_blank" style="color:#0821af;">fill out this spreadsheet</a>, and I'll see what I can do.</p>
<p style="text-align:center">(Grades 8-11: Watch the video on the top of this page to book a session)</p>

<!--p style="text-align:center;font-size:18px;"><b>Rising seniors:</b> (late Grade 11-early Grade 12): <a href="https://calendly.com/geeta-radical/college-counseling" style="color:#0821af;">Book a free session here</a> for help with college admissions.</p>
<p style="text-align:center">(Grades 8-11: Watch the video above to book a session)</p-->

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
