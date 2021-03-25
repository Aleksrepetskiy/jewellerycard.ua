<template>
  <swiper class="swiper" :options="swiperOption">
    <swiper-slide
      ><a href="/ru/news#clasps">
        <img src="@/assets/img/news/zamki_400x400.jpg" alt="clasps" />
      </a>
      <div class="doing__content">
        <div class="doing__title">Новости</div>
        <a href="/ru/news#clasps"
          ><h3 class="h3">
            Купить и не потерять: обзор популярных застежек на серьги
          </h3>
        </a>
        <div class="doing__date">20 марта 2020</div>
        <p>
          Какие бывают застежки? Какие их преимущества и недостатки? Как
          подобрать подходящую для себя и избежать разочарования?
        </p>
      </div></swiper-slide
    >
    <swiper-slide
      ><div class="doing__item">
        <a href="/ru/news#st">
          <img src="@/assets/img/news/ST400x400.jpg" alt="ST400" />
        </a>
        <div class="doing__content">
          <div class="doing__title">Новости</div>
          <a href="/ru/news#st"
            ><h3 class="h3">Как выбрать украшения по своему цветотипу?</h3>
          </a>
          <div class="doing__date">10 марта 2020</div>
          <p>
            Кто-то выглядит эффектно, просто надев серьги с гранатом, а на
            ком-то они смотрятся нелепо. Один и тот же цвет может волшебным
            образом преобразить человека. Но не каждого и не всегда удачно. Всё
            дело в вашем цветотипе, о котором и пойдет речь.
          </p>
        </div>
      </div></swiper-slide
    >
    <swiper-slide
      ><a href="/ru/news#clasps">
        <img src="@/assets/img/news/zamki_400x400.jpg" alt="clasps" />
      </a>
      <div class="doing__content">
        <div class="doing__title">Новости</div>
        <a href="/ru/news#clasps"
          ><h3 class="h3">
            Купить и не потерять: обзор популярных застежек на серьги
          </h3>
        </a>
        <div class="doing__date">20 марта 2020</div>
        <p>
          Какие бывают застежки? Какие их преимущества и недостатки? Как
          подобрать подходящую для себя и избежать разочарования?
        </p>
      </div></swiper-slide
    >
    <swiper-slide>Slide 4</swiper-slide>
    <swiper-slide>Slide 5</swiper-slide>
    <swiper-slide>Slide 6</swiper-slide>
    <swiper-slide>Slide 7</swiper-slide>
    <swiper-slide>Slide 8</swiper-slide>
    <swiper-slide>Slide 9</swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>


<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import 'swiper/css/swiper.css'

export default {
  name: "swiper-example-loop-group",
  // title: 'Loop mode with multiple slides per group',
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: 3,
        slidesPerGroup: 3,
        loop: true,
        loopFillGroupWithBlank: true,
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
        },
      },
    };
  },
};
</script>

<style scoped lang="scss">
.swiper-container {
	padding-bottom: 20px;
}
.swiper-pagination-fraction, .swiper-pagination-custom, .swiper-container-horizontal > .swiper-pagination-bullets {
	bottom: 0;
}
</style>