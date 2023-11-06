<script setup lang="ts">
// export default {
//   data(){
//     return{
//       users:["ame","frank","lisa"]
//     }
//   },
//   methods:{
//     userNameHandler(name,e){
//       console.log(name)
//       console.log(e)
//     }
//   }
// }
import {ref} from "vue";
const users = ref(["ame","frank","lisa"])
function userNameHandler(name:string,e:Event){
  console.log(name)
  console.log(e)
}
</script>

<template>
  <h3>事件传参</h3>
  <div v-for="user in users" @click="userNameHandler(user,$event)">
    <p>{{user}}</p>
  </div>
</template>

<style scoped>

</style>