<template>
  <h1>Interpolation</h1>
  <p> calculate => {{ 10 + 10 }}</p>
  <p> Text => {{ text }}</p>
  <p> Function => {{ getName() }}</p>
  <p> Function with params (2 + 2) => {{ getSum(2,2) }}</p>

  <h3>Method</h3>
  <p> Method Phone => {{ getPhone() }}</p>
  <p> Method All Data => {{ allData() }}</p>
  <p> Get specific data All Data => {{ allData().name }}</p>
  <p> Get specific data All Data => {{ allData().email }}</p>

</template>
<script>
export default{
  name: "Interpolation",
  data() {
    return{
      text: "text",
      getName() {
        return "Abdul Qudoos"
      },
      getSum(a,b) {
        return a+b
      }
    }
  },
  methods: {
    getPhone() {
      return "111-111-1111"
    },
    allData() {
      return{
        name: this.getName(),
        email: "abdul.qudoos@test.com",

      }
    }
  }
}
</script>
<style></style>