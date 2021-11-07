<template>
  <aside>
      <span class="app-name">Contactor</span>
      <nav>
          <ul>
              <li>
                  <nuxt-link to="/dashboard">Dashboard</nuxt-link>
              </li>
              <li>
                  <nuxt-link to="/contacts">Contacts</nuxt-link>
              </li>
          </ul>
      </nav>
  </aside>
</template>

<script>
export default {

}
</script>

<style lang="sass" scoped>
aside
    background: $blue
    min-height: 100vh
    min-width: 200px

    .app-name
        padding: 1.5rem
        padding-left: 2.5rem
        color: $white
        display: block

    ul
        padding: 0
        margin: 0
        list-style: none
        a
            display: block
            padding: 1.5rem
            padding-left: 2.5rem
            color: $white
            text-decoration: none
            &:hover
                background: $lighterBlue

</style>