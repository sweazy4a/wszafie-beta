<template>


<section class="popup-section">

 
    <b-modal class="popup" id="modal-1" >
    <div class="popup-content">
     <div class="pop-left">
      <h2>Logowanie</h2>
      <p class="hasprofile">Nie masz jeszcze konta? <a href="#register">Zarejestruj się</a></p>
  
      <div class="button-row">
         <b-button class="btn-login btn-loginfb"><div class="btn-content"><img src="../assets/icons/fblogin.svg"/><span>Zarejestruj się przez Facebook</span></div></b-button>
         <b-button class="btn-login btn-loginfb"><div class="btn-content"><img src="../assets/icons/glogin.svg"/><span>Zarejestruj się przez Google</span></div></b-button>
      </div>

     <div class="alternative"><span>lub</span></div>

     <div class="form-block">
 
       <b-form inline>
       <b-form-input
       id="inline-form-input-name popinput"
       class="mb-2 mr-sm-2 mb-sm-0"
       placeholder="E-mail">
       </b-form-input>
 
      <b-form @submit.stop.prevent>
       <b-form-input type="password" placeholder="Hasło" id="text-password popinput" aria-describedby="password-help-block"   ></b-form-input>
       
     </b-form>
   

 <!--   <b-form-checkbox class="mb-2 mr-sm-2 mb-sm-0">Remember me</b-form-checkbox> -->

      <div class="forgot-pass">
      <p>Zapomniałeś hasła? <a href="#reset">Zmień je tutaj</a></p>
      </div>
  
      <b-button id="btn-reglogin-action" variant="primary">Zaloguj się</b-button>
     </b-form>
   </div>

     </div>
 
    <div class="pop-right">   
      <div class="txt-pop">
       <h2>Wejdź do szafy i bądź na bieżąco!</h2>
       <p>- wszystko, co modne w jednym miejscu.</p>
       </div>
    </div>

    </div>

  </b-modal>

</section>

</template>

<script>
  require('@/assets/css/forms/popup.scss') 
  export default {
    name: 'Popup',
  }
</script> 
