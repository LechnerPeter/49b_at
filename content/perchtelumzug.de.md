+++
title = 'Perchtelumzug'
date = 2026-06-28T00:00:00+02:00
draft = false
image = '/images/perchtelumzug.png'
+++

<img src="/images/perchtelumzug.png" alt="Angerberger Perchtelumzug" style="max-width: 260px; float: right; margin: 0 0 1.5rem 2rem; border-radius: 10px; box-shadow: 0 4px 16px rgba(0,0,0,0.4);">

## Pertelumzug Angerberg

Alljährlich findet in Angerberg der Perchtelumzug statt, seit 2024 wird er von der Landjugend veranstaltet.

## Die Passen

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

## Was gibt es bei uns

- Perchteln
- Kinder Perchtln
- Nikolaus mit Überraschung für die Kleinen
- Essen und Getränke
- Winterliche musikalische Umrahmung

## Bilder

<div class="photo-gallery" style="display:grid;grid-template-columns:repeat(3,1fr);gap:0.75rem;margin:1rem 0;">
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

## Was gibt es bei uns nicht

- Feuer
- Rauch
- Gewalt

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
