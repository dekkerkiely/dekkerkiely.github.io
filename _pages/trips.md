---
layout: splash
title: "Trips"
permalink: /trips/
author_profile: false
header:
  overlay_image: /assets/IMG_6364.png  # Replace with your actual hero image
  overlay_filter: "0.3"
  caption: "Trip Reports"
search: true
---

<!-- Search bar -->
<div style="text-align:center; margin-bottom: 2em;">
  <input type="text" id="tripSearch" onkeyup="filterTrips()" placeholder="Search trips..." style="padding: 0.5em; width: 60%; font-size: 1.1em;">
</div>

<!-- Trip Cards -->
<div id="tripList" style="display: flex; flex-wrap: wrap; gap: 2em; justify-content: center;">

  <!-- Trip 1 -->
  <div class="trip-card" style="max-width: 300px;">
    <img src="/assets/images/elchalten.jpg" alt="El Chaltén" style="width:100%; height:auto;">
    <h4 style="margin: 0.5em 0 0 0;">December 2024 to February 2025</h4>
    <h2 style="margin: 0;">El Chaltén ’24/’25</h2>
    <p>I left El Chaltén in 2022 knowing that I would not be back the following year...<br><a href="/trips/el-chalten-2025/">Read More</a></p>
  </div>

  <!-- Trip 2 -->
  <div class="trip-card" style="max-width: 300px;">
    <img src="/assets/images/cerro-torre.jpg" alt="Cerro Torre" style="width:100%; height:auto;">
    <h4 style="margin: 0.5em 0 0 0;">December 2024</h4>
    <h2 style="margin: 0;">Southeast Ridge of Cerro Torre</h2>
    <p>I first heard about the Southeast Ridge back in 2017 after hearing Hayden Kennedy’s iconic Enormocast interview...<br><a href="/trips/cerro-torre/">Read More</a></p>
  </div>

  <!-- Trip 3 -->
  <div class="trip-card" style="max-width: 300px;">
    <img src="/assets/images/yosemite.jpg" alt="Yosemite" style="width:100%; height:auto;">
    <h4 style="margin: 0.5em 0 0 0;">October 2023</h4>
    <h2 style="margin: 0;">The Yosemite Triple Crown</h2>
    <p>The Yosemite Triple Crown links the 3 most prominent big walls in the valley...<br><a href="/trips/yosemite-triple-crown/">Read More</a></p>
  </div>

</div>

<script>
function filterTrips() {
  const input = document.getElementById("tripSearch");
  const filter = input.value.toLowerCase();
  const cards = document.getElementsByClassName("trip-card");
  for (let i = 0; i < cards.length; i++) {
    const card = cards[i];
    card.style.display = card.textContent.toLowerCase().includes(filter) ? "block" : "none";
  }
}
</script>
