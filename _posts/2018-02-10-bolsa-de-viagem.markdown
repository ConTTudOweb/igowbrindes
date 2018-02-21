---
layout: post
title: "Bolsa de Viagem"
date: 2018-02-07 22:42:00 -0200
categories: bolsas
permalink: /bolsa-de-viagem/
image: {{ '/assets/img/thumbnail/bolsa-de-viagem.jpeg' | prepend: site.baseurl }}
---
<div style="max-width:100%">
  <img class="mySlides" src="{{ '/assets/img/produtos/bolsa-de-viagem/bolsa-de-viagem.jpeg'
  | prepend: site.baseurl }}" style="width:60%">

  <img class="demo opacity hover-opacity-off img-galeria"
  src="{{ '/assets/img/produtos/bolsa-de-viagem/bolsa-de-viagem.jpeg'
  | prepend: site.baseurl }}" onclick="currentDiv(1)">
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
