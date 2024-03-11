<template>
  <v-app theme="">
    <v-app-bar flat class="border-b" color="white">
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-app-bar-title class="poppins-semibold">
        <h2>Destine-se</h2>
      </v-app-bar-title>
    </v-app-bar>

    <v-main>
      <section id="id1">
        <v-container fluid class="pa-0">
          <v-card>
            <v-img
              :aspect-ratio="3 / 1"
              cover
              src="https://images.pexels.com/photos/2242207/pexels-photo-2242207.jpeg"
              height="670px"
            >
              <div
                class="fill-height d-flex justify-center flex-column pa-16 mx-10 my-6"
              >
                <v-card-title class="custom-title font-weight-bold">
                  Crie o seu DESTINO</v-card-title
                >

                <!-- <v-btn
                  rounded="xl"
                  class="btn-hover"
                  variant="outlined"
                  color="white"
                  size="x-large"
                  width="200"
                >
                  Teste
                </v-btn> -->
              </div>
            </v-img>
          </v-card>
        </v-container>

        <v-row justify="center" :class="{ suo: mdAndUp }">
          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="card-hover" elevation="20">
              <v-img
                class="align-end text-white hover-effect"
                src="https://images.pexels.com/photos/3389955/pexels-photo-3389955.jpeg"
              >
                <v-card-title class="poppins-semibold"
                  >Passeio de balão</v-card-title
                >
              </v-img>
            </v-card>
          </v-col>

          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="card-hover" elevation="20">
              <v-img
                class="align-end text-white hover-effect"
                src="https://images.pexels.com/photos/19639797/pexels-photo-19639797/free-photo-of-cidade-meio-urbano-ferias-ponto-de-referencia.jpeg"
              >
                <v-card-title class="poppins-semibold"
                  >Pontos turísticos</v-card-title
                >
              </v-img>
            </v-card>
          </v-col>

          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="card-hover" elevation="20">
              <v-img
                class="align-end text-white hover-effect"
                src="https://images.pexels.com/photos/2225499/pexels-photo-2225499.jpeg"
              >
                <v-card-title class="poppins-semibold">Praias</v-card-title>
              </v-img>
            </v-card>
          </v-col>
        </v-row>
      </section>

      <section id="id2" class="mt-10">
        <v-container class="pa-0" fluid style="height: 60dvh">
          <div class="fill-height">
            <v-row class="align-center justify-center">
              <v-col cols="auto">
                <v-card
                  elevation="10"
                  append-icon="mdi-account"
                  class="mx-auto"
                  width="300"
                  height="320"
                  subtitle="Malibu - Califórnia"
                  title="Tony Stark"
                >
                  <v-rating
                    class="mt-1 ml-2"
                    :model-value="4.5"
                    color="amber"
                    density="compact"
                    size="comfort"
                    half-increments
                    readonly
                  ></v-rating>
                  <v-card-text>
                    " Excellent tour programming, got to fly a lot. "
                    <br />
                    <br />
                    " I had difficulty parking my plane at the 'Parque de
                    rodeio' and crossing the Júlio Borella, it took me 15
                    minutes to get through! "
                    <br />
                    <br />
                    " Suó for the next one!! "
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="auto">
                <v-card
                  elevation="10"
                  append-icon="mdi-account"
                  class="mx-auto"
                  width="300"
                  height="320"
                  subtitle="Buenos Aires - Argentina"
                  title="Maradona"
                >
                  <v-rating
                    class="mt-1 ml-2"
                    :model-value="5"
                    color="amber"
                    density="compact"
                    size="comfort"
                    half-increments
                    readonly
                  ></v-rating>
                  <v-card-text>
                    " Me gustaron mucho las playas y las chicas. La comida que
                    ofrecían dentro del hotel, definitivamente volveré. "
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="auto">
                <v-card
                  elevation="10"
                  append-icon="mdi-account"
                  class="mx-auto"
                  width="300"
                  height="320"
                  subtitle="Rio de Janeiro - RJ"
                  title="Augustinho Carrara"
                >
                  <v-rating
                    class="ml-2"
                    :model-value="3.0"
                    color="amber"
                    density="compact"
                    size="comfort"
                    half-increments
                    readonly
                  ></v-rating>
                  <v-card-text>
                    " Fui com toda a família para Nicolau Vergueiro, o roteiro e
                    a organização foram fantásticos. Trouxe salame e erva-mate
                    das Salamarias. " <br />
                    <br />
                    "Não gostei do asfalto Marau - Passo Fundo, furei o pneu do
                    meu Taxi."
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
          </div>
        </v-container>
      </section>
    </v-main>
    <v-footer class="text-center d-flex flex-column align-center">
      <div>
        <v-row>
          <v-btn
            prepend-icon="mdi-instagram"
            href="https://instagram.com/gaabrielbrocco"
            title="Perfil"
            class="mb-5"
            variant="text"
          ></v-btn>
          <v-btn
            prepend-icon="mdi-linkedin"
            href="https://www.linkedin.com/in/gabrielbrocco"
            title="Linkedin"
            class="mb-5"
            variant="text"
          ></v-btn>
          <v-btn
            prepend-icon="mdi-twitter"
            href="https://x.com/gaabrielbrocco"
            title="Twitter"
            class="mb-5"
            variant="text"
          ></v-btn>
          <v-btn
            prepend-icon="mdi-email"
            href="mailto:gabsbrocco@gmail.com"
            title="Email"
            class="mb-5"
            variant="text"
          ></v-btn>

        </v-row>
      </div>

      <div class="pt-0">
        Dashboard simples de uma página Web como exemplo para empresa de viagens. Desenvolvida para evoluir conhecimentos utilizando Vue 3 e Vutify.
      </div>

      <v-divider></v-divider>

      <div>{{ new Date().getFullYear() }} — <strong>G B O</strong></div>
    </v-footer>
  </v-app>
</template>

<script setup>
import { useDisplay } from "vuetify";

const { mdAndUp } = useDisplay();
</script>

<style scoped>
.poppins-extralight {
  font-family: "Poppins", sans-serif;
  font-weight: 200;
  font-style: normal;
}

.poppins-light {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  font-style: normal;
}

.poppins-semibold {
  font-family: "Poppins", sans-serif;
  font-weight: 600;
  font-style: normal;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.img-fluid {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.app-color {
  background-color: #11233f;
}

.suo {
  margin-top: -80px;
}
.hover-effect {
  transition: transform 0.5s ease;
}
.hover-effect:hover {
  transform: scale(1.05);
}

.custom-title {
  font-size: 62px;
  color: white;
}
</style>
