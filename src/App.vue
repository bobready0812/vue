<template>
   <div class = "arrange">
   <h1> {{num1}} </h1>
   <h1> {{num2}} </h1>
   <h1> {{num3}} </h1>
   <h1> {{sum}} </h1>
   <button id="btn1" @click="increase1">1</button>
   <button id="btn2" @click="increase2">2</button>
   <button id="btn3" @click="increase3">3</button>
   <button id="btn4" @click="increase4">4</button>
   <button id="btn5" @click="increase5">5</button>
   <button id="btn6" @click="increase6">6</button>
   <button id="btn7" @click="increase7">7</button>
   <button id="btn8" @click="increase8">8</button>
   <button id="btn9" @click="increase9">9</button>
   <br>
   <button class="add" @click="add">Add</button>
   <br>
   <button class="add" @click="reset">Reset</button>
   <br>
   <button class="reset" @click="reset2">Hide</button>
   </div>
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
             ,
            reset2() {
                const button1 =document.getElementById("btn1");
                const button2 =document.getElementById("btn2");
                const button3 =document.getElementById("btn3");
                const button4 =document.getElementById("btn4");
                const button5 =document.getElementById("btn5");
                const button6 =document.getElementById("btn6");
                const button7 =document.getElementById("btn7");
                const button8 =document.getElementById("btn8");
                const button9 =document.getElementById("btn9");
                button1.classList.add("hidden");
                button2.classList.add("hidden");
                button3.classList.add("hidden");
                button4.classList.add("hidden");
                button5.classList.add("hidden");
                button6.classList.add("hidden");
                button7.classList.add("hidden");
                button8.classList.add("hidden");
                button9.classList.add("hidden");
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
        font-size: 150px;
        padding: 20px;
    }
    
    button {
        font-size:50px;
        padding:20px;
        height: 100px;
        
    }
    
    .hidden {
        display: none;
    }
    
    .arrange {
        display: flex;
    }

    
    
</style>