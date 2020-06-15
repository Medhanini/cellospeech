<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-center">
        <v-img src="/cellospeech.com/CelloSpeech Logo.png" ></v-img>
      </div>
  <v-carousel
    cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
        <v-img :src="slide" ></v-img>
    </v-carousel-item>
  </v-carousel>
      <v-card>
        <v-card-title class="headline">
          let's play it
        </v-card-title>
        <v-card-text>
          <p>There are many variations but the of passages of but the majority Lorem Ipsum available, but the majority have su</p>
          <div class="text-xs-right">
            <em><small>&mdash; Imad Essaouissi</small></em>
          </div>
          <hr class="my-3">
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  data () {
      return {
        slides: [
          '/cellospeechgallery/1.jpg',
          '/cellospeechgallery/2.jpg',
          '/cellospeechgallery/3.jpg',
          '/cellospeechgallery/4.jpg',
          '/cellospeechgallery/5.jpg',
          '/cellospeechgallery/6.jpg',
          '/cellospeechgallery/7.jpg',
        ]
      }
    },
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>
