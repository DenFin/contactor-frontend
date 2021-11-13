<template>
  <div class="page">
      <div>
        <h1>404</h1>
        <h2>Page Not Found</h2>
        <nuxt-link class="btn" to="/">Go to homepage</nuxt-link>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Error404'
}
</script>

<style lang="sass" scoped>
.page
    min-height: 100vh
    display: flex
    justify-content: center
    align-items: center

    div, h1, h2, a
        text-align: center

    h1
        color: $blue
        font-size: 5.4rem
        margin-bottom: 0
        @media($desktop)
            font-size: 14rem


</style>