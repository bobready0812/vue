<template>
  
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <h1 class="clock">00:00</h1>
</template>

<script>


import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
const clock = document.querySelector(".clock") 


function getClock() {
  const date = new Date();
  const hours = String(date.getHours());
  const minutes = String(date.getMinutes());

  clock.innerText =`${hours}:${minutes}`;
}

setInterval(getClock,1000);

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
