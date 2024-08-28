<template>
  <div>
    <!-- App Bar for Desktop -->
    <v-app-bar :elevation="2" class="hidden-sm-and-down" style="height:15%">
      <!-- Desktop Logo and Title -->
      <v-app-bar-nav-icon style="margin:50px;margin-top:5%;">
        <v-img class="mr-3" src="../../src/assets/anishlogo.png" height="50px" width="50px" style="border-radius:55px"></v-img>
      </v-app-bar-nav-icon>
    
      <v-toolbar-title style="margin-left:-38px;margin-top:1.5%;font-weight: 600;font-size: 1rem;">ANISH KUMAR BEHERA</v-toolbar-title>
      <v-spacer></v-spacer>

      <!-- Desktop Navigation Buttons -->
      <v-toolbar-items style="margin-top:1%;margin-right:6%">
        <v-btn style="font-weight: 600;font-size: 0.9rem;" v-for="item in nav" :key="item" flat>{{ item.text }}</v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <!-- App Bar for Mobile -->
    <v-app-bar :elevation="2" class="hidden-md-and-up" style="position: fixed; top: 0; width: 100%;">
      <!-- Mobile Menu Toggle Button -->
      <!-- <v-app-bar-nav-icon @click="dialog = !dialog"></v-app-bar-nav-icon> -->
      <!-- <v-btn> -->
        <v-icon size="large" icon="mdi-format-list-bulleted"  @click="dialog = !dialog" style="margin-left:15px"></v-icon>
      <!-- </v-btn> -->
      <!-- Mobile Menu Dialog -->
      <v-dialog v-model="dialog" fullscreen hide-overlay transition="custom-dialog-transition">
        <v-app-bar dark style="position: fixed; top: 0; width: 100%;">
          <!-- <v-app-bar-nav-icon ></v-app-bar-nav-icon> -->
           <!-- <v-btn @click="dialog = false"> -->
        <v-icon size="large" icon="mdi-window-close" @click="dialog = false"  style="margin-left:15px"></v-icon>
      <!-- </v-btn> -->
          <v-toolbar-title >Mobile Menu</v-toolbar-title>
        </v-app-bar>

        <v-list style="margin-top: 60px;">
          <v-list-item v-for="(item, index) in nav" :key="index" :value="item" color="primary">
            <template v-slot:prepend>
              <v-icon :icon="item.icon"></v-icon>
            </template>
            <v-list-item-title v-text="item.text" ></v-list-item-title>
          </v-list-item>
        </v-list>
      </v-dialog>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () => ({
    dialog: false,
    nav: [
      { icon: 'home', text: 'Home', title: 'Back to Home page', active: true },
      { icon: 'info', text: 'About', title: 'About this demo', active: false },
      { icon: 'assignment_turned_in', text: 'Projects', title: 'Some stuff that needs doing', active: false },
      { icon: 'email', text: 'Contact', title: 'Our Contact info', active: false }
    ]
  })
}
</script>

<style scoped>
/* Add any additional styling if needed */
.custom-dialog-transition-enter-active,
.custom-dialog-transition-leave-active {
  transition: transform 0.5s;
}

.custom-dialog-transition-enter, .custom-dialog-transition-leave-to /* .custom-dialog-transition-leave-active in <2.1.8 */ {
  transform: translateX(0);
}

.custom-dialog-transition-enter-to {
  transform: translateX(-50%);
}
</style>
