<script>
export default {
  data(){
    return{
      cansee:true
    }
  }
}
</script>

<template>
  <div>
    <h3>条件渲染</h3>
  </div>
  <div v-if="cansee">你能看见我吗</div>
  <div v-else>看看我</div>
  <button @click="cansee = false">点一下</button>
</template>

<style scoped>

</style>