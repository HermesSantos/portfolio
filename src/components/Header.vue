<script setup lang="ts">
</script>

<template>
  <div class="header-main">
    <div class="header-items">
      <a>Sobre</a>
      <a>Skills</a>
      <a>Projetos</a>
      <a>Experiência</a>
      <a>Contatos</a>
    </div>
  </div>
</template>
<style scoped>
a {
  margin: 0 2rem;
  cursor: pointer;
}
.header-main {
  background-color: #0a0a0a;
  color: white;
  padding: 1rem 5rem;
  width: 100%;
  position: fixed;
  align-items: center;
  box-shadow: 0 1px 2px -2px white;
}
.header-items {
  display: flex;
  justify-content: center;
}
</style>
