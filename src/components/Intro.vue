<script>
    export default {
        data () {
            return {
                name: "Jose M. Fuentes",
                position: "Software Engineer Graduate",
                caption: "I am always eager to learn new technologies", 
                caption2: "and utilize them in my problem solving",
                caption3: "approaches."
            }
        }
    }
</script>

<template>
    <h1>{{ name }}</h1>
    <h3>{{ position }}</h3>
    <br>
    <h5>{{ caption }} <br> {{ caption2 }} <br> {{ caption3 }}</h5>
</template>

<style>
    h1 {font-size: 3rem/**48px*/;color: #EFFAFF;}
    h3 {font-weight: lighter;color: #9FADBD;font-size: 1.25rem;}
    h5 {font-weight:lighter;color: #9FADBD;font-size: 1rem;}
</style>
