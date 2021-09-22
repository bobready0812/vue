<template>
<div class="calc">
<div class="num1">
  <h1> {{num1}} </h1>
</div> 
<div class="num1">
  <h1> {{num2}} </h1>
</div> 
<div class="num1">
    <h1> {{times1}} </h1>
</div>
</div>
</template>

<script>

    export default {
        name: 'App',
        data() {
            return {
               num1: 0,
               num2: 0,
               times1: 0
                    }
        },
        methods: { 
           
        
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
    
.calc {
    display: flex;
}

.num1 {
    padding: 20px;
}

.num2 {
    padding: 20px;
}

h1 {
    font-size: 50px;
}

    
</style>