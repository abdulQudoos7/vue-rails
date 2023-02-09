<template>
    <h1>Child Component</h1>
    <p>Child gets from parent => {{ text }}</p>
    <p>Child gets data from parent => {{ user }} </p>
    <button @click="sendData(2,2)">Click me</button>

</template>
<script>
export default{
    name: 'Child',
    props:{
        text: String,
        user: Object,
        sendData: Function,
    }
}
</script>
<style></style>