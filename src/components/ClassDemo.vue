<script setup lang="ts">
// export default {
//   data(){
//     return{
//       isActive:true,
//       isDanger:true,
//       changes:{
//         'red':true,
//         'big':true
//       }
//     }
//   }
// }
import {reactive, ref} from "vue";

const isActive = ref(true)
const isDanger = ref(true)
const changes = reactive({
  'red':true,
  'big':true
})
</script>

<template>
  <h3 :class="{'active':isActive, 'danger':isDanger}">Class绑定</h3>
  <h3 :class="changes">Class绑定2</h3>

</template>

<style scoped>
.active{
  font-size: 30px;
}
.danger{
  color: aqua;
}
.red{
  color: red;
}
.big{
  font-size: large;
}
</style>