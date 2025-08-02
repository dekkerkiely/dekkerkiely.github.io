---
layout: splash
title: "Trips"
permalink: /trips/
author_profile: false
header:
  overlay_image: /assets/IMG_6364.png  # Replace with your actual hero image
  overlay_filter: "0.3"
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
    <img src="/assets/images/elchalten.jpg" alt="Italy" style="width:100%; height:auto;">
    <h2 style="margin: 0;">Bikepacking Lake Garda</h2>
    <h4 style="margin: 0.5em 0 0 0;">August 2023</h4>
    <p>I left my bag at the nicest hotel i could find..<br><a href="/trips/el-chalten-2025/">Read More</a></p>
  </div>

  <!-- Trip 2 -->
  <div class="trip-card" style="max-width: 300px;">
    <img src="/assets/images/cerro-torre.jpg" alt="Rumney" style="width:100%; height:auto;">
    <h4 style="margin: 0.5em 0 0 0;">August 2023</h4>
    <h2 style="margin: 0;">A week in Chamonix</h2>
    <p>I heard about chamonix through my sister, who vistied this tourist destination with her exchange partner/ longtime friend Lison. I saw pictures and videos everywhere of people climbing these sharp snowy peaks...<br><a href="/trips/cerro-torre/">Read More</a></p>
  </div>

  <!-- Trip 3 -->
  <div class="trip-card" style="max-width: 300px;">
    <img src="/assets/images/yosemite.jpg" alt="Yosemite" style="width:100%; height:auto;">
    <h4 style="margin: 0.5em 0 0 0;">August 2022</h4>
    <h2 style="margin: 0;">Road Trip Across Midwest</h2>
    <p>I need to be back at school the 5th of september with 21 days to burn...<br><a href="/trips/yosemite-triple-crown/">Read More</a></p>
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
