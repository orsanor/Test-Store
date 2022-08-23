<template>
  <v-app>
    <v-card class="d-flex" height="5vw" color="#d5c7c1" elevation="0"> </v-card>
    <v-container>
      <v-row class="mt-12">
        <v-col cols="6">
          <v-carousel
            cycle
            hide-delimiter-background
            show-arrows-on-hover
          >
            <v-carousel-item v-for="(slide, i) in slides" :key="i">
              <v-sheet :color="colors[i]" height="100%">
                <v-row class="fill-height" align="center" justify="center">
                  <div class="text-h2">{{ slide }} Slide</div>
                </v-row>
              </v-sheet>
            </v-carousel-item>
          </v-carousel>
        </v-col>
        <v-col cols="6">
          <v-card
            width="700px"
            height="480px"
            color="#97a889"
            elevation="1"
          >
          </v-card>
        </v-col>
        </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      colors: [
        "indigo",
        "warning",
        "pink darken-2",
        "red lighten-1",
        "deep-purple accent-4",
      ],
      slides: ["First", "Second", "Third", "Fourth", "Fifth"],
    };
  },
};
</script>
