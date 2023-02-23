---
layout: default
title: Your Journey - RCS
permalink: /YourJourney/
---
{%- include YourJourneySenior.html -%}

{%- include YourJourneyHigh.html -%}

{%- include YourJourneyMid.html -%}

<script>
const popupMidComp = document.querySelector("#popupMidComp");
const popup2MidComp = document.querySelector("#popup2MidComp");
const popupMidExpl = document.querySelector("#popupMidExpl");
const popup2MidExpl = document.querySelector("#popup2MidExpl");
const popupHigh = document.querySelector("#popupHigh");
const popup2High = document.querySelector("#popup2High");

function showPopupMidComp() {
  popupMidComp.classList.add('open');
}
function hidePopupMidComp() {
  popupMidComp.classList.remove('open');
}

function showPopup2MidComp() {
  popup2MidComp.classList.add('open');
}

function showPopupMidExpl() {
  popupMidExpl.classList.add('open');
}
function hidePopupMidExpl() {
  popupMidExpl.classList.remove('open');
}

function showPopup2MidExpl() {
  popup2MidExpl.classList.add('open');
}

function showPopupHigh() {
  popupHigh.classList.add('open');
}
function hidePopupHigh() {
  popupHigh.classList.remove('open');
}

function showPopup2High() {
  popup2High.classList.add('open');
}

<!-- Google form:
https://medium.com/@dmccoy/how-to-submit-an-html-form-to-google-sheets-without-google-forms-b833952cc175 -->

var $formHigh = $('form#myFormHigh')
var $formMidComp = $('form#myFormMidComp')
var $formMidExpl = $('form#myFormMidExpl')
const url = 'https://script.google.com/macros/s/AKfycbxqG2lS_HAa1swJ31Xl3F912tJXzk26s0ASB5pwA2IikNo-ojSIF1hC74n88MUHPiZ8/exec'

$("#myFormHigh").submit (function() { 
  showPopup2High();
  $.ajax({
    url: url,
    method: "GET",
    dataType: "json",
    data: $formHigh.serializeJSON(),
    async:false
  });
  
  document.getElementById("myFormHigh").reset(); 
});

$("#myFormMidComp").submit (function() { 
  showPopup2MidComp();
  $.ajax({
    url: url,
    method: "GET",
    dataType: "json",
    data: $formMidComp.serializeJSON(),
    async:false
  });
  
  document.getElementById("myFormMidComp").reset(); 
});

$("#myFormMidExpl").submit (function() { 
  showPopup2MidExpl();
  $.ajax({
    url: url,
    method: "GET",
    dataType: "json",
    data: $formMidExpl.serializeJSON(),
    async:false
  });
  
  document.getElementById("myFormMidExpl").reset(); 
});
</script>

{%- include footer.html -%}
