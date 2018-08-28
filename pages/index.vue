<template lang="pug">
.container
 //-HeaderNav
 Navigation
 //-Carousel
 imageslide
 tile
 Banner2
 tile
 FooterNav
</template>

<script>

import Navigation from '../components/Navigation.vue'
import HeaderNav from '../components/HeaderNav.vue'
import Carousel from '../components/Carousel.vue'
import imageslide from '../components/imageslide.vue'
import Tile from '../components/Tile.vue'
import Banner2 from '../components/Banner2.vue'
import Tile2 from '../components/Tile2.vue'
import FooterNav from '../components/FooterNav.vue'
export default {
  components: {
      Navigation,
      HeaderNav,
      Carousel,
      imageslide,
      Tile,
      Banner2,
      Tile2,
      FooterNav
  }
}
</script>

<style lang="sass">

body
    background: #7e8890
</style>

