<template>
  <header class="header">
    <div class="logo">
      <div class="wrapper">
        <a class="logo__link" href="/ru/"
          ><img class="logo__img" src="/img/svg/logo.svg?v=1" alt="logo"
        /></a>
      </div>
    </div>
    <div class="hamburger" id="hamburger">
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
    </div>
    <div class="header__nav">
      <div class="wrapper">
        <nav class="menu">
          <ul class="menu__list">
            <li class="menu__item">
              <a href="/ru/about" class="menu__link">Ювелирный Дом</a>
            </li>
            <li class="menu__item">
              <a href="/ru/high-jewellery" class="menu__link">High Jewellery</a>
            </li>
            <li class="menu__item">
              <a href="/ru/lemonnier" class="menu__link">LemoNNier</a>
            </li>
            <li class="menu__item">
              <a href="/ru/collections" class="menu__link">Коллекция</a>
            </li>
            <li class="menu__item">
              <a href="/ru/contacts" class="menu__link">Контакты</a>
            </li>
          </ul>
        </nav>
        <div class="lang">
          <div class="lang__list">
            <div class="lang__item active">
              <span class="lang__link">RU</span>
            </div>
            <ul class="lang__dropdown">
              <li class="lang__item"><a href="/" class="lang__link">UA</a></li>
              <li class="lang__item">
                <a href="/en/" class="lang__link">EN</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String,
  },
};
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>