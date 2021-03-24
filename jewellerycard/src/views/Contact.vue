<template>
      <div class="wrapper wrapper--pages">
        <section class="contacts">
          <h2 class="h2">Контакты:</h2>
          <div class="row">
            <div class="col8 middle">
              <p>
                От флагманского ювелирного шоу-рума в сердце столицы до
                региональных магазинов сети Jewellery Card, Вы везде можете
                рассчитывать на высочайший уровень обслуживания и теплую
                семейную атмосферу. Только так мы видим эффективные и
                взаимовыгодные отношения в таких направлениях как:
              </p>
              <ul class="ul">
                <li class="li">
                  создание эксклюзивных украшений по индивидуальным эскизам;
                </li>
                <li class="li">инвестиционное сотрудничество;</li>
                <li class="li">оптовая закупка ювелирных украшений.</li>
              </ul>
              <p>
                Просто отправьте нам сообщение с интересующими Вас вопросами,
                либо заполните форму обратной связи ниже:
              </p>
            </div>
          </div>
          <div class="row">
            <div class="col6 middle">
              <div class="contacts__relations">
                <div class="relations">
                  <!--                        <div class="relations__item">-->
                  <!--                            <a href="tel:+380442353916" class="relations__link"><span class="icon icon-phone"></span>+380442353916</a>-->
                  <!--                        </div>-->
                  <div class="relations__item">
                    <a
                      href="mailto:inquiries@jewellerycard.ua"
                      class="relations__link"
                      ><span class="icon icon-mail"></span
                      >inquiries@jewellerycard.com</a
                    >
                  </div>
                </div>
              </div>
              <div class="contacts__form">
                <div class="success" style="display: none">
                  <div class="success__box">
                    <div class="success__img">
                      <img src="/img/contact/mail.png" alt="" />
                    </div>
                    <div class="success__text">
                      <span class="first-text"
                        >Спасибо, письмо отправлено!</span
                      >
                      <span class="second-text"
                        >Мы ответим Вам в течении 24 часов.</span
                      >
                    </div>
                  </div>
                </div>
                <h3 class="h3">Написать нам</h3>
                <div class="form">
                  <form action="/ru/contacts" method="post" novalidate="">
                    <div class="contacts__form-flex">
                      <div class="form__row">
                        <div class="b-input">
                          <div class="form__error"></div>
                          <input
                            type="text"
                            name="name"
                            value=""
                            pattern="^[a-zA-Zа-яА-Я'][a-zA-Zа-яА-Я-' ]+[a-zA-Zа-яА-Я']?$"
                            placeholder="Имя"
                            class="rfield"
                            minlength="3"
                            maxlength="40"
                            required=""
                          />
                        </div>
                      </div>
                      <div class="form__row">
                        <div class="b-input">
                          <div class="form__error"></div>
                          <input
                            type="email"
                            name="email"
                            value=""
                            placeholder="Email"
                            class="rfield"
                            pattern="^.+@.+\..+$"
                            required=""
                          />
                        </div>
                      </div>
                    </div>
                    <div class="form__row">
                      <div class="b-textarea">
                        <div class="form__error"></div>
                        <textarea
                          class="rfield"
                          name="message"
                          placeholder="Текст"
                          maxlength="1000"
                          required=""
                        ></textarea>
                      </div>
                    </div>
                    <div class="form__row">
                      <input type="hidden" name="action" value="contactMail" />
                      <div class="b-button">
                        <button class="btn" type="submit">Отправить</button>
                      </div>
                    </div>
                    <input name="reCaptcha" id="reCaptcha" hidden="" />
                  </form>
                </div>
              </div>
            </div>
          </div>
          <div class="contacts__showroom">
            <h2 class="h2">Showroom</h2>
            <div class="row">
              <div class="col8 middle left-justify">
                <p>
                  Актуальные коллекции украшений, выпускаемые в свет нашим
                  ювелирным домом, представлены в наших шоурумах, где все
                  посетители имеют возможность ознакомиться и выбрать для себя
                  украшение из нескольких тысяч представленных. В уютной,
                  непринужденной обстановке, вы сможете не только неспешно
                  примерить на себя понравившиеся золотые украшения, но и
                  обсудить детали создания совершенно нового ювелирного
                  произведения по вашим индивидуальным эскизам.
                </p>
              </div>
            </div>
            <!--<div class="contacts__adress"><span class="icon icon-map-pin"></span>ул. Большая Васильковская, 16-->
          </div>
          <div class="contacts__interier">
            <div class="row">
              <div class="col4">
                <img src="/img/contact/contact_1.jpg" alt="" />
              </div>
              <div class="col4">
                <img src="/img/contact/contact_2.jpg" alt="" />
              </div>
              <div class="col4 hide">
                <img src="/img/contact/contact_3.jpg" alt="" />
              </div>
            </div>
          </div>
          <div class="contacts__total">
            <span class="contacts__total-great">20</span>
          </div>
          <h2 class="h2">Наши магазины в Украине</h2>
          <div class="row">
            <div class="col12">
              <img src="/img/contact/map.jpg" alt="" />
            </div>
          </div>
        </section>
      </div>
</template>

