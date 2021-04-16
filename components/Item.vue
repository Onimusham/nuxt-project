<template>
    <div class="container w-full">
        <div class="text-2xl p-1">
            {{item.name.toUpperCase()}}
        </div>
        <div class="italic flex flex-row-reverse">
            {{item.type}}
        </div>
    </div>
</template>

// <script>
// export default {}
// console.log("teste#########################")
import rawData from "@/assets/dados.json"

// console.log(arquivojs)
// let fileJS=arquivojs

import Vue from 'vue'

  export default Vue.extend({
        props: {
          item: {
            type: Object,
            default() {
                return {}
            }
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
</style>
