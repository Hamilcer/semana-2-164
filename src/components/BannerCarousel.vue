<template>
<div>
 <top-menu></top-menu>
     <div id="newcarousel" class="carousel slide" data-ride="carousel">
            <ul class="carousel-indicators">
              <li data-target="#newcarousel" data-slide-to="0" class="active"></li>
              <li data-target="#newcarousel" data-slide-to="1"></li>
              <li data-target="#newcarousel" data-slide-to="2"></li>
            </ul>
            <div class="carousel-inner">
              <div class="carousel-item active">
                <img src="../assets/img/dominio.jpg" alt="" width=auto height=auto>
                <div class="carousel-caption"> 
                  <h4>Dominio Web</h4>
                  <p>Un servidor de dominio es aquel capaz de proporcionar un nombre o una identidad única en la Web.</p>                    
            <a class="btn btn-light" href="https://siaguanta.com/c-tecnologia/que-es-un-servidor-de-dominio/" role="button">Más información</a>
            </div>
              </div>
              <div class="carousel-item">
                <img src="../assets/img/hosting.jpg" alt="" width=auto height=auto>
                <div class="carousel-caption">
                  <h4>Servicio de Hosting</h4>
                  <p>Este servicio provee a los usuarios de Internet un sistema para poder almacenar información,
                    imágenes, vídeo, o cualquier contenido accesible vía web.</p>                      
                <a class="btn btn-light" href="https://es.wikipedia.org/wiki/Alojamiento_web" role="button">Más información</a>
                </div>  
              </div>
              <div class="carousel-item">
                <img src="../assets/img/servicioweb.jpg" alt="" width=auto height=auto>
                <div class="carousel-caption">
                  <h4>Servicio Web</h4>
                  <p>Los servicios web son aplicaciones autónomas modulares que se pueden describir, publicar, localizar e invocar a través de una red".</p>                      
                <a class="btn btn-light" href="https://www.ibm.com/support/knowledgecenter/es/SSAW57_9.0.5/com.ibm.websphere.nd.multiplatform.doc/ae/cwbs_wbs2.html" role="button">Más información</a>
                </div>   
              </div>
            </div>
            <a class="carousel-control-prev" href="#newcarousel" data-slide="prev">
              <span class="carousel-control-prev-icon"></span>
            </a>
            <a class="carousel-control-next" href="#newcarousel" data-slide="next">
              <span class="carousel-control-next-icon"></span>
            </a>
          </div>
         </div>
</template>


<script>
import TopMenu from './TopMenu..vue';
    export default {
        name: 'BannerCarousel',
        components: {
            TopMenu
        }
 };
</script>