---
layout: archive
title: "Gallery"
permalink: /gallery/
author_profile: true
---

*A curated selection of moments across five years of academic excellence, 
leadership, and service.*

---

<style>
.gallery-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(180px,1fr));gap:10px;margin:20px 0;}
.gallery-grid figure{margin:0;cursor:pointer;overflow:hidden;border-radius:8px;border:0.5px solid #ccc;}
.gallery-grid img{width:100%;height:160px;object-fit:cover;display:block;transition:transform 0.2s;}
.gallery-grid figure:hover img{transform:scale(1.04);}
.gallery-grid figcaption{font-size:11px;color:gray;text-align:center;padding:5px 4px;line-height:1.3;}
.gallery-label{font-size:13px;font-weight:600;text-transform:uppercase;letter-spacing:0.08em;color:gray;margin:28px 0 10px;}
.lb-overlay{display:none;position:fixed;inset:0;background:rgba(0,0,0,0.88);z-index:9999;align-items:center;justify-content:center;cursor:pointer;}
.lb-overlay.open{display:flex;}
.lb-overlay img{max-width:90vw;max-height:85vh;object-fit:contain;border-radius:4px;}
.lb-cap{position:absolute;bottom:20px;left:0;right:0;text-align:center;color:rgba(255,255,255,0.75);font-size:13px;}
.lb-close{position:absolute;top:16px;right:20px;color:white;font-size:24px;cursor:pointer;line-height:1;}
</style>

---

<div class="gallery-label">Academic & Intellectual</div>
<div class="gallery-grid">

  <!-- ADD YOUR PHOTOS HERE -->
  <!-- Suggested: studying photos, Kangaroo Math, chess competition,
       exam results, academic award ceremonies -->

  <figure onclick="openLb(this)">
    <img src="/_pages/photos/YOUR-PHOTO.jpg" alt="Description">
    <figcaption>Caption here</figcaption>
  </figure>

</div>

---

<div class="gallery-label">Recognition & Awards</div>
<div class="gallery-grid">

  <!-- ADD YOUR PHOTOS HERE -->
  <!-- Suggested: Tokoh Jati Diri on stage, Kangaroo Math award,
       Tahfiz khatam ceremony, any formal award moments -->

  <figure onclick="openLb(this)">
    <img src="/_pages/photos/YOUR-PHOTO.jpg" alt="Description">
    <figcaption>Caption here</figcaption>
  </figure>

</div>

---

<div class="gallery-label">Discipline & Uniform</div>
<div class="gallery-grid">

  <!-- ADD YOUR PHOTOS HERE -->
  <!-- Suggested: KRS photos NOT already on Activities page,
       National Day shots, formation march group photos -->

  <figure onclick="openLb(this)">
    <img src="/_pages/photos/YOUR-PHOTO.jpg" alt="Description">
    <figcaption>Caption here</figcaption>
  </figure>

</div>

---

<div class="gallery-label">Sports & Physical</div>
<div class="gallery-grid">

  <!-- ADD YOUR PHOTOS HERE -->
  <!-- Suggested: volleyball photos NOT already on Activities page,
       chess competition, any other sports moments -->

  <figure onclick="openLb(this)">
    <img src="/_pages/photos/YOUR-PHOTO.jpg" alt="Description">
    <figcaption>Caption here</figcaption>
  </figure>

</div>

---

<div class="gallery-label">Community & Service</div>
<div class="gallery-grid">

  <!-- ADD YOUR PHOTOS HERE -->
  <!-- Suggested: facilitator programme, Palestine rally,
       engineering course, community moments -->

  <figure onclick="openLb(this)">
    <img src="/_pages/photos/YOUR-PHOTO.jpg" alt="Description">
    <figcaption>Caption here</figcaption>
  </figure>

</div>

---

<div class="gallery-label">Candid & Character</div>
<div class="gallery-grid">

  <!-- ADD YOUR PHOTOS HERE -->
  <!-- Suggested: genuine unposed moments, friendships,
       everyday school life, personality shots -->

  <figure onclick="openLb(this)">
    <img src="/_pages/photos/YOUR-PHOTO.jpg" alt="Description">
    <figcaption>Caption here</figcaption>
  </figure>

</div>

<div class="lb-overlay" id="lb" onclick="closeLb()">
  <span class="lb-close" onclick="closeLb()">&#x2715;</span>
  <img id="lb-img" src="" alt="">
  <p class="lb-cap" id="lb-cap"></p>
</div>

<script>
function openLb(fig){
  document.getElementById('lb-img').src=fig.querySelector('img').src;
  document.getElementById('lb-cap').textContent=fig.querySelector('figcaption').textContent;
  document.getElementById('lb').classList.add('open');
  document.body.style.overflow='hidden';
}
function closeLb(){
  document.getElementById('lb').classList.remove('open');
  document.body.style.overflow='';
}
document.addEventListener('keydown',function(e){if(e.key==='Escape')closeLb();});
</script>
