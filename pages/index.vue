<template>
  <div class="page">
    <section id="start">
      <div class="container">
        <div class="row">
          <div class="col-xs-12 col-lg-6">
            <h1>Manage your contacts in a super innovative way</h1>
            <p>
              This is a project by <a href="">aabhaskrjha</a> and <a href="">denfin</a>. Sign up for free now!
            </p>
            <nuxt-link to="/signup" class="btn">Sign up</nuxt-link>
          </div>
          <div class="col-xs-12 col-lg-6">
            <img src="~/static/img/Email_SVG.svg" alt="">
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  layout: 'default'
}
</script>

<style lang="sass" scoped>
$blue: #0a2463
$lighterBlue: #144bc9
$white: #ffffff

// .row
//   @media($smallDevices)
//     flex-direction: column-reverse

.page
  background: $blue
  color: $white

  h1
    margin-top: 0
    line-height: 1.3
    font-weight: bold
    font-size: 2.8rem

    @media($laptop)
      font-size: 4.8rem

  p
    font-size: 2rem


#start
  min-height: 100vh
  display: flex
  align-items: center

a
  color: $white

img
  max-width: 400px
  margin: 0 auto
  display: block
  filter: grayscale(1)

.btn
  background: $lighterBlue
  border: none
  color: $white
  cursor: pointer
  display: inline-block
  font-size: inherit
  padding: .75em 1.5em
  margin-top: 2rem
  min-width: 170px
  text-align: center
  text-decoration: none

  transition: background .35s ease

  &:hover
      background: lighten($lighterBlue, 10%)

</style>
