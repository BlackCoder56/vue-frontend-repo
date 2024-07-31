<template>
  <div id="app">
    <NavbarPage />
    <div class="content">
      <HomePage />
      <AboutPage />
      <ContactPage />
        <!-- <router-view /> -->
    </div>    
    <FooterPage />
  </div>  
</template>

<script>
  import NavbarPage from './components/NavbarPage.vue';
  import HomePage from './components/HomePage.vue';
  import AboutPage from './components/AboutPage.vue';
  import ContactPage from './components/ContactPage.vue';
  import FooterPage from './components/footerPage.vue';
  
  export default {
    name: 'App',
    components: {
      NavbarPage,      
      FooterPage,
      HomePage,
      AboutPage,
      ContactPage
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
  margin: 0; /* Ensure there is no extra margin */
  padding: 0; /* Ensure there is no extra padding */
}
html {
  scroll-behavior: smooth;
}
</style>
