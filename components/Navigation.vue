<template lang="pug">
.navigation
  .container
    .logo
      | Green
    .menu(:class="{open: open}")
      nav
        .menu-item(v-for="item in menuItem") {{ item }}
    .hamburger(@click="toggle()", :class="{open: open}")
      span =
</template>

<script>
export default {
  data () {
    return {
      menuItem: ['Home', 'About', 'Gallery', 'Contact'],
      open: false
    }
  },
  methods: {
    toggle () {
      this.open = !this.open
    }
  }
}
</script>

<style lang="sass" scoped>

$green: #B2D430
$header-height: 4rem

.navigation
  background: #FFF
  .container
    max-width: 1200px
    height: $header-height
    margin: 0 auto
    display: flex
    justify-content: space-between
    align-items: center
    position: relative
  .hamburger
    position: absolute
    right: 0
    font-size: 2rem
    font-weight: bold
    display: none
    height: $header-height
    width: $header-height
    padding: 0.5rem 0 0 1rem
    cursor: pointer
    z-index: 2
    

  .menu
    nav
      display: flex
      .menu-item
        padding: 1rem


  @media (max-width: 600px) 
    .hamburger
      display: block
    .menu
      display: none
    .menu.open
      display: block

  @media (max-width: 600px)
    .menu nav
      flex-direction: column
      background: #000
      color: #FFF
      position: fixed
      right: 0
      top: 0
      bottom: 0
      width: 15rem
      padding-top: 4rem
      .menu-item
        padding: 1rem 2rem
    .hamburger.open
      background: #000
      color: #FFF

</style>
