<template>
  <q-page padding>
    <div class="q-pa-md row items-start q-gutter-md">
      <q-card
        class="my-card text-white absulute-center"
        flat
        bordered
        style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)">
        <q-card-section>
          <div class="text-h5 q-mt-sm q-mb-xs">Our Changing Planet</div>
          <div>
            <q-item-label class="text-white" caption>
              By John Doe
            </q-item-label>
          </div>
        </q-card-section>
        <q-card-section>
          {{ lorem }}
        </q-card-section>
      </q-card>
        <q-card class="my-card">
      <q-card-section horizontal>
        <q-img
          class="col-5"
          src="https://cdn.quasar.dev/img/parallax1.jpg"
        />
        <q-card-section>
          {{ lorem }}
        </q-card-section>
      </q-card-section>
      <q-separator />
      <q-card-actions>
        <q-btn flat round icon="event" />
        <q-btn flat>
          5:30PM
        </q-btn>
        <q-btn flat>
          7:00PM
        </q-btn>
        <q-btn flat color="primary">
          Reserve
        </q-btn>
      </q-card-actions>
    </q-card>
  </div>
    <q-btn
      class="absolute-center"
      color="primary"
      icon="home"
      label="Go Home"
      @click="$router.replace('/')"/>
  </q-page>

</template>

<script>
export default {
  name: 'AboutMe',
  setup () {
    return {
      lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    }
  }
}
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 350px
</style>
