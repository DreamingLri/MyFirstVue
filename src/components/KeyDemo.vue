<script>
export default {
  data(){
    return{
      userdata:[{
        name:"a",
        age:10,
        gender: "male",
      },{
        name: "b",
        age: 20,
        gender: "female"
      }]
    }
  }
}
</script>

<template>
  <h3>KeyDemo</h3>
  <div v-for="(value,index) in userdata" :key="index"> {{index}}
    <p>{{value.name}}-{{value.age}}-{{value.gender}}</p>
  </div>
</template>

<style scoped>

</style>