<template>

  <div id="team" class="car text-white bg-dark">
    <div class="d-flex justify-content-center p-2">
        <img :src="member.image" alt="Imagen del miembro" class="img rounded-top"/>
    </div>
    <div class ="card-body">
    <h3 class="text-center">{{ member.nombre }}</h3>
    <p>{{member.codigo}}->{{ member.descripcion }}</p>
    </div>
    <div class="card-footer">
    <small class="text-muted">{{ member.rol }}</small>
    </div>
  </div>


</template>

<script>
export default {
  name: "TeamCard",
  props: ["member"],
};
</script>

<style scoped>

div {
    width: 262.4px;
}
div:hover {
    transition: all 0.10s ease-in-out 0s;
    zoom: 100.2%;
    box-shadow: rgba(0, 0, 0, 0.15) 2px 4px 25px 4px;
}
h3 {
    padding: 10px;
}
p {
    padding: 5px;
}
.ml-2 {
    color: white;
}

</style>
