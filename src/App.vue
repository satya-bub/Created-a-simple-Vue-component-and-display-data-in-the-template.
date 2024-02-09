<template>
  <HelloGreetings />
</template>

<script>
import HelloGreetings from './components/HelloGreetings.vue';

export default {
  name: 'App',
  components: {
    HelloGreetings
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left ;
  color: #5085b9;
  margin-top: 60px;
}
</style>
