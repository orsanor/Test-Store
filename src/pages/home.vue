<template>
  <v-app>
      <v-card class="d-flex" height="5vw" color="#d5c7c1" elevation="0">
      </v-card>
    <v-container class="d-flex" sm="6" lg="6">
      <v-row class="justify-center mt-12">
        <v-col cols="6">
          <v-row class="justify-center mt-2">
            <v-img max-height="auto" max-width="55%" src="@/assets/ss.png">
            </v-img>
            <v-carousel
              max-width="auto"
              max-height="auto"
              class="rounded mt-5 pa-6"
              :show-arrows="false"
              hide-delimiter-background
            >
              <v-carousel-item
                v-for="(item, i) in items"
                :key="i"
                :src="item.src"
              ></v-carousel-item>
            </v-carousel>
          </v-row>
        </v-col>
      </v-row>
      <v-col cols="6" class="d-flex mt-16 justify-center">
        <v-row class="justify-center">
          <v-card
            width="700px"
            height="480px"
            class="mt-16 d-flex"
            color="#97a889"
            elevation="1"
          >
          </v-card>
        </v-row>
      </v-col>
    </v-container>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "https://static.stealthelook.com.br/wp-content/uploads/2021/05/guia-das-velas-aromaticas-para-cada-ambiente-de-casa-quarto-20210514183720.jpg",
        },
        {
          src: "https://d3ugyf2ht6aenh.cloudfront.net/stores/001/915/754/products/vela_aromatica_para_ambientes_aqua_1539_2_310f93104c9178fda691b107527611331-956ad4748acca12afc16425075659571-640-0.jpg",
        },
        {
          src: "https://static.stealthelook.com.br/wp-content/uploads/2021/05/guia-das-velas-aromaticas-para-cada-ambiente-de-casa-banheiro-20210514183635.jpg",
        },
        {
          src: "https://static.stealthelook.com.br/wp-content/uploads/2021/05/guia-das-velas-aromaticas-para-cada-ambiente-de-casa-sala-de-jantar-20210514183908.jpg",
        },
      ],
    };
  },
};
</script>
