<template>
  <v-app>
    <v-app-bar 
      app 
      elevation="1" 
      class="pa-12" 
      color="#97a889" 
      elevate-on-scroll
      >
      <v-toolbar-title>
          <v-img  
          max-height="auto" 
          max-width="28%" 
          class="mb-16 mr-10" 
          src="@/assets/logo.png"
          >
        </v-img>
      </v-toolbar-title>
    </v-app-bar>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    menus: [
      { title: "Home", route: "home" },
      // { title: "Como cuidar do seu mimo" },
      { title: "Sobre", route: "sobre" },
    ],
  }),
};
</script>
<style>
#app {
      background-color: #fffdf6;
}
</style>
