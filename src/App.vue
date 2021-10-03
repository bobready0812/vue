<template>
    <div class="calc">
        <div @click="insert1" class="btn">
            <button>1</button>
        </div>
        <div @click="insert2" class="btn">
            <button>2</button>
        </div>
        <div @click="insert3" class="btn">
            <button>3</button>
        </div>
        <div @click="insert4" class="btn">
            <button>4</button>
        </div>
        <div @click="insert5" class="btn">
            <button>5</button>
        </div>
        <div @click="insert6" class="btn">
            <button>6</button>
        </div>
        <div @click="insert7" class="btn">
            <button>7</button>
        </div>
        <div @click="insert8" class="btn">
            <button>8</button>
        </div>
        <div @click="insert9" class="btn">
            <button>9</button>
        </div>
        
        <div class="num1">
            <h1>
                {{num1}}
            </h1>
        </div>
        <div class="num1">
            <h1>
                {{num2}}
            </h1>
        </div>
         <div class="num1">
            <h1>
                {{num3}}
            </h1>
        </div>
        <div class="num1">
            <h1>
                {{times1}}
            </h1>
        </div>
    </div>
    <div @click="times" class="btn">
            <button>X</button>
        </div>
</template>

<script>

    export default {
        name: 'App',
        data() {
            return {num1: 0, num2: 0, num3:0, times1: 0}
        },
        methods: {

            insert1() {
                if (this.num1 == 0) {
                    this.num1 = 1;
                } else if (this.num2 == 0) {
                    this.num2 = 1;
                } else {
                    this.num3 = 1;
                }

            },

            insert2() {

               if (this.num1 == 0) {
                    this.num1 = 2;
                } else if (this.num2 == 0) {
                    this.num2 = 2;
                } else {
                    this.num3 = 2;
                }
            },

            insert3() {

                 if (this.num1 == 0) {
                    this.num1 = 3;
                } else if (this.num2 == 0) {
                    this.num2 = 3;
                } else {
                    this.num3 = 3;
                }
            },

            insert4() {

                 if (this.num1 == 0) {
                    this.num1 = 4;
                } else if (this.num2 == 0) {
                    this.num2 = 4;
                } else {
                    this.num3 = 4;
                }
            },

            insert5() {

               if (this.num1 == 0) {
                    this.num1 = 5;
                } else if (this.num2 == 0) {
                    this.num2 = 5;
                } else {
                    this.num3 = 5;
                }
            },

            insert6() {

                 if (this.num1 == 0) {
                    this.num1 = 6;
                } else if (this.num2 == 0) {
                    this.num2 = 6;
                } else {
                    this.num3 = 6;
                }
            },

            insert7() {

               if (this.num1 == 0) {
                    this.num1 = 7;
                } else if (this.num2 == 0) {
                    this.num2 = 7;
                } else {
                    this.num3 = 7;
                }
            },

            insert8() {

              if (this.num1 == 0) {
                    this.num1 = 8;
                } else if (this.num2 == 0) {
                    this.num2 = 8;
                } else {
                    this.num3 = 8;
                }
            },

            insert9() {

                if (this.num1 == 0) {
                    this.num1 = 9 ;
                } else if (this.num2 == 0) {
                    this.num2 = 9;
                } else {
                    this.num3 = 9;
                }

            },

            times() {
                this.times1 = this.num1 * this.num2 * this.num3;
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

    button {
        font-size: 50px;
        background-color: aquamarine;
    }
</style>