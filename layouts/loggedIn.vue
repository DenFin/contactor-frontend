<template>
  <div class="wrapper">
    <Sidebar />
    <Nuxt />
  </div>
</template>

<script>
import Sidebar from "./../components/sidebar"

export default {
  components: {
    Sidebar
  }
}
</script>

<style lang="sass">

*
  box-sizing: border-box

html
  font-size: 62.5%

body
  margin: 0
  font-family: 'Poppins', sans-serif
  font-size: 1.6rem

h1
  font-size: 2.8rem

.wrapper
    display: flex

.nuxt-link-exact-active
    background: $lighterBlue

</style>