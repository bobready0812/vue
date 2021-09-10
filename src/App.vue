<template>

    <div class="clock">
        <h1 class="clockText">{{hours}}:{{minutes}}</h1>
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

    .clock {

        width: 20%;
        height: 50%;
        background: rgba(14, 48, 201, 0.3);
        border-radius: 20px;
    }

    .clockText {
        font-size: 100px;
        color: aliceblue;
    }
</style>