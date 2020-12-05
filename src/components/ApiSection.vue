<template>
  <div class="row mt-md-5 mt-sm-5 mt-xs-5">
    <div class="col-lg-6 col-xs-12" v-for="(note, index) of news" :key="index">
      <div class="d-flex justify-content-center align-items-center">
        <div class="p-3">
          <!--imagen de la noticia-->
          <img :src="note.image" alt="news picture" width="230em" height="180em">
        </div>

        <div class="p-2">
          <!--texto de la noticia-->
          <p><b>{{note.title}}</b></p>
          <p>
            {{note.content}}
          </p>
          
        </div>
      </div>
      <!--enlace de la noticia-->
      <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
        <a :href="note.url" class="btn btn-outline-info">Leer más</a>
      </div>
    </div>
  </div>
</template>



<script>
import axios from "axios";

export default {
  name: "ApiSection",
  data() {
    return {
      news: null,
    };
  },
  mounted() {
    axios
      .get(
        "https://gnews.io/api/v4/search?q=technology&lang=es&token=172218885b5db79e0a9c6819250a047e"
      )
      .then((response) => {
        this.news = response.data.articles.slice(5, 9);
        console.log(this.news);
      });
  },
};
</script>

