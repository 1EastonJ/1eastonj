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
  margin: 0 auto 80px auto;
  padding: 0 10px;
}

h2 {
  text-align: left;
  margin: 40px 0 15px 0;
  font-size: 1.5em;
  border-left: 4px solid #007acc;
  padding-left: 10px;
}

.scroll-gallery {
  display: flex;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  gap: 18px;
  padding-bottom: 20px;
  scrollbar-width: thin;
  scroll-behavior: smooth;
  perspective: 1000px;
}

.scroll-gallery::-webkit-scrollbar {
  height: 8px;
}
.scroll-gallery::-webkit-scrollbar-thumb {
  background: #bbb;
  border-radius: 4px;
}
.scroll-gallery::-webkit-scrollbar-thumb:hover {
  background: #999;
}

.scroll-item {
  flex: 0 0 auto;
  width: 360px;
  scroll-snap-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: transform 0.4s ease, opacity 0.4s ease;
  opacity: 0.9;
}

.scroll-item img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: 14px;
  box-shadow: 0 6px 18px rgba(0,0,0,0.15);
  transition: transform 0.4s ease, box-shadow 0.4s ease, opacity 0.4s ease;
}

.scroll-item.active img {
  transform: scale(1.07);
  box-shadow: 0 8px 25px rgba(0,0,0,0.25);
  opacity: 1;
}

.caption {
  text-align: center;
  color: #666;
  font-style: italic;
  font-size: 0.9em;
  margin-top: 6px;
  max-width: 95%;
}

/* Fade-in animation */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
.gallery-section {
  animation: fadeIn 1.2s ease both;
}

@media (max-width: 900px) {
  .scroll-item { width: 300px; }
}

@media (max-width: 600px) {
  .scroll-item { width: 260px; }
}
</style>

<script>
document.addEventListener('DOMContentLoaded', () => {
  const galleries = document.querySelectorAll('.scroll-gallery');
  galleries.forEach(gallery => {
    const items = gallery.querySelectorAll('.scroll-item');
    gallery.addEventListener('scroll', () => {
      const galleryCenter = gallery.scrollLeft + gallery.clientWidth / 2;
      items.forEach(item => {
        const rect = item.getBoundingClientRect();
        const itemCenter = rect.left + rect.width / 2;
        const distance = Math.abs(galleryCenter - (gallery.scrollLeft + itemCenter));
        const scale = Math.max(0.9, 1 - distance / 1000);
        item.style.transform = `scale(${scale})`;
        item.style.opacity = scale;
      });
    });
  });
});
</script>

---

<div class="gallery-section">
  <h2>🇺🇸 Madison, USA</h2>
  <div class="scroll-gallery">
    <div class="scroll-item">
      <img src="../travel/1.png" alt="Madison 1">
      <div class="caption">Madison — Lake Monona’s quiet glow.</div>
    </div>
    <div class="scroll-item">
      <img src="../travel/2.png" alt="Madison 2">
      <div class="caption">Madison — Where the wind smells like water.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇺🇸 California, USA</h2>
  <div class="scroll-gallery">
    <div class="scroll-item">
      <img src="../travel/3.png" alt="California">
      <div class="caption">California — The golden haze that never ends.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇭🇰 Hong Kong</h2>
  <div class="scroll-gallery">
    <div class="scroll-item">
      <img src="../travel/4.png" alt="Hong Kong 1">
      <div class="caption">Hong Kong — Hills meet glass and sea.</div>
    </div>
    <div class="scroll-item">
      <img src="../travel/5.png" alt="Hong Kong 2">
      <div class="caption">Hong Kong — Neon, rain, and endless motion.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇪🇬 Egypt</h2>
  <div class="scroll-gallery">
    <div class="scroll-item">
      <img src="../travel/6.png" alt="Egypt">
      <div class="caption">Egypt — Sand remembers better than people do.</div>
    </div>
  </div>
</div>

<div class="gallery-section">
  <h2>🇨🇦 Canada</h2>
  <div class="scroll-gallery">
    <div class="scroll-item"><img src="../travel/7.png"></div>
    <div class="scroll-item"><img src="../travel/8.png"></div>
    <div class="scroll-item"><img src="../travel/9.png"></div>
    <div class="scroll-item"><img src="../travel/10.png"></div>
    <div class="scroll-item"><img src="../travel/11.png"></div>
    <div class="scroll-item"><img src="../travel/12.png"></div>
    <div class="scroll-item"><img src="../travel/13.png"></div>
  </div>
  <div class="caption">Canada — Silence that hums like music.</div>
</div>

<div class="gallery-section">
  <h2>🇨🇳 Harbin, China</h2>
  <div class="scroll-gallery">
    <div class="scroll-item"><img src="../travel/14.png"></div>
    <div class="scroll-item"><img src="../travel/15.png"></div>
    <div class="scroll-item"><img src="../travel/16.png"></div>
  </div>
  <div class="caption">Harbin — Frozen light, warm laughter.</div>
</div>
