<template>
  <div id="app">
    <h1 class="tittle">modes</h1>
    <buttons :colors="colors">

    </buttons>
    <loader/>
  </div>
</template>

<script>
import buttons from "./components/buttons";
import loader from "./components/loader";

export default {
  name: 'App',
  data() {
    return {
      colors: [
          'red',
          'blue',
          'green',
          'yellow',
      ]
    };
  },
  components: {
    buttons, loader
  }
}
</script>

<style>
#app {
  font-family:Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

html {
  width: 100%;
  height: 100%;
  }

</style>
