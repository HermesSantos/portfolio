<script setup lang="ts">
import Card from "./Card.vue"
import {onMounted, ref} from 'vue'

onMounted(() => {
  fetch('https://api.github.com/users/HermesSantos/repos', {
    method: 'get'
  }).then(response => response.json())
    .then((data: GithubProject[]) => {
      projects.value = data.filter(el => el.name === 'aila' || el.name === 'auto-like')
    })
})

const allowedProjects = ['aila', 'auto-like']
const projects = ref<GithubProject[]>()

</script>
<template>
  <div class="flex flex-col items-center justify-center px-10 pt-15">
    <h1 class="text-5xl pb-10">Projetos</h1>
  </div>
  <div class="flex flex-row align-center justify-center px-10 pt-10 pb-10 gap-4">
    <Card v-for="project in projects"
      :key="project.id"
      :projectName="project.name"
      :projectDescription="project.description"
      :projectLanguage="project.language"
      :projectUrl="project.clone_url"
    />
  </div>
</template>
<style lang="scss" scoped>
</style>
