<template>
  <div id="app">
  <banner-carousel></banner-carousel>
  <section-footer></section-footer>
  </div>
</template>

<script>

import BannerCarousel from './components/BannerCarousel.vue';

import SectionFooter from './components/SectionFooter.vue';

export default {
  name: 'App',
  components: {
    BannerCarousel,
    SectionFooter
  },
  }
</script>
