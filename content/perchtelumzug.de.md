+++
title = 'Perchtelumzug'
date = 2026-06-28T00:00:00+02:00
draft = false
image = '/images/perchtelumzug.png'
+++

## Pertelumzug Angerberg

<details class="passen-details">
<summary>Was ist Perchteln?</summary>

Das Perchtln in Angerberg ist ein alter Tiroler Brauch. Dabei ziehen sogenannte Perchten- oder Peaschtl-Passen mit geschnitzten Holzmasken, schweren Kostümen, Schellen und Trommeln durch den Ort. Mit ihrem Lärm und Auftreten sollen sie böse Wintergeister vertreiben und Glück, Gesundheit sowie eine gute Ernte für das kommende Jahr bringen. In Angerberg ist dieser Brauch besonders traditionell geblieben: Neben dem Perchten- und Nikolauseinzug am Dorfplatz gehört auch das Ziehen von Haus zu Haus zur Dorfgemeinschaft. Das Perchtln ist daher nicht nur ein schauriges Schauspiel, sondern ein wichtiger Teil der regionalen Kultur und Identität.

</details>

Alljährlich findet in Angerberg der Perchtelumzug statt, seit 2024 wird er von der Landjugend veranstaltet.

<details class="passen-details">
<summary>Die Passen</summary>

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
    <h3>Was gibt es bei uns</h3>
    <ul>
      <li>Perchteln</li>
      <li>Kinder Perchtln</li>
      <li>Nikolaus mit Überraschung für die Kleinen</li>
      <li>Essen und Getränke</li>
      <li>Winterliche musikalische Umrahmung</li>
    </ul>
  </div>
  <div class="comparison-col comparison-no">
    <h3>Was gibt es bei uns nicht</h3>
    <ul>
      <li>Feuer</li>
      <li>Rauch</li>
      <li>Gewalt</li>
    </ul>
  </div>
</div>

## Bilder

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
