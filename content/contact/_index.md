---
title: "Contacto"
draft: false
---

<section class="contacto">
  <h1>Contacto</h1>

  <form name="contacto"
        method="POST"
        data-netlify="true"
        data-netlify-recaptcha="true"
        netlify-honeypot="bot-field"
        action="/gracias/"
        class="contacto-form">


  <input type="hidden" name="form-name" value="contacto">

  <p class="hidden">
      <label>No completar si sos humano:
        <input name="bot-field">
      </label>
    </p>

  <div class="field">
      <label for="nombre">Nombre</label>
      <input id="nombre" type="text" name="nombre" required>
    </div>

  <div class="field">
      <label for="email">Email</label>
      <input id="email" type="email" name="email" required>
    </div>

  <div class="field">
      <label for="mensaje">Mensaje</label>
      <textarea id="mensaje" name="mensaje" rows="5" required></textarea>
    </div>

  <div data-netlify-recaptcha="true" id="captcha"></div>

  <button type="submit" id="enviar-btn" class="btn">Enviar</button>
  </form>

  <p class="contacto-alt">También podés escribirnos a <a href="mailto:encavernados@gmail.com">encavernados@gmail.com</a>.</p>
</section>

<script>
document.addEventListener("DOMContentLoaded", () => {
  const form = document.querySelector('form[name="contacto"]');
  form.addEventListener("submit", (e) => {
    if (window.grecaptcha && typeof grecaptcha.getResponse === "function") {
      const response = grecaptcha.getResponse();
      if (!response) {
        e.preventDefault();
        alert("Por favor confirmá el reCAPTCHA antes de enviar el mensaje.");
      }
    }
  });
});
</script>
