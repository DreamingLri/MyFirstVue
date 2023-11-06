<script setup lang="ts">
// export default {
//   data(){
//     return{
//       count: 0
//     }
//   },
//   methods:{
//     countAdd(e){
//       console.log(e)
//       this.count++
//     }
//   }
// }

import {ref} from "vue";

const count = ref(0)

function countAdd(e){
  console.log(e)
  count.value++
}
</script>

<template>
 <h3>事件传参</h3>
  <div>
    <p>{{count}}</p>
    <button @click="countAdd">点一下</button>
  </div>
</template>

<style scoped>

</style>