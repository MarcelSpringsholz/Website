<template>
  <div class="home">
    <v-row align="center" justify="center">
      <v-container>
        <v-row align="center" justify="center">
          <h1 class="font-weight-black">About me</h1>
        </v-row>
        <v-row>
          <v-col cols="6">
            <v-img src="../../public/img/Profile.png" width="60%"></v-img>
          </v-col>

          <v-col cols="6">
            <i class="fas fa-quote-left"></i>
            <p>
              Ich bin Marcel Springsholz am 28.06.2001 in Wien geboren. Derzeit besuche ich die HTL-WienWest
              im 5. von 5 Jahren. Ich habe die Medientechnikwelt gewählt, da es mir schon immer Spaß gemacht hat Fotos und Videos zu machen. In
              meiner Ausbildung befasse ich mich mit den diversen Adobe Produkten wie Indesign, Photoshop, Premiere Pro und vielen Weiteren.
              Außerdem befasse ich mich mit Affinity Photo & Designer, Blender, Datenbanken und mehreren Programmiersprachen unter anderem C#,
              JavaScript, HTML, php, sql etc.
            </p>
            <i class="fas fa-quote-right"></i>
          </v-col>
        </v-row>
        <v-row>
          <v-carousel :show-arrows="false">
            <v-carousel-item
              v-for="(item,i) in items"
              :key="i"
              :src="item"
              reverse-transition="fade-transition"
              transition="fade-transition"
            ></v-carousel-item>
          </v-carousel>
        </v-row>
      </v-container>
    </v-row>
    <v-row align="center" justify="center">
      <v-col cols="10">
        <i class="fas fa-code"></i> Programmer
        <i class="fas fa-pen-fancy"></i> Designer
        <i class="fas fa-video"></i> Filmmaker
        <i class="fas fa-video"></i>
        Photographer
        <i class="fas fa-share-alt"></i>

        <i class="fab fa-instagram"></i>
        <i class="fab fa-youtube"></i>
        <i class="fas fa-envelope"></i>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        "Bilder",
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg"
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg"
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg"
        }
      ]
    };
  }
};
</script>

<style>
.backgroundimg {
  background-image: url("../../public/img/IMG_3595.jpg");
}
</style>