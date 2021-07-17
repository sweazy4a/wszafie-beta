<template>

<section class="contact-section">

<div class="contact-row">

  <div class="contact-left">

  <div class="contact-top-txt">
    <h1>Masz pytanie?</h1>
    <p>Napisz do nas </p>
    <p>lub wypełnij formularz!</p> 
  </div>
   <a class="contactmail" href="mailto:redakcja@wszafie.pl"><img class="contact-img" alt="contact image" src="../assets/img/contact/contact.svg"/></a> 
  </div>
 
  <div class="contact-right">
  <!-- Name -->
  <b-form inline>
    <label class="sr-only" for="inline-form-input-name">Name</label>
    <b-form-input
      id="inline-form-input-name"
      class="mb-2 mr-sm-2 mb-sm-0"
      placeholder="Jane Doe"
    ></b-form-input>

  <!-- Email -->
  <label class="sr-only" for="inline-form-input-name">E-mail</label>
     <b-form-input
        id="input-group-1"
        label="Email address:"
        label-for="input-1"
        description="We'll never share your email with anyone else.">
  </b-form-input>

  <!-- Phone -->
    <label class="sr-only" for="inline-form-input-name">Phone</label>
    <b-form-input
      id="inline-form-input-name"
      class="mb-2 mr-sm-2 mb-sm-0"
      placeholder="Phone"
    ></b-form-input>
    
    <!-- Textarea -->
   <label class="sr-only" for="inline-form-input-name">Wiadomość</label>
   <b-form-textarea
      id="textarea"
      v-model="text"
      placeholder="Enter something..."
      rows="3"
      max-rows="6"
    ></b-form-textarea>

<!-- Agreement -->

    <b-form-checkbox class="mb-2 mr-sm-2 mb-sm-0">Wyrażam zgodę na przetwarzanie moich danych osobowych przez firmę TwoGecko Sp. z o.o., ul. Powstańców Śląskich 20B, 01-381 Warszawa w celu świadczenia przez nią usług związanych z działaniami na rzecz serwisu wszafie.pl i innych projektów.
    </b-form-checkbox>
    
    <b-form-checkbox class="mb-2 mr-sm-2 mb-sm-0">Wyrażam zgodę na otrzymywanie e-maili niezbędnych do wykonywania wszelkich działań w serwisie wszafie.pl (e-maile zwiazane z rejestracją, logowaniem, oraz e-maile systemowe).</b-form-checkbox>
   
     <b-form-checkbox class="mb-2 mr-sm-2 mb-sm-0">Chcę, aby informowano mnie o najlepszych promocjach, aktualnościach i innych ciekawych ofertach, pochodzących od firmy TwoGecko Sp.z.o.o. i podmiotów z nią współpracujących. Wiem, że w każdej chwili mogę wypisać się z listy mailingowej nie ponosząc żadnych konsekwencji. Oświadczam, iż zapoznałem się i akceptuję regulamin oraz politykę prywatności wszafie.pl
</b-form-checkbox>

   
    <b-button id="btn-big" class="btn-contact" variant="primary">Wyślij</b-button>
  </b-form>



</div>

  </div>



</section>

</template>

<script>
  require('@/assets/css/forms/contact.scss') 
  export default {
    name: 'Contact',
  }
</script> 
