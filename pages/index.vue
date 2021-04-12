<template>

  <div class="container">
        <h1 class="title">Pipentrega</h1> 
    <div class="search">Pesquise
        <input id="tag" type="text" placeholder="o que quer comer...">
    </div>    
    <ul>
      <li v-for="arquivojs of fileJS" :key="arquivojs">
        {{arquivojs.key1}}
      </li>
      
    </ul>
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
import * as arquivojs from "@/assets/dados.json"
let obj1=JSON.parse(arquivojs)
console.log(arquivojs)
// let fileJS=arquivojs

import Vue from 'vue'

  export default Vue.extend({
    data() {
      
      const fileJS = arquivojs
      return {
        fileJS
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
.container {
  margin: 50;
  min-height: 300;
  display:grid ;
  justify-content:flex;
  align-items: flex;
  text-align: flex;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 100;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 100;
  font-size: 20px;
  color: #526488;
  word-spacing: 5px;
  padding-top: 105px;
}

.links {

  padding-top: 250px;  
}

.search{
  text-align: right;
  font-weight: 200;
  font-size: 30px;
  color: #526488;
}
</style>
