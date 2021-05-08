<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logop0.jpg">
    <carousel></carousel>
    <h1>E-Library</h1>


    <div></div>
    <b-container class="col-sm-4 col-xs-12 text-center">
    <p>Articles | Books</p>
    <p><a href="https://www.goodreads.com/genres/novels" class="citation__doi__link">https://www.goodreads.com/genres/novels</a></p>
    </b-container> 

    


    <b-container class="col-sm-4 col-xs-12 text-center">
    <p>Articles | Technologies</p>
    <p><a href="https://www.goodreads.com/genres/technology" class="citation__doi__link">https://www.goodreads.com/genres/technology</a></p>
    </b-container> 


     <b-container class="col-sm-4 col-xs-12 text-center">
     <p>Articles | Science</p>
     <p><a href="https://www.goodreads.com/genres/science" class="citation__doi__link">https://www.goodreads.com/genres/Science</a></p>
     </b-container> 

     <b-container class="col-sm-4 col-xs-12 text-center">
    <p>Articles | Arts</p>
    <p><a href="https://www.goodreads.com/genres/business" class="citation__doi__link">https://www.goodreads.com/genres/business</a></p>
    </b-container> 

     <b-container class="col-sm-4 col-xs-12 text-center">
    <p>Articles | Mangement</p>
    <p><a href="https://www.goodreads.com/genres/management" class="citation__doi__link">https://www.goodreads.com/genres/management</a></p>
    </b-container> 
    

    <b-container>
    <a class="" href="/About e-Library" title="About e-Library">About e-Library</a>
    </b-container> 
    <b-container>
    <a class="" href="/help" title="Help">Help</a>
    </b-container> 
    <b-container>
    <a class="" href="/contactus" title="Contact Us">Contact Us</a>   
    </b-container>
		

    <b-container  class="col-sm-4 col-xs-12 text-center">
    <p class="footer-content">© 2021 e-Library. All Rights Reserved</p>
    </b-container>
    <div>
    
    </div>
    

  </div>
</template>

<script>
// @ is an alias to /src
import Carousel from '../components/eLibraryCarousel';

export default {
  name: 'Home',
  components: {
    Carousel, 

    
  }
}
</script>

<style scoped>


</style>