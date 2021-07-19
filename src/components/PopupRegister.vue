<template>

<section class="popup-section">

 <b-button v-b-modal.modal-2 id="btn-register">Zaloguj/Zarejestruj</b-button>

    <b-modal class="popup" id="modal-2" >
    <div class="popup-content">
     <div class="pop-left">
      <h2>Rejestracja</h2>
      <p class="hasprofile">Masz już konto? <a href="#register"> Zaloguj się</a></p>
  
      <div class="button-row">
         <b-button class="btn-login btn-loginfb"><div class="btn-content"><img src="../assets/icons/fblogin.svg"/><span>Zarejestruj się przez Facebook</span></div></b-button>
         <b-button class="btn-login btn-loginfb"><div class="btn-content"><img src="../assets/icons/glogin.svg"/><span>Zarejestruj się przez Google</span></div></b-button>
      </div>

     <div class="alternative"><span>lub</span></div>

     <div class="form-block">
 
  <b-form-input
       id="inline-form-input-name"
       class="mb-2 mr-sm-2 mb-sm-0"
       placeholder="Jane Doe"
    > </b-form-input>



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

  
      <b-button id="btn-reglogin-action" variant="primary">Zaloguj się</b-button>
     </b-form>
   </div>

    <b-form-checkbox class="mb-2 mr-sm-2 mb-sm-0">Wyrażam zgodę na przetwarzanie moich danych osobowych przez firmę TwoGecko Sp. z o.o., ul. Powstańców Śląskich 20B, 01-381 Warszawa w celu świadczenia przez nią usług związanych z działaniami na rzecz serwisu wszafie.pl i innych projektów.
    </b-form-checkbox>


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
    name: 'PopupRegister',
  }
</script> 
