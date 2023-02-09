<template>
    <h1>Parent Component</h1>
    <Child text="text form parent component" :user="user" :sendData="sendData" />
</template>
<script >
import Child from './Child.vue';

export default{
    name: "Parent",
    components: { Child },
    data(){
        return{
            user:{name:'Abdul Qudoos', email: 'abdulqudoos@test.com'}
        }
    },
    methods: {
        sendData(a,b){
            console.log(a+b);
        }
    }
}
</script>
<style></style>