+++
title = 'Perchten Procession'
date = 2026-06-28T00:00:00+02:00
draft = false
image = '/images/perchtelumzug.png'
+++

## Perchten Procession Angerberg

<details class="passen-details">
<summary>What is Perchteln?</summary>

The Perchteln tradition in Angerberg is an old Tyrolean custom. Groups known as Perchten- or Peaschtl-Passen march through the village wearing hand-carved wooden masks, heavy costumes, cowbells and drums. With their noise and presence they are meant to drive away evil winter spirits and bring luck, health and a good harvest for the coming year. In Angerberg this custom has remained particularly traditional: alongside the Perchten and St. Nicholas procession at the village square, going from house to house is also part of the community. The Perchteln is therefore not just a spooky spectacle, but an important part of regional culture and identity.

</details>

Every year the Perchten procession takes place in Angerberg. Since 2024 it has been organized by the Landjugend (rural youth association).

<details class="passen-details">
<summary>The Groups</summary>

- Angerberger Gruab Pass
- Rambazamba Pass
- Unterboch Pass
- Ochleit Pass
- Toina Pass
- Lindna Pass
- Feuerwehr Pass
- Brand Pass
- Melcham Pass
- Moosanger Pass
- Auer Pass
- Felderer Pass
- Promill Pass
- Fok'n Pass
- Foastnheisl Pass

</details>

<div class="comparison">
  <div class="comparison-col comparison-yes">
    <h3>What we offer</h3>
    <ul>
      <li>Perchten</li>
      <li>Children's Perchten</li>
      <li>St. Nicholas with a surprise for the little ones</li>
      <li>Food and drinks</li>
      <li>Wintery musical entertainment</li>
    </ul>
  </div>
  <div class="comparison-col comparison-no">
    <h3>What we don't offer</h3>
    <ul>
      <li>Fire</li>
      <li>Smoke</li>
      <li>Violence</li>
    </ul>
  </div>
</div>

## Photos

<div class="photo-gallery" style="display:grid;grid-template-columns:repeat(3,1fr);gap:0.75rem;margin:1rem 0;">
<img src="/images/perchtelumzug.png" alt="Angerberger Perchtelumzug" style="width:100%;aspect-ratio:4/3;object-fit:cover;object-position:top;border-radius:8px;">
<img src="/images/perchteln/DSC02163.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02204.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02227.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02262.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02326.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02350.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02374.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02380.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02422.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02452.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02503.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02533.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02577.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/DSC02592.JPG" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
<img src="/images/perchteln/IMG_4023.jpeg" alt="Perchten" style="width:100%;aspect-ratio:4/3;object-fit:cover;border-radius:8px;">
</div>


<div id="lightbox">
  <button id="lb-prev">&#8249;</button>
  <img src="" alt="Perchten">
  <button id="lb-next">&#8250;</button>
</div>
<script>
(function(){
  const imgs = Array.from(document.querySelectorAll('.photo-gallery img'));
  const lb = document.getElementById('lightbox');
  const lbImg = lb.querySelector('img');
  let current = 0;
  function show(idx) {
    current = (idx + imgs.length) % imgs.length;
    lbImg.src = imgs[current].src;
    lb.classList.add('active');
  }
  imgs.forEach((img, i) => img.addEventListener('click', () => show(i)));
  lb.addEventListener('click', () => lb.classList.remove('active'));
  document.getElementById('lb-prev').addEventListener('click', e => { e.stopPropagation(); show(current - 1); });
  document.getElementById('lb-next').addEventListener('click', e => { e.stopPropagation(); show(current + 1); });
  document.addEventListener('keydown', e => {
    if (!lb.classList.contains('active')) return;
    if (e.key === 'Escape') lb.classList.remove('active');
    if (e.key === 'ArrowLeft') show(current - 1);
    if (e.key === 'ArrowRight') show(current + 1);
  });
})();
</script>
