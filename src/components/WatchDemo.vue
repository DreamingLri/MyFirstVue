<script setup lang="ts">
import {ref, watch} from "vue";

const message = ref("Hello")
function updateHander(){
  message.value = "World"
}

// watch(message, async (newValue, oldValue)=>{
//   console.log(newValue, oldValue)
// })
watch(message,(newValue,oldValue)=>{
  console.log(newValue,oldValue)
})
</script>

<template>
  <h3>侦听器</h3>
  <p>{{message}}</p>
  <button @click="updateHander">修改数据</button>
</template>

<style scoped>

</style>