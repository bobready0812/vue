<template>
    <input class="num1">
    <br>
    <input class="num2">
    <br>
    <button @click="add" class="sum">더하기</button>
    <h1 class="h1"> {{sum}} </h1>
</template>

<script>

    export default {
        name: 'App',
        data() {
            return {
                sum:null,

                    }
        },
        methods: {
          add() {
              const num1 = document.querySelector(".num1");
              const num2 = document.querySelector(".num2");

              this.sum = Number(num1.value) * Number(num2.value);
          }
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

    .num1{
        margin: 30px;
        font-size: 50px;
    }

    .num2{
        margin: 30px;
        font-size: 50px;
    }

    button {
        font-size:50px;
    }
    
</style>