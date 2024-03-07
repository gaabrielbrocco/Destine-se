<template>
  <v-app theme="">
    <v-app-bar flat class="border-b" color="white">
      <v-app-bar-nav-icon
        @click="isDrawerOpen = !isDrawerOpen"
      ></v-app-bar-nav-icon>
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
              <div class="fill-height d-flex justify-center flex-column pa-15">
                <v-card-title> Crie o SEU DESTINO</v-card-title>

                <v-btn
                  rounded="xl"
                  class="btn-hover"
                  variant="outlined"
                  color="white"
                  size="x-large"
                  width="200"
                >
                  Teste
                </v-btn>
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

      <v-section id="id2">
        <v-container
          class="pa-0 mt-15"
          fluid
          style="background-color: #f3f3f3; height: 70dvh"
        >
        </v-container>
      </v-section>
    </v-main>
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
</style>
