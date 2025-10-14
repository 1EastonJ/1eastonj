---
layout: page
title: "Journey"
permalink: /journey/
---

# 🌍 Journey

> “Collect moments, not things.”  
> Snapshots from places that changed how I think, breathe, and see the world.

<style>
.gallery-section {
  max-width: 1200px;
  margin: 0 auto 60px auto;
  padding: 0 10px;
  animation: fadeIn 1s ease-in-out;
}

h2 {
  text-align: left;
  margin: 40px 0 20px 0;
  font-size: 1.5em;
  border-left: 4px solid #007acc;
  padding-left: 10px;
}

.masonry {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 15px;
}

.masonry-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  animation: slideUp 0.8s ease-in-out both;
}

.masonry-item img {
  width: 100%;
  border-radius: 12px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  opacity: 0;
  animation: fadeInImage 1s ease forwards;
}

.masonry-item img:hover {
  transform: scale(1.03);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.25);
}

.caption {
  text-align: center;
  color: #666;
  font-style: italic;
  font-size: 0.9em;
  margin-top: 6px;
}

@media (max-width: 900px) {
  .masonry {
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  }
}

@media (max-width: 600px) {
  .masonry {
    grid-template-columns: 1fr;
  }
}

/* Fade-in & slide-up animations */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes slideUp {
  from { opacity: 0; transform: translateY(25px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeInImage {
  to { opacity: 1; }
}
</style>

---

<div class="gallery-section">
  <h2>🇺🇸 Madison, USA</h2>
  <div class="masonry">
    <div class="masonry-item">
      <img src="../travel/1.png" alt="Madison 1">
      <div class="caption">Madison — Lake Monona’s quiet glow.</div>
    </div>
    <div class="masonry-item">
      <img src="../travel/2.png" alt="Madison 2">
      <div class="caption">Madison — Where the wind smells like water.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇺🇸 California, USA</h2>
  <div class="masonry">
    <div class="masonry-item">
      <img src="../travel/3.png" alt="California">
      <div class="caption">California — The golden haze that never ends.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇭🇰 Hong Kong</h2>
  <div class="masonry">
    <div class="masonry-item">
      <img src="../travel/4.png" alt="Hong Kong 1">
      <div class="caption">Hong Kong — Hills meet glass and sea.</div>
    </div>
    <div class="masonry-item">
      <img src="../travel/5.png" alt="Hong Kong 2">
      <div class="caption">Hong Kong — Neon, rain, and endless motion.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇪🇬 Egypt</h2>
  <div class="masonry">
    <div class="masonry-item">
      <img src="../travel/6.png" alt="Egypt">
      <div class="caption">Egypt — Sand remembers better than people do.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇨🇦 Canada</h2>
  <div class="masonry">
    <div class="masonry-item"><img src="../travel/7.png"></div>
    <div class="masonry-item"><img src="../travel/8.png"></div>
    <div class="masonry-item"><img src="../travel/9.png"></div>
    <div class="masonry-item"><img src="../travel/10.png"></div>
    <div class="masonry-item"><img src="../travel/11.png"></div>
    <div class="masonry-item"><img src="../travel/12.png"></div>
    <div class="masonry-item"><img src="../travel/13.png"></div>
  </div>
  <div class="caption">Canada — Silence that hums like music.</div>
</div>

<div class="gallery-section">
  <h2>🇨🇳 Harbin, China</h2>
  <div class="masonry">
    <div class="masonry-item"><img src="../travel/14.png"></div>
    <div class="masonry-item"><img src="../travel/15.png"></div>
    <div class="masonry-item"><img src="../travel/16.png"></div>
  </div>
  <div class="caption">Harbin — Frozen light, warm laughter.</div>
</div>
