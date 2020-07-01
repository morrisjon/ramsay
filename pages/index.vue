<template>
  <div>
    <section class="hero">
      <v-parallax
        src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
      >
        <v-row align="center" justify="center">
          <v-col class="text-center" cols="12">
            <v-icon dark size="72px">{{ mdiPlayCircle }}</v-icon>
            <h1 class="text-h2 font-weight-bold mt-10 mb-6">
              Vuetify.js is not that Awesome
            </h1>
            <h4 class="text-h5">Build your application today!</h4>
          </v-col>
        </v-row>
      </v-parallax>
    </section>
  </div>
</template>

<script>
  import { mdiPlayCircle } from '@mdi/js'
  export default {
    data() {
      return {
        mdiPlayCircle
      }
    }
  }
</script>
