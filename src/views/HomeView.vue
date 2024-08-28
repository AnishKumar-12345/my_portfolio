<template>
  <Navbar />
<Homesection />
<AboutsectionVue style="background-color: #f5f5f5;"/>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import Navbar from '../components/Navbar.vue';
import Homesection from '../components/Homesection.vue'
import AboutsectionVue from '@/components/Aboutsection.vue';

export default defineComponent({
  name: 'HomeView',

  components: {
    Navbar,
    Homesection,
    AboutsectionVue,
  },
});
</script>
<style scoped>
/* Navbar {
  margin-bottom: 0px; 
  border: 1px solid red;
} */

/* Alternatively, you can add margin or padding to the Homesection component */
/* Homesection {
  margin-top: 10px; 
  

} */
</style>
