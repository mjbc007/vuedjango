<template>
  <div id="app">
    <List/>
  </div>
</template>

<script>
import List from './components/List'

export default {
  name: 'App',
  components: {
    List,
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
