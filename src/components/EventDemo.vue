<script setup lang="ts">
// export default {
//   data(){
//     return{
//       count: 0
//     }
//   },
//   methods:{
//     addCount(){
//       this.count++
//     }
//   }
// }
import {ref} from "vue";
const count = ref(0)
function addCount(){
  count.value++
}
</script>

<template>
  <h3>EventDemo</h3>
  <div>
    <button @click="count++">点一下-{{count}}</button>
    <p></p>
    <button @click="addCount">点一下-{{count}}</button>
  </div>
</template>

<style scoped>

</style>