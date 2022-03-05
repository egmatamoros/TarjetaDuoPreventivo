<template>
  <v-container fluid fill-height class="d-flex align-start ma-0 pa-0" >
    <v-row  class="align-self-stretch blue lighten-2 d-flex justify-center align-center" no-gutters>
      <v-col cols="12" md="4" class="">
        <v-card>
          <v-card-title class="d-flex justify-center">
            <v-spacer/>
            <b class="ml-16">Consultorio Dental</b>
            <v-spacer/>
            <v-img
              :src="require('../assets/duoPreventivo.png')"
              max-width="15%"
              aspect-ratio="1"
              class="justify-self-end"

            ></v-img>
            <br>
            <h6>Cepillo e hilo el dúo preventivo para la salud de tu sonrisa</h6>
          </v-card-title>
          <v-img
            height="360"
            :src="require('../assets/fondo.png')"
            class="d-flex justify-center text-center py-5"
          >
            <v-avatar size="250"   class="mx-auto">
              <img
                alt="user"
                :src="require('../assets/fotoMaggie.png')"
              />
            </v-avatar>
            <v-spacer/>
            <span><b class="tipografia">Magdalena Solís Oviedo</b></span>
            <br>
            <span>Cedula Prof. 10144905</span>
            
          </v-img>
          <v-card-subtitle class="text-center justify-center black--text">
            <p>
              Cirujana Dentista egresada de la UNAM, enfoco mi ejercicio profesional a fomentar la cultura de la prevención y la comprensión de la salud bucodental como parte del bienestar integral.
            </p>
            <p>
              <b><i>"Aspiramos a que la sonrisa de cada paciente contribuya a su calidad de vida.""</i></b>
            </p>
          </v-card-subtitle>
          <v-card-actions>
            <v-btn color="green" rounded class="mx-auto" block @click="whatsapp">
              <v-icon>mdi-whatsapp</v-icon>&nbsp;&nbsp;&nbsp; Escribeme por Whatsapp
            </v-btn>
          </v-card-actions>
        </v-card>
        <v-card class="mt-5">

          <v-card-title>
            Blanqueamiento Dental
          </v-card-title>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'Home',
  components: {
  },
  data: () => ({

  }),
  methods: {
    whatsapp(){
      window.open(
        "https://wa.me/525566986714?text=Hola%20vengo%20desde%20la%20tarjeta%20de%20presentacion",
        "_blank"
        );
    }
  }
}
</script>
<style scoped>
  @font-face {
    font-family: 'bellandha';
    src: url('/bellandha-signature.regular.ttf') format('opentype');
  }
  
  .tipografia{
    font-family: bellandha;
    font-size: 26pt;
  }

</style>
