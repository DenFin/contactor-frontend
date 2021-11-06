<template>
  <div class="page">
      <div>
        <h1>You Are Almost There</h1>
        <p>We sent you an E-Mail with a verification link. Please visit this link to verfiy your account.</p>
        <nuxt-link class="btn" to="/login">Log in</nuxt-link>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="sass" scoped>
.page
    display: flex
    justify-content: center
    align-items: center
    min-height: 100vh

</style>