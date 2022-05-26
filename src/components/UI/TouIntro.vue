<script setup>
import first_knife from "@/assets/img/firts_knife.svg"
import second_knife from "@/assets/img/second_knife.svg"
import three_knife from "@/assets/img/three_knife.svg"
import four_knife from "@/assets/img/four_knife.svg"
import img_knife from "@/assets/img/img_knife-intro.png"
import img_knife_second from "@/assets/img/img_knife_intro-second.png"
import biger_img_intro_first from "@/assets/img/biger_img_intro_first.png"
import biger_img_intro_second from "@/assets/img/biger_img_intro_second.png"
import biger_img_intro_three from "@/assets/img/biger_img_intro_three.png"

</script>

<template>
  <div style="background: #373737;" class="pt-15">
    <v-container style="max-width: 1200px">
      <div class="d-flex justify-space-around">
        <div class="d-flex flex-column align-center">
          <v-img :src="first_knife" class="img_style"></v-img>
          <a href="" class="link_item"><p class="description">Кухонные ножи</p></a>
        </div>
        <div class="d-flex flex-column align-center">
          <v-img :src="second_knife" class="img_style"></v-img>
          <a href="" class="link_item"><p class="description">Складные ножи</p></a>
        </div>
        <div class="d-flex flex-column align-center">
          <v-img :src="three_knife" class="img_style"></v-img>
          <a href="" class="link_item"><p class="description">Точилки для ножей</p></a>
        </div>
        <div class="d-flex flex-column align-center">
          <v-img :src="four_knife" class="img_style"></v-img>
          <a href="" class="link_item"><p class="description">Аксессуары для кухни</p></a>
        </div>
      </div>
      <div class="d-flex mb-10">
        <v-img :src="img_knife" class="size_img"></v-img>
        <div class="" style="margin-left: 80px;">
          <h2 class="text_title text mb-13">«Tuotown» – легендарные ножи, создающие шедевры</h2>
          <p class="text_intro text">Компания «Tuotown» – эксклюзивный представитель профессиональных кухонных ножей,
            изготовленных лучшими мастерами Восточной Азии с применением передового европейского оборудования и
            современных материалов. Они отличаются идеальным балансом и фантастической остротой. Сочетают в себе вековые
            традиции и новейшие разработки. Также предлагаем широкий ассортимент сопутствующих товаров.</p>
        </div>
      </div>
      <div class="d-flex">
        <div style="margin-right: 85px; ">
          <p class="text_intro text mb-7">Истинная красота ножа— совершённая функциональность ивизуальная гармония. Этот
            предмет издревле сопутствовал человеку: отзари цивилизации досегодняшних дней. Напротяжении всей истории
            человечества онбыл верным помощником, незаменимым инструментом игрозным оружием. Предлагаем изделия Hi-end
            качества подоступным ценам настоящим ценителям японских ножей.</p>
          <p class="text_intro text">Отличительной чертой нашего интернет-магазина являются уникальные торговые
            предложения, эксклюзивность продукции, неизменно высокое качество ивыгодные цены. Осуществляем продажи
            элитных японских кухонных ножей дляпрофессионалов илюбителей. Вобширной ассортиментной линейке представлены
            изделия дляразличных потребностей илюбого бюджета— отстоловых приборов дошеф-ножей.</p>
          <h2 class="text_title text mt-11">Ножи «Tuotown» – это главный инструмент поваров исекрет кулинарного
            мастерства</h2>
        </div>
        <v-img :src="img_knife_second" class="size_img"></v-img>
      </div>
    </v-container>
    <v-container fluid class="line-fluid"></v-container>
    <v-container style="max-width: 1200px">
      <h2 class="text_title text mb-9 mt-11">Всё самое интерестное о ножах</h2>
      <div class="d-flex pb-8">
        <v-hover v-slot="{ isHovering, props }">
          <v-card
              class="mx-auto"
              color="grey-lighten-4"
              max-width="380"
              v-bind="props"
          >
            <v-img
                class="align-end text-white overflow-hidden scaled-img"
                cover
                :src="biger_img_intro_first"
            >
              <v-card-title>
                <p>Традиционные виды японских кухонных ножей</p>
              </v-card-title>
              <v-expand-transition>
                <div
                    v-if="isHovering"
                    class="d-flex transition-fast-in-fast-out bg-red-accent-4 v-card--reveal text-h6 text-white"
                    style="height: 20%; border-bottom-right-radius: 7px;border-bottom-left-radius: 7px;"
                >
                  <p class="ml-5">Всемирная история режущих клинков — взгляд в прошлое</p>
                </div>
              </v-expand-transition>
            </v-img>
          </v-card>
        </v-hover>
        <v-hover v-slot="{ isHovering, props }">
          <v-card
              class="mx-auto"
              color="grey-lighten-4"
              max-width="380"
              v-bind="props"
          >
            <v-img
                class="align-end text-white overflow-hidden scaled-img"
                cover
                :src="biger_img_intro_second"
            >
              <v-card-title>
                <p>Традиционные виды японских кухонных ножей</p>
              </v-card-title>
              <v-expand-transition>
                <div
                    v-if="isHovering"
                    class="d-flex transition-fast-in-fast-out bg-red-accent-4 v-card--reveal text-h6 text-white"
                    style="height: 20%; border-bottom-right-radius: 7px;border-bottom-left-radius: 7px;"
                >
                  <p class="ml-5">Традиционные виды японских кухонных ножей</p>
                </div>
              </v-expand-transition>
            </v-img>
          </v-card>
        </v-hover>
        <v-hover v-slot="{ isHovering, props }">
          <v-card
              class="mx-auto"
              color="grey-lighten-4"
              max-width="380"
              v-bind="props"
          >
            <v-img
                class="align-end text-white overflow-hidden scaled-img"
                cover
                :src="biger_img_intro_three"
            >
              <v-card-title>
                <p>Как ухаживать за японскими кухонными ножами?</p>
              </v-card-title>
              <v-expand-transition>
                <div
                    v-if="isHovering"
                    class="d-flex transition-fast-in-fast-out bg-red-accent-4 v-card--reveal text-h6 text-white"
                    style="height: 20%; border-bottom-right-radius: 7px;border-bottom-left-radius: 7px;"
                >
                  <p class="ml-5">Как ухаживать за японскими кухонными ножами?</p>
                </div>
              </v-expand-transition>
            </v-img>
          </v-card>
        </v-hover>
      </div>
    </v-container>
  </div>
</template>

<style scoped lang="scss">
.img_style {
  width: 46px;
  height: 46px;
}

.scaled-img {
  ::v-deep(img) {
    transform: scale(1.015);
  }
}

.link_item {
  text-decoration: none;
  color: #ADACAC;
  padding-top: 30px;
  margin-bottom: 60px;

  &:hover {
    color: #C80000;
  }
}

.line-fluid {
  border-bottom: 1px solid #FFFFFF;
}

.size_img {
  width: 300px;
}

.text {
  color: #ADACAC;
  line-height: 22px;
}

h2.text {
  font-size: 35px;
  line-height: 42px;
}

.v-card--reveal {
  align-items: center;
  bottom: 0;
  justify-content: center;
  opacity: 1;
  position: absolute;
  width: 100%;
}
</style>