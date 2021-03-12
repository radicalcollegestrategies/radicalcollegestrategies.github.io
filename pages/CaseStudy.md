---
layout: default
permalink: /CaseStudy/
---

<section50short>
<h3>For 8th-11th grade students:</h3>
<h1 style="font-size: 36px;">How do you stand out among your peers by <br>building a strong cohesive resume for top colleges<br> without an insane workload?</h1>
</section50short>

<sectionpd>
  <img class="sectionpdPicture sectionpdLeft" src="/images/goal.png" alt="MountainTop">
  <div class="sectionpdContent sectionpdRight">
    <ul class="yes" style="line-height: 3;">This video reveals:
    
    <li>Why you need to plan your academics and activities early on</li>
    <li>How doing too many things actually hurts your chances</li>
    <li>A simple proven system to excel and get colleges to notice you</li>
    </ul>

    <br>

    <button class="mybutton" style="color:white;" onclick="showPopup()">
    <!-- onclick="openForm() -->
    Begin your journey now
    </button>

    <div class="popup">
        <div class="blocker" onclick="hidePopup()"></div>
        <div class="contents" id="myForm">

        <!-- div class="form-popup" id="myForm"-->
        <!--span onclick="closeForm()" class="close-button topright">&times;</span-->
        <span onclick="hidePopup()" class="close-button topright">&times;</span>

        <!-- TODO: clicks outside container inside popup cause problems -->
        <form action="/action_page.php" class="form-container">
        <h2>Enter your email <br> to begin your journey</h2>

        <form action="https://getform.io/f/6f25ddc3-5307-452d-9aae-b330200ba1d5" method="POST">
            <label for="email"></label>
            <input type="text" placeholder="Enter Email" name="email" required>
            <button class="mybutton" style="color:white;" type="submit" class="mybutton">Begin your journey now</button>
            <!--button type="submit" style="font-family:'ABeeZee'; font-weight:'bold'; font-size:16px">Submit</button-->
        </form>
        </form>
        </div>
    </div>
  </div>
</sectionpd>

<script>
// Get the modal
var modal = document.getElementById('myForm');

// When the user clicks anywhere outside of the modal, close it
window.onclick = function(event) {
  if (event.target == modal) {
    modal.style.display = "none";
  }
}

function openForm() {
  document.getElementById("myForm").style.display = "block";
}

function closeForm() {
  document.getElementById("myForm").style.display = "none";
}
// NEW CODE
const popup = document.querySelector('.popup');
function showPopup() {
  popup.classList.add('open');
}
function hidePopup() {
  popup.classList.remove('open');
}
</script>
