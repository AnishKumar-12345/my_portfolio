<template>
  <v-app>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
}
</script>
<style scoped>
*{
  margin: 0px;
  padding: 0px;
  box-sizing: inherit;
  background-color: #fafafa;  
  font-family: inherit;
}
</style>
