<template>
  <div id="app">
    <NavbarPage />
    <div class="content">
      <router-view />
    </div>    
    <FooterPage />
  </div>  
</template>

<script>
  import NavbarPage from './components/NavbarPage.vue';
  import FooterPage from './components/footerPage.vue';
  export default {
    name: 'App',
    components: {
      NavbarPage,
      FooterPage
    }
  };
</script>

<style>
  html, body, #app {
    height: 100%;
    margin: 0;
  }
  #app {
    min-height: 100vh;
   display: flex;
   flex-direction: column;
   font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;  
  color: #2c3e50;
  }
  .content {
  flex: 1;
  margin-bottom: 0;
}
</style>
