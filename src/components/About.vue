<template>
  <v-container>
    <v-row>
      <v-col>
        <v-img :src="farmImage" class="mb-5"></v-img>
        <h1>About Our Farm</h1>
        <p>Our farm is a haven of sustainability and natural beauty. We specialize in dairy farming, organic farming, and poultry. Our commitment is to provide fresh, high-quality products while preserving the environment.</p>
      </v-col>
    </v-row>
    <Footer />
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      farmImage: require('../assets/photo4.jpg'),
    };
  },
};
</script>
