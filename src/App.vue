<template>
<div class="calc">
    <div @click=insert1 class="btn">
        <button>1</button>
    </div>
     <div @click=insert2 class="btn">
        <button>2</button>
    </div>
     <div @click=insert3 class="btn">
        <button>3</button>
    </div>
     <div  @click=insert4 class="btn">
        <button>4</button>
    </div>
     <div @click=insert5 class="btn">
        <button>5</button>
    </div>
     <div  @click=insert6 class="btn">
        <button>6</button>
    </div>
     <div  @click=insert7 class="btn">
        <button>7</button>
    </div>
     <div @click=insert8 class="btn">
        <button>8</button>
    </div>
     <div @click=insert9 class="btn">
        <button>9</button>
    </div>
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
        
        times() {
            
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
}
    
</style>