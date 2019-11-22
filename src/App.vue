<template>
  <div id="app">
    <MainFrame />
  </div>
</template>

<script>
import MainFrame from "./views/MainFrame";
import Home from "./views/Home";
export default {
  components: {
    MainFrame,
    Home
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* width: 90%; */
  height: 100%;
  margin: 0 auto;
  min-width: 1500px;
  /* border: solid black 2px; */
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
