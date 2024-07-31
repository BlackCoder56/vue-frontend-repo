<template>
    <section id="home" class="section">
      <div class="hero">
      <h1>Welcome to Our Website</h1>
      <p>Discover our latest updates and stay informed.</p>
    </div>
    <div class="recent-updates">
      <h2>Recent Updates</h2>
      <div class="updates-container">
        <div class="update">          
          <div class="update-content">
            <img src="@/assets/trump-shooting.jpg" alt="Update 1">
            <div class="text-content">
              <h3>Update Title 1</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque imperdiet.</p>        
              <p>
                <i class="pub-dt">
                  Published: 29/07/2024
                </i>
              </p>     
            </div>            
          </div>
        </div>
        <div class="update hide-on-mobile">
          <div class="update-content">
            <img src="@/assets/trump-shooting.jpg" alt="Update 2">
            <div class="text-content">
              <h3>Update Title 2</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque imperdiet.</p>
              <p >
                <i class="pub-dt">
                  Published: 27/07/2024
                </i>
              </p>    
            </div>
          </div>
        </div>
        <div class="update hide-on-mobile">
          <div class="update-content">
            <img src="@/assets/trump-shooting.jpg" alt="Update 3">
            <div class="text-content">
              <h3>Update Title 3</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque imperdiet.</p>
              <p >
                <i class="pub-dt">
                  Published: 26/07/2024
                </i>
              </p>    
            </div>
          </div>
        </div>
        <div class="update hide-on-mobile">
          <div class="update-content">
            <img src="@/assets/trump-shooting.jpg" alt="Update 3">
            <div class="text-content">
              <h3>Update Title 4</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque imperdiet.</p>
              <p >
                <i class="pub-dt">
                  Published: 25/07/2024
                </i>
              </p>    
            </div>
          </div>
         </div>
      </div>
    </div>
  </section>
</template>

<script>
    export default {
        name: 'HomePage'
    };
</script>

<style scoped>
.section {
  padding: 50px 20px;
  min-height: 100vh;
}
.pub-dt{
  font-size: 15px;
  text-decoration: wavy;
}
.update img {
  width: 150px;
  height: auto;
  border-radius: 8px;
  
}
.update-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  /* background-color: blue;   */
}
.text-content {
  margin-left:20px;
  flex: 1;
}
.home-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}
.hero {
  background: linear-gradient(to right, #008080, #004d4d);
  color: white;
  padding: 50px 20px; 
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}
.hero h1 {
  margin-bottom: 20px;
  font-size: 36px;
}
.hero p {
  font-size: 18px;
  margin-bottom: 0;
}
.recent-updates {
  margin-top: 50px;
  width: 80%;
  /* max-width: 800px; */
}
.recent-updates h2 {
  font-size: 28px;
  margin-bottom: 30px;
}
.updates-container{    
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
}
.update {  
  background: white;
  border: 1px solid #ddd;
  padding-left:20px;
  margin-bottom: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}
.update h3 {
  margin-bottom: 10px;
  font-size: 22px;
  color: #008080;
}
.update p {
  font-size: 16px;
  color: #333;
}
@media (max-width: 768px) {
  .hero h1 {
    font-size: 28px;
  }
  .hero p {
    font-size: 16px;
  }
  .recent-updates h2 {
    font-size: 24px;
  }
  .update h3 {
    font-size: 20px;
  }
  .update p {
    font-size: 14px;
  }
  .recent-updates {
  margin-top: 50px;
  width: 100%;
  max-width: 800px;
}
  .updates-container {
    width:100%;
    grid-template-columns: 1fr;
  }
  .hide-on-mobile {
  display: none;
}
  
}
</style>