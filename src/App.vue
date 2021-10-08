<template>
  <div id="app">
    <headComponent />
    <hr>
    <button @click="destroyComponent">destroyComponent</button>
  </div>
</template>

<script>
import headComponent from './components/headComponent.vue'

export default {
  name: 'App',
  components: {
    headComponent
  },
  methods: {
    destroyComponent () {
      this.$destroy()
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
