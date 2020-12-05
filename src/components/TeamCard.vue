<template>
  
    <div class="ml-2 mr-2 border borderlight rounded">
        <img v-if="member.image" :src="member.image" alt="Imagen del miembro" class="img rounded-top" >
        
            <h3 class="text-center" >{{ member.nombre }}</h3>
            <p> {{member.descripcion}} </p>
            <p> {{member.rol}} </p>
    </div>

</template>

<script>
    export default {
        name: 'TeamCard',
        props: ['member']
    }
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
    color: black;
}

</style>
