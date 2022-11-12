---
layout: default
permalink: /MiddleSchool/
---
<section50short>
<h3 style="margin:10px;">Hello, Middle School STEM students (U.S. only):</h3>
<div class="license" style="text-align:center;font-size:14px;">
    ( <a style="color:blue" href="/HighSchool">High School Students: Click here</a> )
</div> 

<h2 style="margin-top:15px;margin-bottom:0px;color:black">Do you have clarity on what subjects / major <br> you want to excel in?</h2>
<!--h3 style="margin-top:5px;margin-bottom:0px;color:black">- in High School and beyond</h3-->
</section50short>

<section50>
<div class="section50left">
<h3>Yes! <div style="display:inline;font-family:Courier New;font-size:26px;"><b>I</b></div> have a couple favorite subjects</h3>
    <ul class="yes" style="font-size: 16px;padding-left:10px"><h4 style="text-align:left; padding-left:28px">In this short video you will learn how to:</h4>
    
    <li style="margin-bottom:20px">Differentiate impactful prestigious activities from time-sinks</li>
    <li style="margin-bottom:20px">Gain a head start by narrowing down your interests further</li>
    <li>Differentiate yourself early to maintain the edge in high school</li>
    <li>-----------------------------------------</li>
    <li style="margin-bottom:20px">Deep dive into your interest using prestigious competitions</li>
    <li style="margin-bottom:20px">Gain significant advantage entering High School</li>
    <li style="margin-bottom:20px">Gain an edge over your classmates</li>
    <li style="margin-bottom:20px">Stand out from your classmates through early wins</li>
    </ul>
  <img style="width: 400px;" 
   src="/images/StandOut.png" alt="IntroVideo" onclick="showPopup()">

    <p style="text-align:center;padding-top:20px">
    <button class="mybutton" style="color:white;" onclick="showPopup()">
    Get The Video
    </button>
    </p>

</div>

<div class="section50right">
<h3>Umm... Do <div style="display:inline;font-family:Courier New;font-size:26px;"><b>I</b></div> really need to do that now?</h3>
    <ul class="yes" style="font-size: 16px;padding-left:10px"><h4>In this short video you will learn:</h4>
    
    <li style="margin-bottom:20px">Why it is critical to narrow down your interests before entering high school</li>
    <li style="margin-bottom:20px">Why you need to explore way beyond school curriculum</li>
    <li>How to make your subsequent high school journey more targeted and stress-free</li>
    <li>-----------------------------------------</li>
    <li style="margin-bottom:20px">Why it's important to explore things beyond what's taught in school</li>
    <li style="margin-bottom:20px">How much foundation do school subjects provide and how much does one need to explore oneself</li>
    <li style="margin-bottom:20px">How to explore the different major / career options</li>
    <li style="margin-bottom:20px">How to have a stress-free high school journey with no flundering</li>
    <li style="margin-bottom:20px">How to enter high school with a plan</li>
    </ul>

  <img style="width: 400px;" 
   src="/images/StandOut.png" alt="IntroVideo" onclick="showPopup()">

    <p style="text-align:center;padding-top:20px">
    <button class="mybutton" style="color:white;" onclick="showPopup()">
    Get The Video
    </button>
    </p>

</div>

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

</section50>


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
