<template>
    <h1>Conditional Rendering</h1>
    <p v-if="toggle">If condition</p>
    <p v-else>Else condition</p>
    <button @click="toggle= !toggle" >toggle</button>


</template>
<script>
export default{
    name: 'ConditionalRendering',
    data(){
        return{
            toggle:true,
        }
    },
}
</script>
<style></style>