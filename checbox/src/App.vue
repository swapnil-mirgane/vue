<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <gender/>
  <loop/>
  <sele/>

</template>

<script>
import gender from './components/ChecBox.vue';
import loop from './components/loop.vue';
import sele from './components/Check.vue';
export default {
  name: 'App',
  components: {
    gender,
    loop,
    sele,
    
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
