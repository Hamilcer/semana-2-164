<template>
  <div id="app">

    <banner-carousel></banner-carousel>

    <div class="container d-flex justify-content-between mt-5">
      <api-section></api-section>
    </div>

    <div class="container-fluid">
      <div class="row justify-content-center mb-5">
        <div class="col mt-5" v-for="(member, index) of member" :key="index">
          <team-card v-bind:member="member"></team-card>
        </div>
      </div>
    </div>

    <section-footer></section-footer>
  </div>
</template>

<script>
import ApiSection from "./components/ApiSection.vue";
import TeamCard from "./components/TeamCard.vue";
import BannerCarousel from './components/BannerCarousel.vue';
import SectionFooter from './components/SectionFooter.vue';

export default {
  name: "App",
  components: {
    BannerCarousel,
    ApiSection,
    TeamCard,
    SectionFooter
  },
  data() {
    return {
      member: [
        {
          codigo: 1,
          nombre: "Camilo Andrés Cipagauta",
          descripcion:
            "Estudiante de la Universidad Distrital Francisco José de Caldas, Bogotá-Colombia. ",
          rol: "Desarrollador Backend",
          image: "./img/camilo.png",
        },
        {
          codigo: 2,
          nombre: "Juan David González",
          descripcion:
            "Estudiante de Ingeniería Informática Universidad Autónoma de Occidente, 21 años, Cali- Colombia.",
          rol: "Desarrollador Backend- Tester",
          image: "./img/juan.png",
        },
        {
          codigo: 3,
          nombre: "Hamilton Camilo Espitia",
          descripcion:
            "Estudiante Desarrollo de software Misión TIC 2022 - UTP, 18 años, Bogotá-Colombia.",
          rol: "Desarrollador Frontend",
          image: "./img/hamilton.png",
        },
        {
          codigo: 4,
          nombre: "Angie Carolina Bonilla",
          descripcion:
            "Ingeniera industrial de la universidad distrital, 23 años, Bogotá-Colombia.",
          rol: "Desarrollador Frontend",
          image: "./img/angie.png",
        },
      ],
    };
  },
};
</script>

<style>

</style>