<template>

  <body id="app">
       <HeaderFlow/>

      <section class="flow-container">
        <div class="flow-row">
          
        <Blog/>
      
          </div>
        </section>
       <FooterFlow/>
  
  
  </body>

</template>


<script>
import Vue from 'vue'
import HeaderFlow from './components/HeaderFlow.vue'

/*
import Hero from './components/Hero.vue'
import Products from './components/Products.vue'

 import Popup from './components/Popup.vue' */
/*import Contact from './components/Contact.vue' */

import Blog from './components/Blog.vue'



import FooterFlow from './components/FooterFlow.vue'
/* Bootstrap load */
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

/* Popper load */
/* import { createPopper } from '@popperjs/core'; */

// Make BootstrapVue available throughout your project
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)




require('@/assets/css/styles.scss') 
export default {
  name: 'App',
  components: {
     HeaderFlow,
     Blog,
     FooterFlow,
 
    }
   
  }



</script>


