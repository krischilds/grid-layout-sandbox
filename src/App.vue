<template>
  <div id="app" class="app-font">
    <GridLayout msg="Grid Layout" />
  </div>
</template>

<script>
import GridLayout from "./components/GridLayout.vue";

export default {
  name: "App",
  components: {
    GridLayout,
  },
};
</script>

<style>
body {
  border: 0;
  padding: 0;
  margin: 0;
  background: gray;
}

.app-font {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#app {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
}
</style>
