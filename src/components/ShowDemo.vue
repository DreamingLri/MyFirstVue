<script setup lang="ts">
// export default {
//   data(){
//     return{
//       names:["111","222","333"],
//       userdata:[{
//         name:"a",
//         age:10,
//         gender: "male",
//       },{
//         name: "b",
//         age: 20,
//         gender: "female"
//       }]
//     }
//   }
// }
import {ref} from "vue";

const names = ref(["111","222","333"])
const userdata = ref([{
  name:"a",
  age:10,
  gender:"male"
},{
  name:"b",
  age:20,
  gender:"female"
}])
</script>

<template>
  <h3>列表渲染</h3>
  <p v-for="(name,index) in names"> {{name}}-{{index}} </p>
  <div v-for="value in userdata">
    <p>{{ value.name }} - {{value.age}} - {{value.gender }}</p>
  </div>
</template>

<style scoped>

</style>