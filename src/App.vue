<template>
  <div id="app">
    <p>Sever Status: {{  status }}</p>
    <hr>
    <button @click="changeStatus">Change Status</button>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      status: 'Critical'
    }
  },
  methods: {
    changeStatus () {
      this.status = 'Normal'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
