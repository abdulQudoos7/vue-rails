<template>
<div>
    <h1>Events in Vue </h1>
    <button v-on:click="getMsg()">Click Me</button>

    <button @click="getMsg()">Using shorten @ </button>

    <button v-on:click="getMsg1('Passing params Alert')">Passing params</button>

</div>
</template>
<script>
import { registerRuntimeCompiler } from 'vue';

export default{
    name: 'Event',
    data() {
    },
    methods: {
        getMsg(){
            alert("hello world")
        },
        getMsg1(text){
            alert(text)
        }
    }
}
</script>
<style>
</style>