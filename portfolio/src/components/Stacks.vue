<template>
  <div id="stacks" class="p-8">
    <div class="mx-auto">
      <h3 class="text-center text-[46px] font-semibold mb-2 text-slate-100 hover:text-purple-500">My Tech Stacks</h3>
      <p class="text-center text-slate-100 text-lg">Technologies I’ve been working with recently</p>
    </div>
    <div class="grid grid-cols-4 gap-y-4 gap-y-6 place-items-center my-20">
      <a href="https://www.w3schools.com/html/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/html.svg" alt="html" width="120" height="120">
      </a>
      <a href="https://www.w3schools.com/css/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/css.svg" alt="css" width="120" height="120">
      </a>
      <a href="https://www.w3schools.com/js/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/js.svg" alt="js" width="120" height="120">
      </a>
      <a href="https://getbootstrap.com/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/bootstrap.svg" alt="bootstrap" width="120" height="120">
      </a>
      <a href="https://tailwindcss.com/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/tailwind.svg" alt="tailwind" width="120" height="120">
      </a>
      <a href="https://vuejs.org/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/Vue.js_Logo_2.svg.png" alt="vue" width="120" height="120">
      </a>
      <a href="https://quasar.dev/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/quasar-logo.svg" alt="quasar" width="120" height="120">
      </a>
      <a href="https://legacy.reactjs.org/" class="block p-2 my-2 cursor-pointer">
        <img class="block" src="../assets/react.svg" alt="react" width="120" height="120">
      </a>
      <a href="https://git-scm.com/" class="block p-2 my-2 cursor-pointer"  v-on:mouseenter="tooltip=true" v-on:mouseleave="tooltip=false">
        <img class="block" src="../assets/git.svg" alt="git" width="120" height="120">
      </a>
      <a href="https://github.com/" class="block p-2 my-2 cursor-pointer"  v-on:mouseenter="tooltip=true" v-on:mouseleave="tooltip=false">
        <img class="block" src="../assets/github.svg" alt="github" width="120" height="120">
      </a>
      <a href="https://gitlab.com/" class="block p-2 my-2 cursor-pointer"  v-on:mouseenter="tooltip=true" v-on:mouseleave="tooltip=false">
        <img class="block" src="../assets/gitlab.svg" alt="github" width="120" height="120">
      </a>
      <a href="https://code.visualstudio.com/" class="block p-2 my-2 cursor-pointer"  v-on:mouseenter="tooltip=true" v-on:mouseleave="tooltip=false">
        <img class="block" src="../assets/vscode.svg" alt="vscode" width="120" height="120">
      </a>
    </div>
  </div>
</template>
<script setup>
  import { ref } from 'vue'
  let tooltip = ref(false)
</script>
