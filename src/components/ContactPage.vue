<template>
    <div class="contact-page">
      <ContactFormPage />
    </div>
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
    .contact-page {
    display: flex;
    justify-content: center;
    align-items: center;
    height: calc(100vh - 100px); /* Adjust for navbar height */
    padding: 10px; /* Reduce padding to decrease space */
    background-color: #e0f7fa;
}
</style>
  