---
layout: default
permalink: /Works3/
---
<!-- Work in progress. Try this again:
https://medium.com/@dmccoy/how-to-submit-an-html-form-to-google-sheets-without-google-forms-b833952cc175 -->
<sectionpd>
<h3>For 8th-11th grade students:</h3>
<h1 style="font-size: 36px;">How do you stand out among your peers by <br>building a strong cohesive resume for top colleges<br> without an insane workload?</h1>

  <img class="sectionpdPicture sectionpdLeft" src="/images/goal.png" alt="MountainTop">
  <div class="sectionpdContent sectionpdRight">
    <ul class="yes" style="line-height: 3;">This video reveals:
    
    <li>Why you need to plan your academics and activities early on</li>
    <li>How doing too many things actually hurts your chances</li>
    <li>A simple proven system to excel and get colleges to notice you</li>
    </ul>

    <br>

    <button class="mybutton" style="color:white;" onclick="showPopup()">
    Begin your journey now
    </button>

    <div class="popup">
        <div class="blocker" onclick="hidePopup()"></div>
        <div class="contents">

        <span onclick="hidePopup()" class="close-button topright">&times;</span>

        <form action="/Video/" onsubmit="dosomething(this)" class="form-container" id="myForm">
            <h2>Enter your email <br> to begin your journey</h2>

            <label for="email"></label>
            <input type="text" placeholder="Enter Email" name="email" required>
            <button class="mybutton" style="color:white;" type="submit" class="mybutton">Begin your journey now</button>
        </form>
        </div>
    </div>
  </div>
</sectionpd>

<script>
const popup = document.querySelector('.popup');
function showPopup() {
  popup.classList.add('open');
}
function hidePopup() {
  popup.classList.remove('open');
}

const form1 = document.forms['myForm']
const url = 'https://script.google.com/macros/s/AKfycbxqG2lS_HAa1swJ31Xl3F912tJXzk26s0ASB5pwA2IikNo-ojSIF1hC74n88MUHPiZ8/exec'
var form2 = document.getElementById("myForm")

function dosomething(theform) {
  //alert("GEETA:\n" + form1);

  var jqxhr = $.ajax({
    url: url,
    method: "GET",
    dataType: "json",
    data: form.serializeObject()
  })

  document.getElementById("myForm").reset(); 
}
</script>