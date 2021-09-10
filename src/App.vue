<template>
  
 
      <h1 class="clock">{{hours}}:{{minutes}}</h1>
      
   
</template>

<script>




export default {
  name: 'App',
  data () {
    return {
      hours: 0,
      minutes: 0, 
    }
  },
  methods: {
    
    getClock() {
      const date = new Date();
        this.hours = date.getHours();
        this.minutes = this.PadStartMinutes(date.getMinutes());
    },
    setTime () {
      
      setInterval(this.getClock, 1000)
    },
    PadStartMinutes (digit) {
      return ('0' + digit).slice(-2)
    }
  },
  mounted () {
    this.setTime()
  }
}


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
