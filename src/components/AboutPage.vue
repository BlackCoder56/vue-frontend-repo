<template>
   <section id="about" class="section about-section">
    <div class="about-content">
      <h2>About Us</h2>
      <div class="about-container">
        <div class="about-item">
          <img src="@/assets/politics.jpeg" alt="Service 1">
          <div class="about-text">
            <h3>Service 1</h3>
            <p>We offer comprehensive environmental education programs tailored for young people.</p>
          </div>
        </div>
        <div class="about-item">       
          <div class="about-text">
            <h3>Service 2</h3>
            <p>Our team conducts community outreach and conservation initiatives to promote sustainability.</p>
          </div>
          <img src="@/assets/politics.jpeg" alt="Service 2">
        </div>
        <div class="about-item">
          <img src="@/assets/politics.jpeg" alt="Service 3">
          <div class="about-text">
            <h3>Service 3</h3>
            <p>We provide resources and tools to help individuals and organizations reduce their environmental impact.</p>
          </div>
        </div>
      </div>
  </div>
  </section>
  </template>

<script>
    export default{
        name: 'AboutPage'
    };
</script>

<style scoped>
.section {
  padding: 50px 20px;   
  min-height: 100vh;
}
.about-content{
  /* width: 90%; */
  /* max-width: 1000px;     */
  margin: 0 auto;
}
h2{
  text-align: center;
}
about-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}
.about-item {
  display: flex;
  margin: 20px auto;
  align-items: center;
  background: white;
  border: 1px solid #ddd; 
  padding-left: 10px;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  max-width: 900px;    
}
.about-item img {
  width: 250px;
  height: 200px;
  border-radius: 4px;
  /* margin-right: 20px; */
  margin: 20px;  
}
.about-text {
  flex: 1;
  margin:20px;
}
.about-text h3 {
  margin-bottom: 10px;
  font-size: 22px;
  color: #008080;
}
.about-text p {
  font-size: 16px;
  color: #333;
}

@media (max-width: 768px) {
  .about-item {  
    margin-top:10px;
    display: flex;
    flex-direction: column;

  }  
  .about-item img {
  width: 90%;
  height: auto;
  border-radius: 4px;  
  margin-bottom: 10px;
}
.about-text {
  flex: 1;
  margin:10px 20px;
}
.about-text p {
  font-size: 14px;
}
.about-text h3 {
  margin-top: 10px;
  font-size: 18px;
  color: #008080;
}

}

</style>