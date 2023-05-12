<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-grey">Olá, tudo bem?</h1>
              <h1 class="text-white">Sou Julio Gouveia</h1>
              <span class="text-grey">Engenheiro de Software</span> <br />
              <v-btn tile dark class="mt-8 texto-roxo" variant="outlined">Fale comigo</v-btn>
            </div>
          </v-col>
          <v-col cols="2">
            <div style="position: absolute; z-index: 9999; bottom: 0; margin-left:auto; margin-right: auto; left: 0; right: 0; text-align: center;">
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="5"></v-col>
        </v-row>
      </div>
    </v-container>
  </v-app>
</template>

<script>
import { defineComponent } from 'vue';

// Component
import NavBar from '@/components/NavBar.vue';

export default defineComponent({
  name: 'HomeView',

  components: {
    NavBar
},
});
</script>
<style scoped>
.v-container {
  padding: 16px 0;
}
.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  widows: 100%;
  color: white;
}
.head::before {
  content: " ";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}
.head::after {
  content: " ";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}
.texto-roxo {
  color: #9c3fc5;
}
</style>