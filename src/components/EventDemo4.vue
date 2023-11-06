<script>
export default {
  data(){
    return{

    }
  },
  methods:{
    clickHandler(e){
      // e.preventDefault();
      console.log("点击了")
    },
    clickDiv(){
      console.log("DIV")
    },
    clickP(){
      console.log("P")
    }
  }
}


</script>

<template>
  <h3>事件修饰符</h3>
  <a @click.prevent="clickHandler" href="https://dreaminglri.cn">我的网页</a>
  <div @click="clickDiv">
    <p @click.stop="clickP">测试冒泡</p>
  </div>
</template>

<style scoped>

</style>