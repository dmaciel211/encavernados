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
  <section class="home-about">
  <div class="home-about__inner">
  <p>
    <strong>Encavernados</strong> es un grupo de reflexión filosófica que nació hace una década en Lomas de Zamora. 
    En sus orígenes estuvo formado por docentes y estudiantes de filosofía, y con el tiempo se fueron sumando miradas de otras disciplinas: 
    Letras, Psicología, Historia, Sociología, Pedagogía, además de artistas y autodidactas. 
    Esa diversidad sigue siendo hoy nuestra mayor riqueza.
  </p>



  <p>
    De nuestras reuniones surgieron charlas, seminarios, talleres y publicaciones. 
    También tres libros colectivos: <em>Filosofía argentina</em> (2021), <em>Filosofía y tango</em> (2023) y <em>Filosofía y poder</em> (2025). 
    Ni siquiera la pandemia detuvo nuestra actividad: continuamos encontrándonos y sosteniendo la práctica filosófica como un espacio compartido.
  </p>



  <p>
    Actualmente el grupo está integrado por <strong>María Meza</strong>, <strong>Nieves Ioannu</strong>, <strong>Natalia Antelo</strong>, 
    <strong>Sebastián Gerez</strong> y <strong>Carlos Butavand</strong>. 
    Seguimos trabajando con la misma convicción: hacer comunidad, pensar con libertad y poner la filosofía en diálogo con la vida cotidiana.
  </p>



  <p>
    Esta página es parte de esa búsqueda. Queremos que sea un punto de encuentro abierto, donde leer, discutir y compartir ideas. 
    Porque la filosofía, para nosotros, no es una disciplina encerrada en los libros: es una práctica viva, crítica y comunitaria.
  </p>
  </div>
</section>
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