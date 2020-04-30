<template>
  <v-app>
    <v-app-bar
                app
                color="white"
                flat
                light
                style="padding: 0 15% 0 15%;"
        >

              <div class="d-flex">
                <v-img
                        alt="Logo"
                        class="shrink"
                        contain
                        src="../src/assets/logo.png"
                        transition="scale-transition"
                />
              </div>
          <v-spacer></v-spacer>
              <v-toolbar-items id="appbar" >
                <v-btn
                        id="btnbar"
                        v-for="item in barbtn" :key="item.title"
                        color="transparent"
                        class="text-none primary--text"
                        style=" font-family: 'Roboto', sans-serif;
                                font-weight: normal;
                                letter-spacing: normal;
                                font-size: 18px;
                                padding: 0 13px 0 13px"
                        depressed>
                  {{ item.title}}
                </v-btn>
              </v-toolbar-items>

        </v-app-bar>
 <!--   <v-navigation-drawer
            color="transparent"
            fixed
            flat
    >
    </v-navigation-drawer> -->
    <v-content>
      <div class="section bg-hero">
        <v-row no-gutters>
          <v-col cols="10" class="hero">
            <v-row no-gutters>
              <v-col cols="4" offset="4" offset-lg="3">
                <v-container id="heroinfo">
                  <v-card v-for="item in heroinf" :key="item.index" color="transparent" class="mt-12" flat>
                    <v-card-title class="primary--text" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase; margin-bottom: 1rem;">
                      {{item.title}}
                    </v-card-title>
                    <v-card-subtitle style="font-family: 'Roboto'; font-size: 18px" class="black--text">
                      {{item.subtitle}}
                    </v-card-subtitle>
                  </v-card>
                  <v-card-actions>
                    <v-btn rounded class="primary--text" style="min-width: 36px; margin-right: 40px">
                      ?
                    </v-btn>
                    <v-btn rounded class="primary--text" style="min-width: 36px">
                      ?
                    </v-btn>
                  </v-card-actions>
                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

      <div class="section">
        <v-row no-gutters>
          <v-col cols="10" lg="11">
            <v-row no-gutters>
              <v-col cols="8" offset="4" offset-lg="3">
                <v-container>

                  <v-card-title class="primary--text mb-12" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase; margin-top: 100px">
                    Обо мне
                  </v-card-title>

                  <v-row no-gutters justify="space-between">

                      <div>
                        <v-card color="primary" class="white--text" style=" position:relative; width: 475px; padding: 2rem">
                          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                          <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
                          <div style="position: absolute; left: 10%; top: 95%">
                            <v-card color="white" class="primary--text" style="width: 510px; padding: 2rem">
                              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                              <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
                            </v-card>
                          </div>
                          <div style="position: absolute; top: 35%; left: 95%">
                            <v-img transition="scale-transition" src="../src/assets/M.png"></v-img>
                          </div>
                        </v-card>
                      </div>

                    <v-card flat style="max-width: 415px" color="transparent">
                      <v-row no-gutters justify="end">
                        <v-img
                                max-width="225px"
                                src="../src/assets/about1.png"
                                transition="scale-transition"
                                class="ma-1"
                        />
                        <v-img
                                max-width="225px"
                                src="../src/assets/about2.png"
                                transition="scale-transition"
                                class="ma-1"
                        />
                        <v-img
                                max-width="400px"
                                src="../src/assets/about3.png"
                                transition="scale-transition"
                                class="ma-1"
                        />
                      </v-row>
                    </v-card>

                <!--    <v-overlay>
                      <img src="../src/assets/M.png">
                    </v-overlay> -->
                  </v-row>
                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

      <div class="section">
        <v-row no-gutters>
          <v-col cols="10" lg="11">
            <v-row no-gutters>
              <v-col cols="8" offset="4" offset-lg="3">
                <v-container>

                  <v-card-title class="primary--text" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase;">
                    Индивидуальные консультации
                  </v-card-title>

                  <v-row no-gutters justify="space-between">
                    <v-card flat>
                      <v-card-title>
                        <v-img height="642px" transition="scale-transition" src="../src/assets/consult1.png"></v-img>
                      </v-card-title>
                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn color="primary" class="white--text">Контент-мейкер</v-btn>
                        <v-spacer></v-spacer>
                      </v-card-actions>
                    </v-card>

                    <v-card flat>
                      <v-card-title>
                        <v-img height="642px" transition="scale-transition" src="../src/assets/consult2.png"></v-img>
                      </v-card-title>
                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn color="primary" class="white--text">Ивентщик</v-btn>
                        <v-spacer></v-spacer>
                      </v-card-actions>
                    </v-card>

                    <v-card flat>
                      <v-card-title>
                        <v-img height="642px" transition="scale-transition" src="../src/assets/consult3.png"></v-img>
                      </v-card-title>
                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn color="primary" class="white--text">Аффтор жжот</v-btn>
                        <v-spacer></v-spacer>
                      </v-card-actions>
                    </v-card>

                  </v-row>
                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

      <div class="section bg-haliava">
        <v-row no-gutters>
          <v-col cols="10" lg="11">
            <v-row no-gutters>
              <v-col cols="8" offset="4" offset-lg="3">
                <v-container>

                  <v-card-title class="white--text mb-12" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase; margin-top: 100px">
                    Халява, плиз!
                  </v-card-title>

                  <v-card width="100%" color="primary"> <!-- циклом сделать не получилось (-->
                    <v-row no-gutters >
                      <v-col cols="3">
                        <v-card-title>
                          <v-img transition="scale-transition" src="../src/assets/hal1.png"></v-img>
                        </v-card-title>
                      </v-col>
                      <v-col cols="9">
                        <v-card-text class="white--text" style="font-weight: bold; font-size: 24px; height: 60%">
                          Гайд по заработку на текстах
                        </v-card-text>
                        <v-card-text align="end">
                          <v-btn class="white--text mr-10" color="primary" style="height: 55px; border-radius: 20px; box-shadow: 0 3px 3px rgba(0,0,0, 0.1),0 -3px 3px rgba(225,225,225, 0.4);">
                            Подробнее
                          </v-btn>
                          <v-btn class="white--text" color="primary" style="min-width: 36px; border-radius: 50%; box-shadow: 0 3px 3px rgba(0,0,0, 0.1),0 -3px 3px rgba(225,225,225, 0.4);">
                            ?
                          </v-btn>
                        </v-card-text>
                      </v-col>
                    </v-row>
                  </v-card>

                  <v-card width="100%" color="primary">
                    <v-row no-gutters >
                      <v-col cols="3">
                        <v-card-title>
                          <v-img transition="scale-transition" src="../src/assets/hal2.png"></v-img>
                        </v-card-title>
                      </v-col>
                      <v-col cols="9">
                        <v-card-text class="white--text" style="font-weight: bold; font-size: 24px; height: 60%">
                          Бесплатный вебинар по event-маркетингу
                        </v-card-text>
                        <v-card-text align="end">
                          <v-btn class="white--text mr-10" color="primary" style="height: 55px; border-radius: 20px; box-shadow: 0 3px 3px rgba(0,0,0, 0.1),0 -3px 3px rgba(225,225,225, 0.4);">
                            Подробнее
                          </v-btn>
                          <v-btn class="white--text" color="primary" style="min-width: 36px; border-radius: 50%; box-shadow: 0 3px 3px rgba(0,0,0, 0.1),0 -3px 3px rgba(225,225,225, 0.4);">
                            ?
                          </v-btn>
                        </v-card-text>
                      </v-col>
                    </v-row>
                  </v-card>

                  <v-card width="100%" color="primary" class="mb-12">
                    <v-row no-gutters >
                      <v-col cols="3">
                        <v-card-title>
                          <v-img transition="scale-transition" src="../src/assets/hal3.png"></v-img>
                        </v-card-title>
                      </v-col>
                      <v-col cols="9">
                        <v-card-text class="white--text" style="font-weight: bold; font-size: 24px; height: 60%">
                          Чек-лист по контент продвижению
                        </v-card-text>
                        <v-card-text align="end">
                          <v-btn class="white--text mr-10" color="primary" style="height: 55px; border-radius: 20px; box-shadow: 0 3px 3px rgba(0,0,0, 0.1),0 -3px 3px rgba(225,225,225, 0.4);">
                            Подробнее
                          </v-btn>
                          <v-btn class="white--text" color="primary" style="min-width: 36px; border-radius: 50%; box-shadow: 0 3px 3px rgba(0,0,0, 0.1),0 -3px 3px rgba(225,225,225, 0.4);">
                            ?
                          </v-btn>
                        </v-card-text>
                      </v-col>
                    </v-row>
                  </v-card>

                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

      <div class="section">
        <v-row no-gutters>
          <v-col cols="10" lg="11">
            <v-row no-gutters>
              <v-col cols="8" offset="4" offset-lg="3">
                <v-container>

                  <v-card-title class="primary--text" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase; margin-top: 100px">
                    Мои проекты
                  </v-card-title>

                  <v-row no-gutters>
                    <v-col v-for="item in 6" :key="item.item" cols="4">
                      <v-card flat>
                        <v-card-title>
                          <v-img transition="scale-transition" src="../src/assets/work.png"></v-img>
                        </v-card-title>
                        <v-card-text align="end" class="black--text" style="font-size: 18px">
                          Name project
                          <span><v-btn rounded class="primary--text" style="min-width: 36px; margin-left: 20px">
                            <!-- ? -->
                          </v-btn></span>
                        </v-card-text>
                      </v-card>
                    </v-col>


                  </v-row>


                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

      <div class="section" style="background-color: #FFF8F8">
        <v-row no-gutters>
          <v-col cols="10" lg="11">
            <v-row no-gutters>
              <v-col cols="8" offset="4" offset-lg="3">
                <v-container>

                  <v-card-title class="primary--text" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase; margin-top: 100px">
                    Книги
                  </v-card-title>

                  <v-row no-gutters justify="space-around">
                    <v-card flat color="transparent" width="390px">
                      <v-card-title>
                        <v-img transition="scale-transition" src="../src/assets/book01.png"></v-img>
                      </v-card-title>
                      <v-card-title style="font-size: 24px">
                        <span class="primary--text">ИММИГРАНТКА</span><span style="font-style: italic; font-weight: normal">.fi</span>
                      </v-card-title>
                      <v-card-text>
                        На дворе экономический кризис, дома – кризис семейный. Для того, чтобы поправить финансовое положение и спасти любовь, Она покупает себе и мужу билеты, садится на паром Таллинн – Хельсинки и… совершает побег в новую жизнь.
                      </v-card-text>

                      <v-card-subtitle class="primary--text" style="text-transform: uppercase; font-weight: bold">
                        Подробнее
                        <span><img transition="scale-transition" src="../src/assets/rect.png"></span>
                      </v-card-subtitle>
                    </v-card>

                    <v-card flat color="transparent" width="390px">
                      <v-card-title>
                        <v-img transition="scale-transition" src="../src/assets/book02.png"></v-img>
                      </v-card-title>
                      <v-card-title class="primary--text" style="font-size: 24px">
                        ИМПОРТНЫЕ МАМЫ
                      </v-card-title>
                      <v-card-text>
                        Три девицы под окном пряли поздно вечерком. А наши три девицы уехали в тридесятое царство, тридесятое государство и вышли замуж за добрых молодцев.<br>
                        Помните, как в сказке?
                      </v-card-text>

                      <v-card-subtitle class="primary--text" style="text-transform: uppercase; font-weight: bold">
                        Подробнее
                        <span><img transition="scale-transition" src="../src/assets/rect.png"></span>
                      </v-card-subtitle>
                    </v-card>
                  </v-row>



                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

      <div class="section">
        <v-row no-gutters>
          <v-col cols="10" lg="11">
            <v-row no-gutters>
              <v-col cols="8" offset="4" offset-lg="3">
                <v-container>

                  <v-card-title class="primary--text mb-12" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase; margin-top: 100px">
                    Обо мне в медиа
                  </v-card-title>

                  <v-row no-gutters justify="space-between">

                    <div>
                      <v-card color="primary" class="white--text" style=" position:relative; width: 475px; padding: 2rem">
                        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                        <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
                        <div style="position: absolute; left: 10%; top: 95%">
                          <v-card color="white" class="primary--text" style="width: 510px; padding: 2rem">
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                            <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
                          </v-card>
                        </div>
                      </v-card>
                    </div>

                    <v-card flat style="max-width: 415px" color="transparent">
                      <v-row no-gutters>
                        <v-container>
                          <v-row no-gutters>
                            <v-col cols="6">
                              <v-img
                                      src="../src/assets/about4.png"
                                      transition="scale-transition"
                                      class="mr-2"
                              />
                            </v-col>
                            <v-col cols="6">
                              <v-img
                                      src="../src/assets/about1.png"
                                      transition="scale-transition"
                                      class="mb-2"
                              />
                              <v-img

                                      src="../src/assets/about2.png"
                                      transition="scale-transition"
                                      class="pa-1"
                              />
                            </v-col>
                          </v-row>
                          <v-row no-gutters>
                            <v-img
                                    src="../src/assets/about3.png"
                                    transition="scale-transition"
                                    class="mt-2"
                            />
                          </v-row>

                        </v-container>
                      </v-row>
                    </v-card>
                  </v-row>
                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

      <div class="section" style="background-color: #E51A4B">
        <v-row no-gutters>
          <v-col cols="10" lg="11">
            <v-row no-gutters>
              <v-col cols="8" offset="4" offset-lg="3">
                <v-container>

                  <v-card-title class="white--text mb-12" style="font-family: 'Cyrvetica'; font-size: 48px; text-transform: uppercase; margin-top: 100px">
                    Контакты
                  </v-card-title>

                  <v-card class="pt-12 pb-12">
                    <v-card-title class="primary--text mb-12" style="font-size: 24px">
                      <v-spacer></v-spacer>
                      Оставьте свою заявку и мы с вами свяжемся
                      <v-spacer></v-spacer>
                    </v-card-title>
                    <v-card-text>
                      <v-row no-gutters justify="center">
                          <v-text-field outlined placeholder="Имя" class="shrink mr-3" style="width: 240px"></v-text-field>
                          <v-text-field outlined placeholder="E-mail" class="shrink mr-3" style="width: 330px"></v-text-field>
                          <v-btn class="white--text" color="primary" style="height: 52px; text-transform: none; font-weight: bold; font-size: 15px">Отправить</v-btn>
                      </v-row>
                    </v-card-text>
                  </v-card>

                  <v-row no-gutters>
                    <v-col cols="6" class="mt-12" style="font-size: 18px; font-weight: bold">
                      <v-card class="white--text" align="center" flat color="transparent">
                        (?) +333333333
                      </v-card>
                    </v-col>
                    <v-col cols="6" class="mt-12" style="font-size: 18px; font-weight: bold">
                      <v-card class="white--text" align="center" flat color="transparent">
                        (?) ksenia.malkki
                      </v-card>
                    </v-col>
                    <v-col cols="6" class="mt-12" style="font-size: 18px; font-weight: bold">
                      <v-card class="white--text" align="center" flat color="transparent">
                        (?) pochta@gmail.com
                      </v-card>
                    </v-col>
                    <v-col cols="6" class="mt-12 mb-12" style="font-size: 18px; font-weight: bold">
                      <v-card class="white--text" align="center" flat color="transparent">
                        (?) ksenia.malkki
                      </v-card>
                    </v-col>
                  </v-row>

                </v-container>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>

        <div style="background-color: #E51A4B">
            <v-card color="transparent" style="padding: 1rem 15% 1rem 15%;">
                <v-row no-gutters class="white--text">
                    <div class="d-flex">
                        <v-img
                                alt="Logo"
                                class="shrink"
                                contain
                                src="../src/assets/logo2.png"
                                transition="scale-transition"
                        />
                    </div>
                    <v-spacer></v-spacer>
                    <span class="mt-2">© 2020 Все права защищены</span>
                    <v-spacer></v-spacer>
                    <span class="mt-2">Developer ProSofta</span>
                </v-row>
            </v-card>
        </div>

        <div style="position: fixed; top:40%; left:16%; z-index: 100; height: 20vh; width: 8%;">
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
            <div style="width: 50px; height: 2px; background-color: #E51A4B; margin-bottom: 15px"></div>
        </div>

    </v-content>
  </v-app>
</template>

<script>
//import Hero from './components/Hero';

export default {
  name: 'App',

  components: {
    //Hero,
  },

  computed: {
    barbtn () {
      return [
        {title: 'Обо мне'},
        {title: 'Консультации'},
        {title: 'Мои проекты'},
        {title: 'Книги'},
        {title: 'Халява, плиз!'},
        {title: 'Контакты'}
      ]
    },
    heroinf () {
      return[
        {title:"Бизнесвумен", subtitle:"Основала агентство контент-маркетинга Malkki Media, организатор мероприятий."},
        {title:"Писатель", subtitle:"Автор книг о жизни и воспитании детей в Финляндии."},
        {title:"Блогер", subtitle:"В Instagram блог о бизнесе и текстах."}
      ]
    }
  },

  data: () => ({
    //
  }),
};
</script>

<style>

  @font-face {
    font-family: Cyrvetica;
    src: url(../src/fonts/cyrvetica-extra-outline.ttf);
  }

  .section{
    margin: 0;
    padding: 0;
    min-height: 100vh;
    position: relative;
  }

  .bg-hero{
    background: white url("../src/assets/bghero.png") right bottom no-repeat;
  }

  .hero{
    height: 100vh;
    background: transparent url("../src/assets/hero.png") right bottom no-repeat;
  }

  .bg-haliava{
    background: white url("../src/assets/haliava.png") center center no-repeat;
  }

</style>
