<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="bg-slate-950 text-slate-100 w-full mx-auto">
    <RouterView />
  </div>
</template>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: #e9d5ff;
}

::-webkit-scrollbar-thumb {
  border-radius: 15px;
  background: #c084fc;
}
</style>
