<script setup>
import ContactButtons from "./ContactButtons.vue";
import Skills from "./Skills.vue";
</script>

<template>
  <div class="about-main">
    <h1>Hermes Santos</h1>
    <div class="text-about" id="about-section">
      Desenvolvedor apaixonado com uma habilidade especial para solucionar problemas complexos por meio de código. Majoritariamente autodidata, sou movido por uma curiosidade incansável que me leva a explorar e dominar tecnologias como Vue e React para interfaces dinâmicas, Laravel e Node.js para backends robustos, e MySQL para gerenciamento eficiente de dados. Atualmente, estou mergulhando no estudo de Golang, buscando expandir ainda mais minhas capacidades e criar soluções escaláveis e performáticas.
    </div>
    <div id="contact-section">
      <ContactButtons />
    </div>
    <div>
      <Skills />
    </div>
  </div>
</template>
<style lang="scss" scoped>
.about-main{
  h1{
    font-size: 3rem;
    font-weight: 700;
    background: linear-gradient(
      to right,
      #7953cd 20%,
      #00affa 30%,
      #00f5d4 40%,
      #0190cd 70%,
      #764ada 80%
      );
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
    text-fill-color: transparent;
    background-size: 500% auto;
    animation: textShine 3s ease-in-out infinite alternate;
  }
  text-align: center;
  padding: 6rem 25rem;
  .text-about {
    font-size: 1rem;
    margin-top: 3rem;
    text-align: justify;
  }
  @keyframes textShine {
  0% {
    background-position: 0% 50%;
  }
  100% {
    background-position: 100% 50%;
  }
  }
}
</style>
