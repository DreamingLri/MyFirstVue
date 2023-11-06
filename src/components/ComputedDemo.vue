<script setup lang="ts  ">
// export default {
//   data(){
//     return{
//       user:{
//         name:"lisa",
//         conten:["1","2","3"]
//       }
//     }
//   },
//   computed:{
//     //计算属性，进行缓存
//     userContent(){
//       return this.user.conten.length > 0 ? "Yes":"No"
//     }
//   }
// }
import {computed, ref} from "vue";
const user = ref({
  name:"lisa",
  content:["1","2","3"]
})

const userContent = computed(() =>{
  return user.value.content.length > 0 ? "Yes":"No"
})
</script>

<template>
  <h3>{{user.name}}</h3>
  <p>{{ userContent }}</p>
</template>

<style scoped>

</style>