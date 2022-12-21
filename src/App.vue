<template>
  <div>
    <button @click="Adiciona">+1</button>
    <p v-html="count"></p>
    <button @click="Diminui">-1</button>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const count = ref(0)

function Adiciona () {
  count.value = count.value + 1
}

function Diminui () {
  count.value = count.value - 1
}



// export default {
//   name: 'App',

//   data () {
//     return {
//       count: 0
//     }
//   },

//   methods: {
//     Adiciona () {
//       this.count = this.count + 1
//     },

//     Diminui () {
//       this.count = this.count - 1
//     }
//   },

//   mounted() {
//     alert(`The initial count is ${this.count}`)
//   }
// }

</script>

<style scoped>

</style>
