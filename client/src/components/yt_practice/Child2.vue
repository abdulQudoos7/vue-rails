<template>
<div class="Child2Div">
  <p>User Name => <span class="user">{{user.name}}</span> And User Email => <span class="user">{{user.email}}</span></p>
  <button v-on:click="getAlert(user.name)">Click Me</button>
</div>
</template>

<script>
export default {
  name: "Child2",
  props:{
    user: Object,
    getAlert: Function,
  },
}
</script>

<style scoped>
.user{
  color: #358eff;
}
.Child2Div{
  display:flex
}
.Child2Div button{
  margin-left: 10px;
  margin-bottom: 10px;
}
</style>