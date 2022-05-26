<script setup>

// import {ref} from "vue";
import logo_footer from "@/assets/img/logo_footer.png"

// const icons = ref([
//   'mdi-facebook',
//   'mdi-twitter',
//   'mdi-linkedin',
//   'mdi-instagram',
// ]);

</script>

<template>
  <div style="background:#272727;">
    <v-container style="max-width: 1200px">
      <v-footer class="wrap_footer" style="background:#272727;">
        <div>
          <div class="d-flex">
            <a href="">
              <v-img class="footer_img-size mr-6" :src="logo_footer"></v-img>
            </a>
            <p class="style_text-footer text_wrap">легендарные ножи,<br>создающие шедевры</p>
          </div>
          <p class="style_text-footer mt-6">Компания «Tuotown» – эксклюзивный представитель <br> профессиональных
            кухонных
            ножей, изготовленных
            <br> лучшими
            мастерами Восточной Азии сприменением <br> передового европейского оборудования <br> исовременных
            материалов. </p>
          <p class="style_text-footer mt-6">Ониотличаются идеальным балансом <br>ифантастической остротой. Сочетают
            всебе
            вековые
            <br>традиции иновейшие
            разработки. <br>Такжепредлагаем широкий ассортимент <br> сопутствующих товаров.</p>
        </div>
        <div class="ml-11">
          <div>
            <h2 class="title_footer-text"><a href="">Информация</a></h2>
            <ul class="list_footer d-flex justify-space-between">
              <li class="item_footer"><a href="" class="link_item">Главная</a></li>
              <li class="item_footer"><a href="" class="link_item">Новости</a></li>
              <li class="item_footer"><a href="" class="link_item">О компании</a></li>
              <li class="item_footer"><a href="" class="link_item">Контакты</a></li>
            </ul>
          </div>
          <div>
            <h2 class="title_footer-text mt-9"><a href="">Каталог</a></h2>
            <ul class="list_footer d-flex">
              <li class="item_footer pr-3"><a href="" class="link_item">Кухонные ножи</a></li>
              <li class="item_footer pr-3"><a href="" class="link_item">Складные ножи</a></li>
              <li class="item_footer pr-3"><a href="" class="link_item">Точилки для ножей</a></li>
              <li class="item_footer"><a href="" class="link_item">Аксессуары</a></li>
            </ul>
          </div>
        </div>
        <div class="ml-16">
          <div>
            <h2 class="title_footer-text text_wrap"><a href="">Контактная информация</a></h2>
            <ul class="list_footer">
              <li class="item_footer mt-4 text-h6 text_wrap"><a href="" class="link_item telephone">+7(981)120-11-17</a>
              </li>
              <li class="item_footer mt-2"><a href="" class="link_item">tuotown@mail.ru</a></li>
              <li class="item_footer mt-7"><a href="" class="link_item">08:00-18:00, every day</a></li>
              <li class="item_footer mt-5"><a href="" class="link_item">Praha 1, Adress 123</a></li>
            </ul>
          </div>
        </div>
      </v-footer>
    </v-container>
  </div>
</template>

<style scoped lang="scss">
.wrap_footer {
  align-items: normal;
}

.footer_img-size {
  width: 194px;
}

.style_text-footer {
  font-size: 14px;
  color: white;
}

.list_footer {
  list-style-type: none;

  .link_item {
    color: white;
    opacity: 0.5;
    text-decoration: none;

    .telephone {
      color: white;
      opacity: 1;
    }

    &:hover {
      color: #C80000;
      opacity: 1;
    }
  }
}

.title_footer-text {
  font-size: 14px;
  margin-bottom: 14px;

  a {
    color: white;
    text-decoration: none;
  }
}

.text_wrap {
  white-space: nowrap;
}


</style>