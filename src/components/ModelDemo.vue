<script setup lang="ts">
import {ref} from "vue";

const message = ref("")
const checked = ref(true)
function chat(){
  if (message.value === "1"){
    message.value = "这是1"
  }
}
</script>

<template>
  <h3>表单输入绑定</h3>
  <form>
    <input type="text" v-model="message">
    <input type="checkbox" id="checkbox" v-model="checked">
    <label for="checkbox">{{checked}}</label>
    <p>{{message}}</p>
  </form>
</template>

<style scoped>

</style>