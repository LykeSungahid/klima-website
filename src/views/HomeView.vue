<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <div class="home">
      <div class="container text-center">    
        <p>About Us</p>
      </div>
      <div id="myCarousel" class="carousel slide" data-ride="carousel">
        <!-- Indicators -->
        <ol class="carousel-indicators">
          <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#myCarousel" data-slide-to="1"></li>
          <li data-target="#myCarousel" data-slide-to="2"></li>
        </ol>
        
        <!-- Wrapper for slides -->
        <div class="carousel-inner" role="listbox">
          <div class="item active">
            <a id="logo" href="/about"><img src="@/assets/team1.jpg" alt="Image"></a>
            <div class="carousel-caption">
              <h3>Sell $</h3>
              <p>Money Money.</p>
            </div>      
          </div>

          <div class="item">
            <a id="logo" href="/about"><img src="@/assets/tools.jpg" alt="Image"></a>
            <div class="carousel-caption">
              <h3>More Sell $</h3>
              <p>Lorem ipsum...</p>
            </div>      
          </div>

          <div class="item">
            <a id="logo" href="/about"><img src="@/assets/tools2.jpg" alt="Image"></a>
            <div class="carousel-caption">
              <h3>More Sell $</h3>
              <p>Lorem ipsum...</p>
            </div>      
          </div>
        </div>

        <!-- Left and right controls -->
        <a class="left carousel-control" href="#myCarousel" role="button" data-slide="prev">
          <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a class="right carousel-control" href="#myCarousel" role="button" data-slide="next">
          <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
          <span class="sr-only">Next</span>
        </a>
      </div>

      <div class="container text-center">    
        <p>Our Services</p><br>
        <div class="row">
          <div class="col-sm-4">
            <a id="logo" href="/services"><img src="@/assets/installation.jpg" class="img-responsive" style="width:100%" alt="Image"></a>
            <h4>Installations</h4>
          </div>
          <div class="col-sm-4"> 
            <a id="logo" href="/services"><img src="@/assets/management.jpg" class="img-responsive" style="width:100%" alt="Image"></a>
            <h4>Project Design, Management and Estimates </h4>    
          </div>
          <div class="col-sm-4"> 
            <a id="logo" href="/services"><img src="@/assets/maintenance.jpg" class="img-responsive" style="width:100%" alt="Image"></a>
            <h4>Preventive Maintenance</h4>    
          </div>
          <div class="col-sm-4"> 
            <a id="logo" href="/services"><img src="@/assets/ventilation.jpg" class="img-responsive" style="width:100%" alt="Image"></a>
            <h4>Ventilation</h4>    
          </div>
          <div class="col-sm-4"> 
            <a id="logo" href="/services"><img src="@/assets/civilworks.jpg" class="img-responsive" style="width:100%" alt="Image"></a>
            <h4>Architectural and Civil Works</h4>    
          </div>
          <div class="col-sm-4"> 
            <a id="logo" href="/services"><img src="@/assets/mech.jpg" class="img-responsive" style="width:100%" alt="Image"></a>
            <h4>Other Mechanical - Related Works</h4>    
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
h4 {
  font-family: 'Courier New', Courier, monospace;
  margin-bottom: 30px;
  font-size: 14px;
  font-weight: bold;
}
p {
    font-weight: bold;
    font-family: 'Courier New', Courier, monospace;
}
#myCarousel {
  display: block;
  width: 65%;
  margin-left: auto;
  margin-right: auto;
  margin-top: 20px;
  margin-bottom: 50px;
}
.carousel-caption {
    display: none; 
}
.carousel-inner img {
    width: 100%; /* Set width to 100% */
    margin: auto;
    min-height: 200px;
}
@media (min-width: 1024px) {
  p {
    font-weight: bold;
    font-family: 'Courier New', Courier, monospace;
  }
  .carousel-inner img {
    width: 100%; /* Set width to 100% */
    margin: auto;
    min-height:200px;
  }
  .carousel-caption {
    display: none; 
  }
  .home {
    min-height: 10vh;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
  }
  body {
    display: flex;
    place-items: center;
  }
  #app {
    display: grid;
    grid-template-columns: 1fr;
    padding: 0 2rem;
  }
}
</style>