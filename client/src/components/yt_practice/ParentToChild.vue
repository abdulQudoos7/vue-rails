<template>
  <h1>Parent2</h1>
  <ul>
    <li v-for="user in users" :key="user.name" >
<!--      {{user.name}}-->
      <Child2 :user="user" :getAlert="getAlert"/>

    </li>
  </ul>

  <!--  <h4>parent=>{{users.name}}</h4>-->

</template>

<script>
import Child2 from "./Child2.vue";

export default {
  name: "ParentToChild",
  components: {Child2},
  data() {
    return {
      users: [
        {name: "user1", email: "user1@gmail.com"},
        {name: "user2", email: "user2@gmail.com"},
        {name: "user3", email: "user3@gmail.com"},
        {name: "user4", email: "user4@gmail.com"},
        {name: "user8", email: "user8@gmail.com"},
        {name: "user7", email: "user7@gmail.com"},
        {name: "user6", email: "user6@gmail.com"},
        {name: "user5", email: "user5@gmail.com"},
      ]
    }
  },
  methods: {
    getAlert(name){
      alert("Hello "+name)
    }
  }
}
</script>

<style scoped>

</style>