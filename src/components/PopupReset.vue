<template>

<section class="popup-section">
 <b-button v-b-modal.modal-3 id="btn-register">Zaloguj/Zarejestruj</b-button>
    <b-modal class="popup" id="modal-3" >
    
    <div class="popup-content"> 

     <div class="reset-section">
      <div class="reset-top">
       <h2>Przypominanie hasła</h2>
       <p>Jednak pamiętam!<a href="#">Wróć do logowania</a></p>
    </div>

    <div class="reset-row">
       <b-form-input
        id="input-group-1"
        placeholder="E-mail"
        label="Email address:"
        label-for="input-1"
        description="We'll never share your email with anyone else.">
      </b-form-input>

     <b-button id="btn-reset" class="btn-reset" variant="primary">Zresetuj hasło</b-button>
</div>



  </div>


      </div>
  </b-modal>
</section>

</template>

<script>
  require('@/assets/css/forms/popup.scss') 
  export default {
    name: 'PopupReset',
  }
</script> 
