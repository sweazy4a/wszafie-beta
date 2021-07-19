

<template>

<header id="navigation">
  <!-- Left side -->

    <b-navbar toggleable="lg" type="dark" variant="info">
    <div class="left-side">
    <b-navbar-brand class="logo" href="#"><img src="../assets/img/logo.png"/></b-navbar-brand>
   </div>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
     <!-- Mid side --> 
     <div class="mid-side">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Jaki produkt sprawi Ci dziś przyjemność?"></b-form-input>
          <b-button id="search-btn" size="sm" class="my-2 my-sm-0" type="submit"><img src="../assets/icons/search.svg"/></b-button>
        </b-nav-form>
       </div>

<!-- Right side -->
  <div class="right-side">
      <b-navbar-nav>
        <b-nav-item href="#">Produkty</b-nav-item>
        <b-nav-item href="#">Blog</b-nav-item>
        <b-nav-item href="#">O nas</b-nav-item>
        <b-nav-item href="#">Kontakt</b-nav-item>
        <b-button v-b-modal.modal-1 id="btn-register">Zaloguj/Zarejestruj</b-button>


      </b-navbar-nav>

      <!-- Right aligned nav items -->
   
      <div class="socials">
       <a class="social-ic" href="#facebook" target="_blank"><img alt="facebook" src="../assets/icons/face.svg"/></a>
       <a class="social-ic" href="#instagram" target="_blank"><img alt="instagram" src="../assets/icons/insta.svg"/></a>
       <a class="social-ic" href="#pinterest" target="_blank"><img alt="pinterest" src="../assets/icons/pint.svg"/></a> 
   </div>

</div>
    </b-collapse>
    
  </b-navbar>

</header>

</template>


<script>
require('@/assets/css/header.scss') 
export default {
  name: 'HeaderFlow',
  
}


</script>