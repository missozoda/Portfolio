<template>
  <div id="about_me" class="mt-[40px] sm:mt-[56px] md:mt-[76px] lg:mt-[91px] py-12 md:py-24">
    <div class="grid grid-cols-3 sm:grid-cols-2 gap-2 md:gap-5 sm:items-center justify-between">
      <div class="lg:pl-20 col-span-2 sm:col-span-1">
        <h2 class="text-slate-100 text-lg sm:text-xl md:text-3xl xl:text-5xl font-semibold italic tracking-wider leading-relaxed">Hi👋, 
          <br> My name is 
          <span class="text-purple-600">Ozoda</span> 
          <br>
          I build things for web
        </h2>
        <button data-modal-target="defaultModal" data-modal-toggle="defaultModal" type="button" class="text-slate-100 bg-purple-600 hover:bg-purple-400 hover:text-slate-950 font-medium rounded-xl text-sm md:text-base px-10 py-1 md:py-2 mt-8 xl:mt-10" @click="modal=true">More</button>
      </div>
      <img class="block ml-auto xl:mr-28 rounded-full border-4 border-purple-600 scale-75 md:scale-90 lg:scale-100" src="../assets/avatar.jpg" alt="avatar" width="350" height="350">
    </div>

    <!-- Modal About me -->
    
    <div id="defaultModal" tabindex="-1" aria-hidden="true" class="fixed top-0 left-0 right-0 z-5 w-full p-4 overflow-x-hidden overflow-y-auto md:inset-0 h-[calc(100%-1rem)] flex justify-center items-center overflow-auto" :class="modal ? 'block bg-slate-950/70' : 'hidden'">
      <div class="relative w-[95%] sm:w-2/3 md:w-1/2 h-auto max-w-2xl max-h-full shadow border-2 border-purple-600 bg-slate-950 rounded-xl">
        <div class="flex items-start justify-between p-2 lg:p-4 border-b rounded-t">
          <h3 class="text-lg lg:text-2xl font-semibold text-slate-100">
              About me
          </h3>
          <button type="button" class="text-slate-100 bg-transparent hover:bg-slate-200 hover:text-slate-900 rounded-lg text-sm p-1.5 ml-auto inline-flex items-center " data-modal-hide="defaultModal" @click="modal=false">
            <svg aria-hidden="true" class="w-4 lg:w-5 h-4 lg:h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path>
            </svg>
            <span class="sr-only">Close modal</span>
          </button>
        </div>
        <div class="h-[85%] overflow-y-auto">
          <div class="text-sm sm:text-base lg:text-lg font-medium p-4 lg:p-8 tracking-wider leading-relaxed text-justify indent-2 text-slate-100">
            I am Ernazarova Ozoda. I am 20 years old and I  am in 3rd year of Tashkent State Technical University named after Islam Karimov.👩‍🎓
            <br>
            <br>
            I am frontend developer. I learn a lot and fast.⚡
            <br>
            I am not afraid of difficulties and always move forward. 
            <br>
            <br>
            I love my job.❤
            </div>
          <div class="flex items-center justify-end mt-6 sm:mt-10 lg:mt-16 mb-4">
            <button class="mx-5 sm:mx-10 text-slate-100 bg-purple-600 hover:bg-purple-400 hover:text-slate-950 font-medium rounded-xl text-sm lg:text-base px-10 py-1  lg:py-2" type="button" @click="modal=false">Exit</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  import { ref } from 'vue'
  let modal = ref(false);
</script>
