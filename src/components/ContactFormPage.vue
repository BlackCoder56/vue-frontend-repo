<template>
    <div class="contact-form">
      <h1>Contact Us</h1>
      <form @submit.prevent="submitForm">
        <div class="form-group">
          <label for="fullName">Full Name</label>
          <input type="text" id="fullName" v-model="form.fullName" required>
        </div>
        <div class="form-group">
          <label for="contactNumber">Contact Number</label>
          <input type="text" id="contactNumber" v-model="form.contactNumber" required>
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" v-model="form.email" required>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" v-model="form.message" rows="5" required></textarea>
        </div>
        <button type="submit">Submit</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ContactForm',
    data() {
      return {
        form: {
          fullName: '',
          contactNumber: '',
          email: '',
          message: ''
        }
      };
    },
    methods: {
      submitForm() {
        alert('Form submitted: ' + JSON.stringify(this.form));
        // Here you can handle the form submission, e.g., send the data to an API
        this.form.fullName = '';
        this.form.contactNumber = '';
        this.form.email = '';
        this.form.message = '';
      }
    }
  };
  </script>
  
  <style scoped>
  .contact-form {
    /* width: 90%; */
    max-width: 600px;
    margin: 0 auto;
    /* margin: 20px auto;
    padding: 20px;
    background-color: #f9f9f9;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); */
  }
  .contact-form h1 {
    text-align: center;
    margin-bottom: 20px;
  }

  .form-group {
    margin-bottom: 15px;    
  }
  .form-group label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
  }
  .form-group input,
  .form-group textarea {
    width: 100%;
    padding: 8px;
    margin-top: 3px;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  .form-group input:focus,
    .form-group textarea:focus {
    border-color: #008080; /* Deep teal color */
    box-shadow: 0 0 5px rgba(0, 128, 128, 0.5);
    color: #000000; /* Deep teal color for text */
    }
  .form-group textarea {
    resize: none;
  }
  button {
    display: block;
    width: 100%;
    padding: 10px 20px;
    background-color: #008080;
    color: white;
    border: none;
    border-radius: 4px;
    font-size: 16px;
    cursor: pointer;
  }
  button:hover {
    background-color: #006666;
  }
  </style>
  