<template>
  <h1 class="page-headline">{{ headline }}</h1>
</template>

<script>
export default {
    props: ['headline']
}
</script>

<style lang="sass" scoped>
h1.page-headline
    +h1

</style>