<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  projectName: String,
  projectDescription: String,
  projectLanguage: String,
  projectUrl: String
})

</script>
<template>
  <div class="max-w-sm border-2 border-solid text-white rounded overflow-hidden shadow-lg">
    <div class="px-6 py-4">
      <div class="font-bold text-xl mb-2">{{projectName}}</div>
      <p class="text-white text-base">{{projectDescription}}</p>
    </div>
    <div class="px-6 pt-4 pb-2">
      <div>
        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#{{projectLanguage}}</span>
      </div>
      <div class="mt-2 flex align-center justify-center px-2 pt-2 pb-2">
        <button target="_blank" :href="projectUrl" data-modal-target="default-modal" data-modal-toggle="default-modal" @click="handleModalContacs">Saber Mais</button>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
p {
  text-transform: capitalize;
}
button {
  margin: 0 1rem;
  padding: .5rem 2rem;
  background-color: #7953cd;
  border-radius: .3rem;
  background: none;
  border: 2px solid grey;
  font-size: .8rem;
  cursor: pointer;
}
button:hover {
  border: 2px solid #7953cd;
  transition: 0.3s;
}
</style>
