<script setup lang="ts">
// export default {
//   data(){
//     return{
//       names:["ame","frank","lisa"]
//     }
//   },
//   methods:{
//     addNameHandler(){
//       //引起ui自动更新
//       this.names.push("sakura")
//     }
//   }
// }

import {ref} from 'vue'
const names = ref(["ame","frank","lisa"])
// function addNameHandler(){
//   this.name.push("sakura")
function addName(){
  names.value.push("sakura")
}
</script>

<template>
  <h3>数组侦听</h3>
  <button @click="addName">添加数据</button>
  <ul>
    <li v-for="(name,index) in names" :key="index">{{name}}</li>
  </ul>
</template>

<style scoped>

</style>