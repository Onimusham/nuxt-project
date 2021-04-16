<template>

  <div class="container w-full">
      <div class="m-auto text-6xl">
        Pipentrega
      </div> 
    <div class="m-2 py-5 flex">
        <input class="border border-gray-500 w-full" id="tag" type="text" placeholder="qcq come!?">
    </div>    
    <div class="w-full">
      <div class="m-1 h-20 px-10 border border-black" v-for="itemData of data" :key="itemData.name">
        <Item :item="itemData"/>
      </div>
      
    </div>
    <!-- <div class="subtitle">
      <a v-for="arquivojs of fileJS" :key="arquivojs" class="px-8 sm:px-10 lg:px-12 m-auto">
            
      </a> -->
      
  </div>
     
      
      
      
    
     

    <!-- <div>

      <Logo />
      <h1 class="title">
        
      </h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Menu
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div> -->
</template>

// <script>
// export default {}
// console.log("teste#########################")
import rawData from "@/assets/dados.json"

// console.log(arquivojs)
// let fileJS=arquivojs

import Vue from 'vue'

  export default Vue.extend({
    data() {
      const data = rawData
      return {
        data
      }
    }
  })
</script>

<style>
/*Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
::-webkit-input-placeholder {
   text-align: center;
}

:-moz-placeholder { /* Firefox 18- */
   text-align: center;  
}

::-moz-placeholder {  /* Firefox 19+ */
   text-align: center;  
}

:-ms-input-placeholder {  
   text-align: center; 
}
</style>
