<script setup lang="ts">
</script>

<template>
  <div class="header-main">
    <div class="header-items">
      <a class="header-link-item">Sobre</a>
      <a class="header-link-item">Skills</a>
      <a class="header-link-item">Projetos</a>
      <a class="header-link-item">Experiências</a>
      <a class="header-link-item">Contatos</a>
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
