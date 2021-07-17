<template>

<section class="profile-section">
<img class="profleft" src="../assets/img/profright.svg"/>
<img class="profright" src="../assets/img/profleft.svg"/>
<div class="profile-content">

<div class="profile-top-row">
<!-- left avatar -->
<div class="avatar-left">
  <div class="mb-2">
    <b-avatar src="https://placekitten.com/300/300" size="6rem"></b-avatar>
    <b-button class="edit-avatar"><img class="editimg" src="../assets/icons/editavatar.svg"/><span>Edytuj zdjęcie</span></b-button>
  </div>

  </div>

  <div class="remove-right">
    <!-- Remove profile right -->
    
     <b-button id="btn-remove">Usuń konto</b-button>
    
    </div>  
   
</div>


<form class="profile-data-row">
    
    <!-- User data -->
      <div class="prof-col">
      <h3>Dane użytkownika</h3>
      <!-- Name -->
      <label class="sr-only" for="inline-form-input-name">Imię</label>
       <b-form-input
       id="inline-form-input-name"
       class="mb-2 mr-sm-2 mb-sm-0"
       placeholder="Jane Doe"
    > </b-form-input>

   <!-- E-mail -->
   <label class="sr-only" for="inline-form-input-name">E-mail</label>
     
  <div class="mail-lock">
      <b-form-input
        id="input-group-1"
        label="Email address:"
        label-for="input-1"
        description="We'll never share your email with anyone else.">
      </b-form-input>
           <img class="mail1-icon" src="../assets/icons/lock.svg"/>     
     </div>
       </div>

     <!-- Additional info  -->
       <div class="prof-col">
       <h3>Dodatkowe informacje</h3>
       <!-- Date -->
       <label class="sr-only" for="inline-form-input-name">Data urodzenia</label>
       <b-form-datepicker v-model="value" :min="min" :max="max" locale="en"></b-form-datepicker>
  
       <!-- About me -->
       <label class="txtarea sr-only" for="inline-form-input-name">Coś o sobie…</label>
        <b-form-textarea
        id="textarea"
        v-model="text"
        placeholder="Enter something..."
        rows="3"
        max-rows="6"
    ></b-form-textarea>
<!-- Add button -->

<b-button id="btn-big">Zapisz zmiany</b-button>
       </div>

<!-- Change password -->
      <div class="prof-col">
      <h3>Zmiana hasła</h3>
     <!-- Password -->
     <label for="text-password">Obecne hasło</label>
     <div class="input-eyepass">
     <b-form-input type="password" id="text-password" aria-describedby="password-help-block"></b-form-input>
     <img class="password1-icon" src="../assets/icons/eye.svg"/>     
     </div>
     <!-- Password repeat -->
     <label for="text-password">Nowe hasło</label>
     <b-form-input type="password" id="text-password" aria-describedby="password-help-block"></b-form-input>

    <!-- Add button -->
      <b-button id="btn-change">Zmień hasło</b-button>
       
 
       </div>

   </form>
   
  

</div>




</section>

</template>

<script>
  require('@/assets/css/profile/profile.scss') 
  export default {
    name: 'Profile',
  }
</script> 
