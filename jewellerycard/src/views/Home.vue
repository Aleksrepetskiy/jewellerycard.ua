<template>
  <div>
    <section class="banner limited">
      <video autoplay="" loop="" muted="muted">
        <source src="@/assets/img/video/banner.webm" type="video/webm" />
        Your browser does not support the video tag. I suggest you upgrade your
        browser.
        <img src="@/assets/img/video/banner.png" class="video-holder" />
      </video>
      <div class="banner__content">
        <div class="banner__title">
          Where Perfection <br />
          Becomes Passion
        </div>
        <h2 class="h2">— 1999 —</h2>
      </div>
    </section>
    <div class="wrapper">
      <section class="direction">
        <div class="row">
          <div class="col4">
            <div class="direction__desc">
              <h2 class="h2">Производство</h2>
              <p>
                Приоткрываем завесу над таинством создания ювелирных шедевров
                мастерами ювелирного дома Jewellery Card. Впервые за 19 лет.
              </p>
              <a href="/ru/production" class="btn">Детальнее</a>
            </div>
          </div>
          <div class="col8 order_0">
            <h2 class="h2 hide">Производство</h2>
            <div class="direction__img">
              <img src="@/assets/img/production/index.jpg" alt="" />
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col8">
            <div class="direction__img">
              <h2 class="h2 hide">High Jewellery</h2>
              <img src="@/assets/img/high/index.jpg" alt="" />
            </div>
          </div>
          <div class="col4 col4-pad">
            <div class="direction__desc">
              <h2 class="h2">High Jewellery</h2>
              <p>
                Почувствуйте трепет от обладания поистине уникальным ювелирным
                украшением, которое идеально дополняет Ваш образ и черты
                характера. Откройте мир High Jewellery сегодня.
              </p>
              <a href="/ru/high-jewellery" class="btn">Детальнее</a>
            </div>
          </div>
        </div>
      </section>
      <section class="doing mb-80">
        <h2 class="h2">События</h2>
        <Slider />
      </section>
    </div>
  </div>
</template>

<script>
import Slider from "@/components/Slider.vue";
export default {
  name: "Home",
  components: {
    Slider,
  },
};
</script>


