<template>
    <section id="contact" class="section">
            <ContactFormPage />      
    </section>
  </template>
  
  <script>
  import ContactFormPage from './ContactFormPage.vue';

  
  export default {
    name: 'ContactPage',
    components: {
        ContactFormPage
    }
  };
  </script>
  
  <style scoped>
  .section {
  padding: 50px 20px;
  min-height: 100vh;
}
    
</style>
  