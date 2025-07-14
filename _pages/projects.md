---
layout: splash
title: "Projects"
permalink: /projects/
author_profile: false
header:
  overlay_image: /assets/513c165751eef94f8c951c082a7a5213-beige-engineering-background-design.webp  # Replace with your actual hero image
  overlay_filter: "0.3"
  caption: "Engineering Projects"
search: true
---

<!-- Search bar -->
<div style="text-align:center; margin-bottom: 2em;">
  <input type="text" id="projectSearch" onkeyup="filterProjects()" placeholder="Search projects..." style="padding: 0.5em; width: 60%; font-size: 1.1em;">
</div>

<!-- Project Cards -->
<div id="projectList" style="display: flex; flex-wrap: wrap; gap: 2em; justify-content: center;">

  <!-- Project 1 -->
  <div class="project-card" style="max-width: 300px;">
    <img src="/assets/images/wave-generator.jpg" alt="Wave Generator" style="width:100%; height:220px; object-fit: cover;">
    <h4 style="margin: 0.5em 0 0 0;">September 2024- April 2025</h4>
    <h2 style="margin: 0;">Wave Generator for Flume Tank</h2>
    <p>Designed and built a wave generator for environmental testing, using scaled wave theory and Froude similitude...<br><a href="/projects/wave-generator/">Read More</a></p>
  </div>

  <!-- Project 2 -->
  <div class="project-card" style="max-width: 300px;">
    <img src="/assets/images/bas-control.jpg" alt="Design of Airfoil" style="width:100%; height:220px; object-fit: cover;">
    <h4 style="margin: 0.5em 0 0 0;">Spring 2025</h4>
    <h2 style="margin: 0;">Design, build and test a airfoil.</h2>
    <p>Performed life cycle assessment on a BAS control board including energy, emissions, and end-of-life impact...<br><a href="/projects/bas-lca/">Read More</a></p>
  </div>

  <!-- Project 3 -->
  <div class="project-card" style="max-width: 300px;">
    <img src="/assets/images/powder-nozzle.jpg" alt="Powder Delivery Nozzle" style="width:100%; height:220px; object-fit: cover;">
    <h4 style="margin: 0.5em 0 0 0;">Fall 2024</h4>
    <h2 style="margin: 0;">Powder Delivery Nozzle Design</h2>
    <p>Conceptualized and tested different nozzle designs for laser metal deposition, analyzing flow, clogging, and spray angle...<br><a href="/projects/powder-nozzle/">Read More</a></p>
  </div>

</div>

<script>
function filterProjects() {
  const input = document.getElementById("projectSearch");
  const filter = input.value.toLowerCase();
  const cards = document.getElementsByClassName("project-card");
  for (let i = 0; i < cards.length; i++) {
    const card = cards[i];
    card.style.display = card.textContent.toLowerCase().includes(filter) ? "block" : "none";
  }
}
</script>
