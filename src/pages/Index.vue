<template>
  <q-page padding>
    <div class="q-pa-md">
      <div class="q-gutter-md">
        <q-carousel
          v-model="slide"
          transition-prev="scale"
          transition-next="scale"
          swipeable
          animated
          control-color="white"
          navigation
          padding
          arrows
          height="300px"
          class="bg-primary text-white shadow-1 rounded-borders"
        >
          <q-carousel-slide name="style" class="column no-wrap flex-center">
            <q-page class="flex flex-center">
              <img
                alt="Quasar logo"
                src="https://cdn.quasar.dev/img/mountains.jpg"
                style="width: 100%; height: 39%"
              />
            </q-page>
          </q-carousel-slide>
          <q-carousel-slide name="tv" class="column no-wrap flex-center">
            <q-page class="flex flex-center">
              <img
                alt="Quasar logo"
                src="https://cdn.quasar.dev/img/mountains.jpg"
                style="width: 100%; height: 50%"
              />
            </q-page>
          </q-carousel-slide>
          <q-carousel-slide name="layers" class="column no-wrap flex-center">
            <q-page class="flex flex-center">
              <img
                alt="Quasar logo"
                src="https://cdn.quasar.dev/img/mountains.jpg"
                style="width: 100%; height: 65%"
              />
            </q-page>
          </q-carousel-slide>
          <q-carousel-slide name="map" class="column no-wrap flex-center">
            <q-page class="flex flex-center">
              <img
                alt="Quasar logo"
                src="https://cdn.quasar.dev/img/mountains.jpg"
                style="width: 100%; height: 80%"
              />
            </q-page>
          </q-carousel-slide>
          <q-carousel-slide name="map" class="column no-wrap flex-center">
            <q-page class="flex flex-center">
              <img
                alt="Quasar logo"
                src="https://cdn.quasar.dev/img/mountains.jpg"
                style="width: 100%; height: 80%"
              />
            </q-page>
          </q-carousel-slide>
        </q-carousel>
      </div>
      <q-btn
        class="absolute-center"
        color="primary"
        icon="account_circle"
        label="about me"
        @click="$router.replace('/aboutme')"
      />
    </div>
  </q-page>
</template>
<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref('style')
    }
  }
}
</script>
