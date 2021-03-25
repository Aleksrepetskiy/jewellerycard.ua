<template>
  <footer class="footer">
    <div class="wrapper">
      <div class="footer__box footer__contacts">
        <div class="relations">
          <div class="relations__item">
            <a href="tel:+380442353916" class="relations__link"
              ><span class="icon icon-phone"></span>+380442353916</a
            >
          </div>
          <div class="relations__item">
            <a href="mailto:inquiries@jewellerycard.ua" class="relations__link"
              ><span class="icon icon-mail"></span>inquiries@jewellerycard.ua</a
            >
          </div>
        </div>
      </div>
      <div class="footer__box footer__logo">
        <img src="@/assets/img/svg/logo-footer.svg" alt="logo-footer" />
      </div>
      <div class="footer__box footer__copyrating">© 1999 Jewellery Card</div>
      <div class="to-top" style="display: block">
        <div class="to-top__img">
          <img src="@/assets/img/totopNormal.png" alt="" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  props: {
    msg: String,
  },
};
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.footer {
  background-color: #f8f8f8;
  border-top: 1px solid #ebebeb;
  position: relative;
  color: #b7b7b7;
  font-size: 14px;
  line-height: 1.2em;
  font-weight: 400;
  padding: 24px 0;
  &::before {
    content: "";
    width: 24px;
    height: 24px;
    display: block;
    background: url(../assets/img/svg/crown.svg) 0 0 no-repeat;
    position: absolute;
    left: 50%;
    margin-left: -10px;
    top: -12px;
  }

  .wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .relations {
    &__link {
      font-size: 14px;
      font-weight: 400;
      color: #434343;
    }

    .relations__item + .relations__item {
      margin-left: 10px;
    }
  }

  &__box {
    width: 33.33%;
  }

  &__logo img {
    margin: 0 auto;
    max-width: 166px;
  }

  &__copyrating {
    text-align: right;
  }

  .icon {
    margin-right: 18px;
    color: #b7b7b7;
    font-size: 14px;
  }

  .icon-mail {
    font-size: 11px;
  }
}

@media screen and (max-width: 1130px) {
  .footer {
    .relations {
      .relations__item + .relations__item {
        margin: 10px 0 0 0;
      }
    }
  }
}
@media screen and (max-width: 700px) {
  .footer {
    margin-top: 30px;
    .wrapper {
      flex-wrap: wrap;
    }

    &__logo {
      width: 100%;
      order: -1;
      margin-bottom: 20px;
    }

    &__contacts,
    &__copyrating {
      width: 50%;
    }

    .icon {
      margin-right: 5px;
    }
  }
}
@media screen and (max-width: 460px) {
  .footer__contacts,
  .footer__copyrating {
    width: 100%;
    text-align: center;
  }
  .footer__copyrating {
    margin-top: 20px;
  }
}
@media screen and (max-width: 420px) {
  .footer__box {
    width: 100%;
  }
}
@media screen and (max-width: 370px) {
  .footer {
    &__box {
      width: 100%;
      text-align: center;
    }

    &__copyrating {
      margin-top: 20px;
    }
  }
}
</style>