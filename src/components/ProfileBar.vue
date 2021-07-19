<template>

<section class="profile-bar-section">
     <img class="profleft" src="../assets/img/profright.svg"/>
     <img class="profright" src="../assets/img/profleft.svg"/> 
    

    <a href="#" class="edit-btn"><img src="../assets/icons/edit.svg"/>Edytuj konto</a>
     <div class="profile-bar">

     <!-- Left side -->
         <div class="bar-left">
            <b-avatar src="https://placekitten.com/300/300" size="6rem"></b-avatar>
            <div class="prof-info">
                <h2>Karolina</h2>
                <div class="prof-info-row">
                <!-- Age -->    
                    <div class="info-line">
                        <img src="../assets/icons/birthdate.svg"/>
                        <span>30 lat</span>
                    </div>
                 <!-- Location -->
                     <div class="info-line">
                        <img src="../assets/icons/location.svg"/>
                           <span>Warszawa</span>
                    </div>

             <!-- Liked products -->
                     <div class="info-line">
                        <img src="../assets/icons/like.svg"/>
                         <span>Moja szafa (8)</span>
                    </div>
                </div>
            </div>
         </div>

      <!-- Right side -->
       <div class="bar-right">
           <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea</p>
 
       </div>

     </div>


</section>

</template>
<script>

 
  require('@/assets/css/profile/profile.scss') 
export default {
    name: 'ProfileBar',
   
}
</script>


