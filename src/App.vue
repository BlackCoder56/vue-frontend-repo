<template>
  <div id="app">
    <NavbarPage />
    <router-view/>
  </div>
  
</template>

<script>
  import NavbarPage from './components/NavbarPage.vue';

  export default {
    name: 'App',
    components: {
      NavbarPage
    }
  };
</script>

<style>
  html, body, #app {
    height: 100%;
    margin: 0;
  }
  #app {
   display: flex;
   flex-direction: column;
   font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;  
  color: #2c3e50;
  }
</style>
<!-- <style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style> -->
