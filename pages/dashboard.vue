<template>
  <main>
      <page-headline headline="Dashboard"></page-headline>
  </main>
</template>

<script>
import PageHeadline from '../components/PageHeadline.vue'
export default {
  components: { PageHeadline },
  layout: 'loggedIn'
}
</script>

<style lang="sass">
main
    padding: 1rem 3rem
</style>