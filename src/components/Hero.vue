<template>
<section id="hero">
  <div>
    <VueSlickCarousel :arrows="true" :dots="true">
      <div>
       <img src="../assets/img/home/hero.png"/>
       <div class="hero-content">
        <h1>A Twoja garderoba </br>jest gotowa na lato?</h1>
        <p>Zainspiruj się i stwórz wspaniałą stylizację razem <br>z Wszafie!</p>
        <p>Najlepsze wzory i kolory ubrań na lato <br> znajdziesz tylko w naszym poradniku!</p>
        <b-button class="hero-btn">Pobierz poradnik</b-button>
        </div>
      </div>
      <div>2</div>
      <div>3</div>
      <div>4</div>
    </VueSlickCarousel>
  </div>
  </section>
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  // optional style for arrows & dots
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
 
  export default {
    name: 'Hero',
    components: { VueSlickCarousel },
  }

  require('@/assets/css/homepage/home.scss') 
</script> 
