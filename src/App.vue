<template>
  <div id="app">
    <h1>{{ message }}</h1>
    <button @click="reverseMessage">Reverse Message</button>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      message: '这是实验二的效果图'
    }
  },
  methods: {
    reverseMessage() {
      this.message = this.message.split('').reverse().join('');
    }
  }
}
</script>

<style>
#app {
  text-align: center;
  margin-top: 60px;
}
</style>
