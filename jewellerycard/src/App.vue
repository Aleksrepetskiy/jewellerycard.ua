<template>
  <div id="app" class="container">
    <Header />
    <main class="main">
		<router-view />
      <!-- <div id="nav">
		<router-link to="/">Home</router-link> |
		<router-link to="/about">About</router-link> |
		<router-link to="/contact">Contact</router-link>
		</div>
		<router-view/> -->
    </main>
    <Footer />
    <div id="active-popup" class="popup" style="">
      <div class="popup__content">
        <div class="popup__middle js-append-box">
          <div data-controller="User" class="append-popup-content">
            <div class="popup__top clearfix">
              <div class="popup__ttl">Вхід</div>
              <div class="popup__authorization">
                <a
                  class="popup__authorization-link popup__authorization-link--registration"
                  href="/user/signup/"
                  rel="nofollow"
                  data-action="signup"
                  >Зареєструватися ⟶</a
                >
              </div>
            </div>
            <div class="popup__middle">
              <form
                id="w0"
                action="/rest/user?view=login"
                method="post"
                novalidate="true"
                data-blur="false"
              ></form>
              <form
                id="form-user-default-login-1"
                class="popup__form user-form-login"
                name="login_panel"
                action="/user/login/"
                method="post"
                data-tools='["updateInputs"]'
                novalidate="true"
                data-blur="false"
              >
                <div class="row-input field-login-email required">
                  <div class="b-input b-input-v2">
                    <input
                      type="email"
                      id="login-email"
                      name="Login[email]"
                      form="form-user-default-login-1"
                      data-property="email"
                      pattern="^[^@]+@[^\.]+\..+"
                      aria-required="true"
                      required="true"
                      class="form-entered form-filled"
                    />
                    <label class="ttl-input" for="login-email">Email</label
                    ><span class="form-clear icon icon-cancel"></span>
                    <p class="help-block-error"></p>
                  </div>
                </div>
                <div class="row-input field-login-password required">
                  <div class="b-input b-input-v2">
                    <input
                      type="password"
                      id="login-password"
                      name="Login[password]"
                      value=""
                      form="form-user-default-login-1"
                      data-property="password"
                      aria-required="true"
                      required="true"
                      class="form-entered form-filled"
                    />
                    <label class="ttl-input" for="login-password">Пароль</label
                    ><span class="form-clear icon icon-cancel"></span
                    ><span
                      data-tools='["viewPassword"]'
                      class="icon icon-eye_close"
                    ></span>
                    <p class="help-block-error"></p>
                  </div>
                </div>
                <div class="row-input row-input--double clearfix">
                  <div class="row-input__wrap">
                    <div class="row-left">
                      <div class="b-input b-input-v2">
                        <input
                          type="hidden"
                          name="Login[rememberMe]"
                          value="0"
                        />
                        <input
                          type="checkbox"
                          id="login-rememberme"
                          name="Login[rememberMe]"
                          value="1"
                          checked=""
                          data-property="rememberMe"
                          class="form-entered form-filled"
                        />
                        <label
                          for="login-rememberme"
                          class="hint-form__check-text"
                          >Запам'ятати мене</label
                        >
                        <p class="help-block-error"></p>
                      </div>
                    </div>
                    <div class="row-right">
                      <div class="remind-pass">
                        <a
                          class="row-link"
                          href="/user/password/reset-request/"
                          rel="nofollow"
                          data-action="resetRequest"
                          data-tools='["mobileResetRequest"]'
                          >Забули пароль?</a
                        >
                      </div>
                    </div>
                  </div>
                  <input type="hidden" name="notification" value="true" />
                  <div class="popup__btns">
                    <button
                      type="submit"
                      class="btn btn-blue"
                      name="Login[scenario]"
                      value="byEmail"
                      form="form-user-default-login-1"
                    >
                      Увійти
                    </button>
                  </div>
                </div>
              </form>
            </div>
            <div class="popup__bottom">
              <div class="popup__socials">
                <div class="popup__socials-ttl">Або увійти як користувач:</div>
                <div id="w1" class="popup__socials-btns">
                  <a
                    class="auth-link"
                    href="/auth/?authclient=google"
                    title="Google"
                    ><span class="svg svg-googleplus"></span></a
                  ><a
                    class="auth-link"
                    href="/auth/?authclient=facebook"
                    title="Facebook"
                    ><span class="svg svg-fb"></span
                  ></a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="popup__exit">
          <span class="icon icon-cancel"></span>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";

export default {
  name: "Home",
  components: {
    //HelloWorld,
    Footer,
    Header,
  },
};
</script>

<style lang="scss">
#active-popup {
	display: none;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;
    margin: 0 10px;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
