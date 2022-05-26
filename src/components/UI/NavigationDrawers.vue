<script setup>

import {ref, watch} from "vue";
import logo_nav from "@/assets/img/logo.png"
import logo_click from "@/assets/img/click_logo.svg"
import logo_map from "@/assets/img/map_logo.svg"
import TouCarousel from "@/components/UI/TouCarousel";
// import main_carousel from "@/assets/img/main_carousel.png"
// import header_open from "@/assets/img/header_open.png"

const drawer = ref(null);
const group = ref(null);
const items = ref([
  {
    title: 'Foo',
    value: 'foo',
  },
  {
    title: 'Bar',
    value: 'bar',
  },
  {
    title: 'Fizz',
    value: 'fizz',
  },
  {
    title: 'Buzz',
    value: 'buzz',
  },
  {
    title: 'Foo',
    value: 'foo',
  },
  {
    title: 'Bar',
    value: 'bar',
  },
  {
    title: 'Fizz',
    value: 'fizz',
  },
  {
    title: 'Buzz',
    value: 'buzz',
  },
])

watch(group, () => {
  drawer.value = false
});


</script>

<template>
  <v-navigation-drawer
      v-model="drawer"
      temporary
      style="width: 444px; background: rgba(33, 33, 33, 0.3)"
  >
    <v-list
        :items="items"
        style="background: rgba(33, 33, 33, 0.3)"
        class="list_style"
    ></v-list>
  </v-navigation-drawer>
  <v-app-bar
      prominent
      style="background: rgba(33, 33, 33, 0.8) "
  >
    <v-container style="max-width: 1200px" class="d-flex align-center">
      <v-app-bar-nav-icon variant="text" :icon="''" default @click.stop="drawer = !drawer" class="rounded-0">
        <v-img :src="logo_click"></v-img>
      </v-app-bar-nav-icon>

      <v-toolbar-title>
        <div class="wrap_title align-center">
          <a href="">
            <v-img class="logo_map" :src="logo_map"></v-img>
          </a>
          <a href="" class="phone_number">
            +420736555866
          </a>
          <a href="/">
            <v-img class="logo_nav" :src="logo_nav"></v-img>
          </a>
        </div>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn variant="text" icon="mdi-shopping-outline" style="color: white"></v-btn>

      <v-btn variant="text" icon="mdi-email-outline" style="color: white"></v-btn>

      <v-btn variant="text" icon="mdi-magnify" style="color: white"></v-btn>
    </v-container>
  </v-app-bar>
  <v-main style="background: linear-gradient(268.39deg, rgba(0, 0, 0, 0) 21.45%, #000000 85.16%); padding-top: 0;">
    <tou-carousel>
      2123
    </tou-carousel>
  </v-main>


</template>

<style scoped>
.v-container {
  padding: 0;
}
.v-toolbar-title {
  flex: 1 1 auto;
}


.logo_nav {
  width: 144px;
  height: 35px;
}

.logo_map {
  width: 23px;
  height: 23px;
}

.phone_number {

  color: white;
  text-decoration: none;
}

.wrap_title {
  display: flex;
  justify-content: space-around;
}
.list_style {
  color: white;
  padding-top: 115px;
}

</style>