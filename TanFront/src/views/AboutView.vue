<template>
  <div class="about">
    <h1>Tan Webpage</h1>
    <br />
    <p>
      Esta pagina web busca ayudar a los viajeros en sus aventuras guardando
      lugares y aventuras favoritas en cada lugar.Asi mismo poder compartir esta
      informacion con otros usuarios .
    </p>
    <h1>Ubicación Actual</h1>
    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1335.9958305118894!2d-77.02270115921559!3d-12.13535652313325!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105b7fcaea4a133%3A0xb86fbddb0dc89e2e!2sUniversidad%20de%20Ingenier%C3%ADa%20y%20Tecnolog%C3%ADa%20-%20UTEC!5e0!3m2!1ses!2spe!4v1653358501595!5m2!1ses!2spe"
      width="700"
      height="600"
      style="border: 0; padding: 20px"
      allowfullscreen=""
      loading="lazy"
      referrerpolicy="no-referrer-when-downgrade"
    ></iframe>
  </div>
</template>

<script>
export default {
  name: "AboutView",
  components: {},
};
</script>

<style scoped>
.about {
  margin-top: 20px;
  font-family: Helvetica, Arial, sans-serif;
  color: #444444;
  margin-left: 190px;
  width: 60%;
}

h1 {
  font-weight: 500;
}
</style>
