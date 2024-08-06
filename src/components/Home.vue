<template>
  <v-container>
    <v-carousel class="background-image">
      <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src"></v-carousel-item>
    </v-carousel>
    <v-divider class="my-5"></v-divider>
    <v-row>
      <v-col>
        <h1>Welcome to Our Farm</h1>
        <p>Discover the beauty and bounty of our farm. We are dedicated to sustainable farming practices and providing the freshest products to our community.</p>
      </v-col>
    </v-row>
    <Footer />
  </v-container>
</template>

<script>
import Footer from './Footer.vue';

export default {
    components: { Footer },
  data() {
    return {
      items: [
        { src: require('../assets/photo1.jpg') },
        { src: require('../assets/photo2.jpg') },
        { src: require('../assets/photo3.jpg') },
        { src: require('../assets/photo4.jpg') },
      ],
    };
  },
};
</script>
