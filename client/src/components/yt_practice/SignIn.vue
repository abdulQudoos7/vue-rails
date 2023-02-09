<template>
    <h1>Sign In</h1>
    <input type="text" placeholder="Email" v-model="email"><br /><br />
    <input type="password" placeholder="Password" v-model="password"><br /><br />
    <button v-on:click="getData()" >submit</button>

</template>
<script>
export default{
    name: 'SignIn',
    data(){
        return{
            email: '',
            password: ''
        }
    },
    methods: {
        getData(){
            console.log( "values :" ,this.email, this.password );
        }
    }
}
</script>
<style>
</style>