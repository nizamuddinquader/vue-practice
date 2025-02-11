<script setup>
import { ref } from 'vue';


  // const myFun=()=>{
  // }
  const  count = ref(0)
</script>

<template>

   <button @click="myFun()">I am button</button>
   <h1>{{ count }}</h1>
   <h2>{{ count }}</h2>
   <h3>{{ count }}</h3>
   <h4>{{ count }}</h4>
   <h5>{{ count }}</h5>
   <h6>{{ count }}</h6>
   <input type="text" placeholder="type here" v-model="count">

</template>

<style scoped>

</style>