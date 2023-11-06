<script setup lang="ts">
import {ref} from 'vue'
const obj = ref({
  stylecolor:'red',
  stylesize:'30px',
})
const fontStyle = {
  color:'skyblue',
  fontSize:'60px'
}
</script>

<template>
  <p :style="{color : obj.stylecolor, fontSize : obj.stylesize}">Style绑定</p>
  <p :style="fontStyle">Style绑定</p>
</template>

<style scoped>

</style>