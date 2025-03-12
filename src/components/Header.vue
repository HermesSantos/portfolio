<script setup lang="ts">
import {ref} from 'vue'
import ModalContact from './ContactModal.vue';

const show = ref(false);
const handleModal = () => {
  show.value = !show.value
}
</script>

<template>
  <div class="header-main lg:text-base text-5xl">
    <ModalContact :show="show" @close-modal="handleModal"/>
    <div class="header-items">
      <a href="#about-section" class="header-link-item">Sobre</a>
      <a href="#tech-section" class="header-link-item">Tecnologias</a>
      <!-- <a href="#projects-section" class="header-link-item">Projetos</a> -->
      <!-- <a href="#xp-section" class="header-link-item">Experiências</a> -->
      <button @click="handleModal" class="header-link-item">Contatos</button>
    </div>
  </div>
</template>
<style scoped lang="scss">
a {
  color: white;
  text-decoration: none;
}
.header-main {
  background-color: #0a0a0a;
  color: white;
  padding: 1rem 5rem;
  width: 100%;
  position: fixed;
  align-items: center;
  box-shadow: 0 1px 2px -2px white;
  .header-items {
    display: flex;
    justify-content: center;
  }
  .header-link-item {
    margin: 0 2rem;
    cursor: pointer;
  }
  .header-link-item:hover {
    color: #7953cd;
    transition: 0.3s;
  }
}
</style>
