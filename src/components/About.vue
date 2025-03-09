<script setup lang="ts">
import ContactButtons from "./ContactButtons.vue";
import Skills from "./Skills.vue";
</script>

<template>
  <div class="about-main">
    <h1>Hermes Santos</h1>
    <div class="text-about">
      Desenvolvedor com uma habilidade especial para resolver problemas complexos através de código. Majoritariamente autodidata e movido por uma curiosidade incansável para explorar e dominar novas tecnologias.
    </div>
    <div>
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
    margin-top: 2rem;
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
