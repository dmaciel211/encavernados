---
title: "Encavernados"
draft: false
---

<section class="home-hero">
  <div class="home-hero__media">
    <picture>
      <!-- versión mobile -->
      <source srcset="/media/portadamobile.webp" media="(max-width: 768px)">
      <!-- versión desktop -->
      <img src="/media/portada.webp" alt="Encavernados">
    </picture>
  </div>
  <div class="home-hero__text">
  </div>
</section>

<script>
document.addEventListener('DOMContentLoaded', () => {
  document.querySelectorAll('.home .post-summary .post-cover').forEach(img => {
    function tag() {
      const w = img.naturalWidth || img.width;
      const h = img.naturalHeight || img.height;
      if (w && h && h > w) img.classList.add('is-portrait');
    }
    if (img.complete) tag();
    else img.addEventListener('load', tag, { once: true });
  });
});
</script>