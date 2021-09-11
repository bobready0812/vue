<template>
    <div class="clock">
        <div class="bg">
            <h2 id="h">{{hours}}</h2>
        </div>
        <h2>:</h2>
        <div class="bg">
            <h2 id="m">{{minutes}}</h2>
        </div>
    </div>
</template>

<script>

    export default {
        name: 'App',
        data() {
            return {hours: 0, minutes: 0}
        },
        methods: {

            getClock() {
                const date = new Date();

                if (date.getHours() > 13) {
                    this.hours = date.getHours() - 12;
                } else if (date.getHours() == 0) {
                    this.hours = 12;
                } else {
                    this.hours = date.getHours();
                }
                this.minutes = this.PadStartMinutes(date.getMinutes());
            },
            setTime() {

                setInterval(this.getClock, 1000)
            },
            PadStartMinutes(digit) {
                return ('0' + digit).slice(-2)
            }
        },
        mounted() {
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

    body {
        background: #ebf5fc;
    }

    .clock {
        color: #000;
        font-size: 56px;
        text-align: center;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 0 20px;
    }

    h2 {
        color: #85C1E9;
        padding: 30px;
    }

    .bg {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 4em;
        height: 4em;
        background: inherit;
        position: relative;
        border-radius: 50%;
        box-shadow: inset -2px -2px 5px rgba(255, 255, 255, 1), inset 3px 3px 5px rgba(0, 0, 0, 0.2);
    }

    #m {
        margin: 0 10px;
    }
</style>