<script setup>
import {ref} from "vue";
import main_carousel from "@/assets/img/main_carousel.png"

const items = ref([
  {
    src: main_carousel
  },
  {
    src: main_carousel
  },
  {
    src: main_carousel
  },
  {
    src: main_carousel
  }
])
</script>


<template>
  <div class="position-relative">
      <v-carousel height="auto">
        <v-carousel-item
            v-for="(item,i) in items"
            :key="i"
            :src="item.src"
            cover
        ></v-carousel-item>
      </v-carousel>
    <div class="c-caption position-absolute">
      <v-container style="max-width: 1200px;">
        <div class="d-flex flex-wrap align-center flex-column text-style">
          <div class="text_style-title text-white">
            Исключительное качество без компромиссов
          </div>
          <div class="text_style-intro text-white">
            Ножи «Tuotown» – это главный инструмент поваров и секрет кулинарного мастерства
          </div>
        </div>
        <div>
          <v-btn class="style_btn-about">More info</v-btn>
        </div>
      </v-container>
    </div>
  </div>
</template>


<style scoped lang="scss">


::v-deep(.v-window__controls) {
  align-items: end;
  z-index: 2;
}

.c-caption {
  left: 0;
  right: 0;
  top: 40%;
  transform: translate3d(0, -50%, 0);
}

.text-style {
  width: 600px;
}

.text_style-intro {
  font-size: 19px;
}

.text_style-title {
  font-size: 41px;
  font-weight: 300;
}

.style_btn-about {
  margin-top: 30px;
  background: linear-gradient(268.39deg, rgba(0, 0, 0, 0) 21.45%, #000000 85.16%);
  color: white;
  border: 2px solid #C80000;
  border-radius: 27px;
  padding: 25px;

  &:hover {
    background: #C80000;
  }
}

</style>