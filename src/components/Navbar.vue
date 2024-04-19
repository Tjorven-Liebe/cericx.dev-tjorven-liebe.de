<script setup>

import {ref} from "vue";

let props = defineProps(['title', 'items'])
let isActive = ref("Home");
//
// addEventListener("scroll", () => {
//   let elementById = document.getElementById("main-nav")
//   if (window.scrollY > 0) {
//     elementById.classList.add("navbar-shadow")
//   } else
//     elementById.classList.remove("navbar-shadow")
// });
</script>

<template>
  <nav id="main-nav" class="navbar navbar-expand-lg">
    <div class="container-fluid">
      <a class="navbar-brand" href="#"><img src="https://cdn.discordapp.com/avatars/428284027519369217/0684c3e0ead56a37f55cffe7934f18ac.gif?size=256" height="40"/>{{ props.title }}</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mx-auto navbar-center">
          <li v-for="item in props.items" class="nav-item text-uppercase">
            <a :href="'#' + item " class="nav-link" @click="isActive = item;" :class="{ active: (isActive===item ? 'active' : '') }">{{ item }}</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>

@media only screen and (min-width: 990px){
  .navbar-brand {
    position: absolute !important;
  }
}

.navbar-collapse {
  align-items: center !important;
}
</style>