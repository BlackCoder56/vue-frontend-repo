<template>
    <footer class="footer">
      <div class="footer-content">
        <p>&copy; {{ currentYear }} {{ developerName }}</p>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooterPage',
    data() {
      return {
        currentYear: new Date().getFullYear(),
        developerName: 'BlackCoder56'  // Replace with your name or developer's name
      };
    }
  };
  </script>
  
  <style scoped>
.footer {
  background-color: #008080; /* Deep teal color */
  color: white;
  padding: 5px; /* Reduced padding around the footer content */
  text-align: center;
  position: relative; /* Ensure it is positioned relative to the page content */
  width: 100%;
  margin-top: -20px; /* Reduce space above footer by applying negative margin */
  box-shadow: 0 -1px 5px rgba(0, 0, 0, 0.1);
}
.footer-content {
  font-size: 14px;
  justify-content: center;
}
</style>