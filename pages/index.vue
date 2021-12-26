<template>
  <v-app>
    <Hero />
    <DisplayCards :title="dhaka" />
  </v-app>
</template>

<script>
import DisplayCards from '../components/DisplayCards.vue'
export default {
  components: { DisplayCards },
}
</script>
