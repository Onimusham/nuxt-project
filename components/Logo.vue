<template>
  <main class="-m-24 sm:-m-10 m lg:m-32">
    <div class='flex pb-40 md:pb-12 lg:pb-52'>
      <img class="mx-auto w-60" src="@/assets/Tita-drinking.png" />
    </div>
    <div class='font-cantarell text-2xl lg:text-3xl subpixel-antialiased pt-5 cursor-default text-gray-800'>
      <div class="flex flex-row py-1.5 mx-7">
        <div v-for="letter of tita" :key="letter" class="px-8 sm:px-10 lg:px-12 m-auto">
          {{ letter }}
        </div>
      </div>
      <div class="bg-black h-0.5 sm:h-10" />
      <div class="flex flex-row py-1.5 mx-7">
        <div v-for="letter of rest" :key="letter" class="px-8 sm:px-10 lg:px-12 m-auto">
          {{ letter }}
        </div>
      </div>
    </div>
  </main>
</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    data() {
      const tita = "tita"//["T", "I", "T", "A"]
      const rest = "restaurante"//["R", "E", "S", "T", "A", "U", "R", "A", "N", "T", "E"]
      return {
        tita,
        rest
      }
    }
  })
</script>


<style>
.NuxtLogo {
  animation: 1s appear;
  margin: auto;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>
