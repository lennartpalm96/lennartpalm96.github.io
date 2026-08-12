---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
- /about/
- /about.html
---

Welcome to my page! I am a PhD candidate in economics at the University of Duisburg-Essen and the [Doctoral Research Training Group on Regional Disparities & Economic Policy](https://www.regional-disparities.de).

My research lies in urban and regional economics, with a particular focus on place-based policies and regional development in South Korea. In my work, I combine spatial data analysis and large administrative datasets to study how local policies shape economic outcomes across regions using both reduced form methods and quantitative spatial models.

I hold a Master’s degree in Economics from the Technical University of Dresden and a Bachelor’s degree in Economics from the Georg-August University of Göttingen.

## Selected Figures

<div class="paper-slideshow">

  <div class="slide fade">
    <div class="slide-image">
      <img src="{{ site.baseurl }}/images/maps/Gyeongbu_map(1).png" alt="Gyeongbu HSR line map">
    </div>
    <div class="slide-caption">
      <p>Gyeongbu HSR line — original route (blue) and 2010 extension (red), with treated and excluded districts.</p>
      <p class="slide-paper">From <a href="{{ site.baseurl }}/papers/#design-based">The Heterogeneous Effects of Highspeed-Rail Access on Establishment Performance</a> (with Jaewon Jung)</p>
    </div>
  </div>

  <div class="slide fade">
    <div class="slide-image">
      <img src="{{ site.baseurl }}/images/maps/Overview.png" alt="Innovation City and Enterprise City locations">
    </div>
    <div class="slide-caption">
      <p>Korea's New Town programs: Innovation Cities, Enterprise Cities, and Sejong, relative to the Seoul Metropolitan Area.</p>
      <p class="slide-paper">From <a href="{{ site.baseurl }}/papers/#tasks">Moving Government, Moving People? Public Sector Relocation as a Place-Based Policy</a></p>
    </div>
  </div>

  <div class="slide fade">
    <div class="slide-image">
      <img src="{{ site.baseurl }}/images/maps/IC_2x2_panel.png" alt="Innovation City before and after construction">
    </div>
    <div class="slide-caption">
      <p>Before/after satellite imagery of Innovation Cities Wonju and Busan.</p>
      <p class="slide-paper">From <a href="{{ site.baseurl }}/papers/#tasks">Moving Government, Moving People? Public Sector Relocation as a Place-Based Policy</a></p>
    </div>
  </div>

  <div class="slide fade">
    <div class="slide-image">
      <a href="https://claude.ai/public/artifacts/ba265c2e-f117-4f06-9682-48564aa8224c" target="_blank" rel="noopener">
        <img src="{{ site.baseurl }}/images/maps/1786517842733_image.png" alt="Interactive spatial equilibrium model diagram">
      </a>
    </div>
    <div class="slide-caption">
      <p class="slide-paper">The model from my third paper, <a href="{{ site.baseurl }}/papers/#tasks">Moving Government, Moving People? Public Sector Relocation as a Place-Based Policy</a> — <a href="https://claude.ai/public/artifacts/ba265c2e-f117-4f06-9682-48564aa8224c" target="_blank" rel="noopener">open the interactive model (WIP)</a></p>
    </div>
  </div>

  <a class="slide-prev" onclick="plusSlide(-1)">&#10094;</a>
  <a class="slide-next" onclick="plusSlide(1)">&#10095;</a>

  <div class="slide-dots">
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
    <span class="dot" onclick="currentSlide(4)"></span>
  </div>

</div>

<style>
.paper-slideshow {
  position: relative;
  max-width: 380px;
  margin: 30px auto;
}
.paper-slideshow .slide {
  display: none;
}
.paper-slideshow .slide-image {
  height: 320px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 4px;
  overflow: hidden;
  box-sizing: border-box;
}
.paper-slideshow .slide-image a {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}
.paper-slideshow .slide-image img {
  max-width: 100%;
  max-height: 100%;
  width: auto;
  height: auto;
  display: block;
}
.paper-slideshow .slide-caption {
  padding: 10px 4px 0 4px;
}
.paper-slideshow .slide-caption p {
  font-size: 0.85em;
  color: #666;
  margin: 4px 0;
  text-align: center;
}
.paper-slideshow .slide-paper {
  font-style: italic;
}
.paper-slideshow .slide-prev,
.paper-slideshow .slide-next {
  cursor: pointer;
  position: absolute;
  top: 150px;
  padding: 8px;
  color: #333;
  font-weight: bold;
  font-size: 20px;
  user-select: none;
  background: rgba(255,255,255,0.75);
  border-radius: 50%;
  z-index: 2;
}
.paper-slideshow .slide-prev { left: -10px; }
.paper-slideshow .slide-next { right: -10px; }
.paper-slideshow .slide-prev:hover,
.paper-slideshow .slide-next:hover {
  background: rgba(0,0,0,0.1);
}
.paper-slideshow .slide-dots {
  text-align: center;
  padding-top: 10px;
}
.paper-slideshow .dot {
  cursor: pointer;
  height: 8px;
  width: 8px;
  margin: 0 4px;
  background-color: #ccc;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.3s ease;
}
.paper-slideshow .dot.active {
  background-color: #555;
}
</style>

<script>
var slideIdx = 1;
showSlideNum(slideIdx);

function plusSlide(n) {
  showSlideNum(slideIdx += n);
}
function currentSlide(n) {
  showSlideNum(slideIdx = n);
}
function showSlideNum(n) {
  var slides = document.getElementsByClassName("slide");
  var dots = document.getElementsByClassName("dot");
  if (n > slides.length) { slideIdx = 1; }
  if (n < 1) { slideIdx = slides.length; }
  for (var i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  for (var i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIdx-1].style.display = "block";
  dots[slideIdx-1].className += " active";
}
</script>
