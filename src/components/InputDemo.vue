<script setup lang="ts">
import {ref} from "vue";

const message = ref('')
</script>

<template>
  <p>Message is {{message}}</p>
  <input v-model="message" placeholder="input" />
</template>

<style scoped>

</style>