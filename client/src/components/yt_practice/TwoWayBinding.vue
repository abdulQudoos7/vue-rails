<template>
    <h1>Two Way Binding</h1>
    <input type="text" v-model="result">
    <h3>Result = > {{ result }}</h3>

</template>

<script>
export default{
    name: "TwoWayBinding",
    data(){
        return{
            result: '',
        }
    }
}
</script>