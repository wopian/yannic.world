<template lang="pug">
  footer.navbar
    .container.nav
      .navbar-text Copyright © {{ thisYear }}, Yannic Geurts
</template>

<script>
  export default {
    data () {
      return {
        thisYear: new Date().getFullYear()
      }
    }
  }
</script>

<style lang="sass" scoped>
  @import '../styles/variables'

  footer
    height: 5rem
    margin-top: 2rem
    justify-content: center
    border-top: 1px solid rgba($black, .05)
    background: darken($white, 4)

  .navbar-text
    text-align: center
    width: 100%
</style>
