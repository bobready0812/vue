<template>
   
   <h1> {{num1}} </h1>
   <h1> {{num2}} </h1>
   <h1> {{num3}} </h1>
   <h1> {{sum}} </h1>
   <button @click="increase1">1</button>
   <button @click="increase2">2</button>
   <button @click="increase3">3</button>
   <button @click="increase4">4</button>
   <button @click="increase5">5</button>
   <button @click="increase6">6</button>
   <button @click="increase7">7</button>
   <button @click="increase8">8</button>
   <button @click="increase9">9</button>
   <br>
   <button class="add" @click="add">Add</button>
   <br>
   <button class="add" @click="reset">Reset</button>
</template>

<script>

    export default {
        name: 'App',
        data() {
            return {
               num1:null,
               num2:null,
               num3:null,
               sum:null
                    }
        },
        methods: { 
            increase1() {
            if(this.num1 == null) {
                this.num1 = 1;
            } else if(this.num2 == null) {
                this.num2 = 1;
            } else {
                this.num3 = 1;
            }

            },
            increase2() {
            if(this.num1 == null) {
                this.num1 = 2;
            } else if(this.num2 == null) {
                this.num2 = 2;
            } else {
                this.num3 = 2;
            }
            },
            increase3() {
           if(this.num1 == null) {
                this.num1 = 3;
            } else if(this.num2 == null) {
                this.num2 = 3;
            } else {
                this.num3 = 3;
            }
            },
            increase4() {
            if(this.num1 == null) {
                this.num1 = 4;
            } else if(this.num2 == null) {
                this.num2 = 4;
            } else {
                this.num3 = 4;
            }
            },
            increase5() {
           if(this.num1 == null) {
                this.num1 = 5;
            } else if(this.num2 == null) {
                this.num2 = 5;
            } else {
                this.num3 = 5;
            }
            },
            increase6() {
            if(this.num1 == null) {
                this.num1 = 6;
            } else if(this.num2 == null) {
                this.num2 = 6;
            } else {
                this.num3 = 6;
            }
            },
            increase7() {
            if(this.num1 == null) {
                this.num1 = 7;
            } else if(this.num2 == null) {
                this.num2 = 7;
            } else {
                this.num3 = 7;
            }
            },
            increase8() {
            if(this.num1 == null) {
                this.num1 = 8;
            } else if(this.num2 == null) {
                this.num2 = 8;
            } else {
                this.num3 = 8;
            }
            },
            increase9() {
            if(this.num1 == null) {
                this.num1 = 9;
            } else if(this.num2 == null) {
                this.num2 = 9;
            } else {
                this.num3 = 9;
            }
            },
             
            add() {
              this.sum = this.num1+ this.num2 + this.num3;
            },

            reset() {
                this.num1 = null;
                this.num2 = null;
                this.num3 = null;
                this.sum = null;
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
    

    .add {
        margin: 50px;
    }
    h1 {
        font-size: 100px;
    }
    
    button {
        font-size:100px;
        padding:30px;
    }
 
    
</style>