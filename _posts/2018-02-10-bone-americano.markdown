---
layout: post
title: "Boné Americano"
date: 2018-02-07 22:42:00 -0200
categories: bonés
permalink: /bone-americano/
image: '/assets/img/thumbnail/bone-americano.jpeg'
---
<div style="max-width:100%">
  <img class="mySlides" src="{{ '/assets/img/produtos/bone-americano/bone-americano.jpeg'
  | prepend: site.baseurl }}" style="width:60%">
  <img class="mySlides" src="{{ '/assets/img/produtos/bone-americano/bone-americano-1.jpeg'
  | prepend: site.baseurl }}" style="width:60%">
  <img class="mySlides" src="{{ '/assets/img/produtos/bone-americano/bone-americano-2.jpeg'
  | prepend: site.baseurl }}" style="width:60%">

  <img class="demo opacity hover-opacity-off img-galeria"
  src="{{ '/assets/img/produtos/bone-americano/bone-americano.jpeg'
  | prepend: site.baseurl }}" onclick="currentDiv(1)">
  <img class="demo opacity hover-opacity-off img-galeria"
  src="{{ '/assets/img/produtos/bone-americano/bone-americano-1.jpeg'
  | prepend: site.baseurl }}" onclick="currentDiv(2)">
  <img class="demo opacity hover-opacity-off img-galeria"
  src="{{ '/assets/img/produtos/bone-americano/bone-americano-2.jpeg'
  | prepend: site.baseurl }}" onclick="currentDiv(3)">
</div>

<script>
var slideIndex = 1;
showDivs(slideIndex);

function plusDivs(n) {
  showDivs(slideIndex += n);
}

function currentDiv(n) {
  showDivs(slideIndex = n);
}

function showDivs(n) {
  var i;
  var x = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  if (n > x.length) {slideIndex = 1}
  if (n < 1) {slideIndex = x.length}
  for (i = 0; i < x.length; i++) {
     x[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
     dots[i].className = dots[i].className.replace(" opacity-off", "");
  }
  x[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " opacity-off";
}
</script>
