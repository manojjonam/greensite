<template lang="pug">
.container
    //- HeaderNav
    Navigation
    //- Carousel
</template>

<script>

import Navigation from '../components/Navigation.vue'
import HeaderNav from '../components/HeaderNav.vue'
import Carousel from '../components/Carousel.vue'
export default {
  components: {
      Navigation,
      HeaderNav,
      Carousel
  }
}
</script>

<style lang="sass">
body
    background: #7e8890
</style>

