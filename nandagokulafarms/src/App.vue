<template>
  <v-app>
    <Navbar/>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
  components: {
    Navbar
  },
};
</script>

<style>
@import '~vuetify/dist/vuetify.min.css';

.background-image {
  background-image: url('@/assets/background.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>
