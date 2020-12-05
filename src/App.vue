<template>
  <div id="app" class="container d-flex justify-content-between mt-5">

    <div v-for="(item, index) of member" :key="index">
      <TeamCard v-bind:member="item"></TeamCard>
    </div>
    

  </div>
</template>

<script>

import TeamCard from './components/TeamCard.vue'
export default {
  name: 'App',
  components: {
    TeamCard
  },
  data() {
    return{
      member: [
      {
        codigo: 1,
        nombre: 'Camilo Andrés Cipagauta',
        descripcion: 'Estudiante de la Universidad Distrital Francisco José de Caldas, Bogotá-Colombia. ',
        rol: 'Desarrollador Backend',
        image: './img/camilo.png'
      },
      {
        codigo: 2,
        nombre: 'Juan David Gonzáles',
        descripcion: 'Estudiante de Ingeniería Informática Universidad Autónoma de Occidente, 21 años, Cali- Colombia.',
        rol: 'Desarrollador Backend- Tester',
        image: './img/juan.png'
      },
      {
        codigo: 3,
        nombre: 'Hamilton Camilo Espitia',
        descripcion: 'Estudiante Desarrollo de software Misión TIC 2022 - UTP, 18 años, Bogotá-Colombia.',
        rol: 'Desarrollador Frontend',
        image: './img/hamilton.png' 
      },
      {
        codigo: 4,
        nombre: 'Angie Carolina Bonilla',
        descripcion: 'Ingeniera industrial de la universidad distrital, 23 años, Bogotá-Colombia.',
        rol: 'Desarrollador Frontend',
        image: './img/angie.png'
      },

      ]
    }
  }
}
</script>

<style>
#app {
  display: flex;
}
</style>

