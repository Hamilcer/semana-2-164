<template>
  <div id="app">
  <div class="container-fluid">
    <api-section></api-section>
  </div>
  </div>
</template>

<script>

import ApiSection from './components/ApiSection.vue';


export default {
  name: 'App',
  components:{
    ApiSection
  }
  
}
</script>

