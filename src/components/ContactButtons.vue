<script setup>
import ContactModal from "./ContactModal.vue";
import {ref} from "vue";
const show = ref(false);
const handleModalContacs = () => {
  show.value = !show.value;
}
</script>
<template>
  <ContactModal :show="show" @close-modal="handleModalContacs"/>
  <div class="contact-buttons-main">
    <button data-modal-target="default-modal" data-modal-toggle="default-modal" @click="handleModalContacs">Entre em Contato</button>
    <a title="Linkedin" href="https://www.linkedin.com/in/hermes-santos-8596031a0/">
      <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="25" height="25" viewBox="0 0 50 50" style="background-color: black;">
        <path fill="#FFFFFF" d="M41,4H9C6.24,4,4,6.24,4,9v32c0,2.76,2.24,5,5,5h32c2.76,0,5-2.24,5-5V9C46,6.24,43.76,4,41,4z M17,20v19h-6V20H17z M11,14.47c0-1.4,1.2-2.47,3-2.47s2.93,1.07,3,2.47c0,1.4-1.12,2.53-3,2.53C12.2,17,11,15.87,11,14.47z M39,39h-6c0,0,0-9.26,0-10 c0-2-1-4-3.5-4.04h-0.08C27,24.96,26,27.02,26,29c0,0.91,0,10,0,10h-6V20h6v2.56c0,0,1.93-2.56,5.81-2.56 c3.97,0,7.19,2.73,7.19,8.26V39z"></path>
      </svg>
    </a>
    <a title="Github" href="https://github.com/HermesSantos">
      <svg width="15" height="15" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg" class="h-5 w-5"><path d="M7.49933 0.25C3.49635 0.25 0.25 3.49593 0.25 7.50024C0.25 10.703 2.32715 13.4206 5.2081 14.3797C5.57084 14.446 5.70302 14.2222 5.70302 14.0299C5.70302 13.8576 5.69679 13.4019 5.69323 12.797C3.67661 13.235 3.25112 11.825 3.25112 11.825C2.92132 10.9874 2.44599 10.7644 2.44599 10.7644C1.78773 10.3149 2.49584 10.3238 2.49584 10.3238C3.22353 10.375 3.60629 11.0711 3.60629 11.0711C4.25298 12.1788 5.30335 11.8588 5.71638 11.6732C5.78225 11.205 5.96962 10.8854 6.17658 10.7043C4.56675 10.5209 2.87415 9.89918 2.87415 7.12104C2.87415 6.32925 3.15677 5.68257 3.62053 5.17563C3.54576 4.99226 3.29697 4.25521 3.69174 3.25691C3.69174 3.25691 4.30015 3.06196 5.68522 3.99973C6.26337 3.83906 6.8838 3.75895 7.50022 3.75583C8.1162 3.75895 8.73619 3.83906 9.31523 3.99973C10.6994 3.06196 11.3069 3.25691 11.3069 3.25691C11.7026 4.25521 11.4538 4.99226 11.3795 5.17563C11.8441 5.68257 12.1245 6.32925 12.1245 7.12104C12.1245 9.9063 10.4292 10.5192 8.81452 10.6985C9.07444 10.9224 9.30633 11.3648 9.30633 12.0413C9.30633 13.0102 9.29742 13.7922 9.29742 14.0299C9.29742 14.2239 9.42828 14.4496 9.79591 14.3788C12.6746 13.4179 14.75 10.7025 14.75 7.50024C14.75 3.49593 11.5036 0.25 7.49933 0.25Z" fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"></path></svg>
    </a>
    <button>Experiências</button>
  </div>
</template>
<style scoped lang="scss">
a {
  color: white;
  text-decoration: none;
}
.contact-buttons-main{
  display: flex;
  justify-content: center;
  margin-top: 5rem;
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

  a:hover {
    border: 2px solid #7953cd;
    transition: 0.3s;
  }

  a {
    margin: 0 1rem;
    padding: .5rem 2rem;
    background-color: #7953cd;
    border-radius: .3rem;
    background: none;
    border: 2px solid grey;
    font-size: .8rem;
    cursor: pointer;
  }
}
</style>
