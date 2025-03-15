<script setup lang="ts">
import Header from '../components/Header.vue'
import About from '../components/About.vue'
import Projects from '../components/Projects.vue'
import {ref} from 'vue'

const position = ref({
  x: 0,
  y: 0
})
function onMouseMove (e: any) {
  position.value.x = e.clientX + window.scrollX
  position.value.y = e.clientY + window.scrollY
}
</script>

<template>
  <main @mousemove="onMouseMove">
    <Header />
    <About />
    <Projects />
    <div class="mouse-effect"
      :style="{top: `${position.y}px`, left: `${position.x}px`}">
    </div>
  </main>
</template>
<style scoped>
.mouse-effect {
  height: 5rem;
  pointer-events: none;
  width: 5rem;
  background: rgb(0,85,230);
  filter: blur(4rem);
  background: linear-gradient(90deg, rgba(0,85,230,1) 0%, rgba(126,21,191,1) 31%, rgba(19,96,182,1) 52%, rgba(97,18,174,1) 74%, rgba(9,9,121,1) 100%, rgba(0,212,255,1) 100%);
  position: absolute;
}
</style>
