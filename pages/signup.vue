<template>
  <div class="page">
      <section class="left">
        <div class="container">
            <div class="row">
                <div class="col-xs-12">
                    <div>
                        <span class="app-name">Contactor</span>
                    </div>
                    <div>
                        <h1>Create Your Free Account</h1>
                        <p>
                            Already have an Account? <nuxt-link to="/login">Log in</nuxt-link>
                        </p>
                        <form>
                            <input v-model="email" type="email" name="email" placeholder="E-Mail"><br>
                            <input v-model="password" type="password" name="password" placeholder="Password"><br>
                            <button class="btn btn--submit" @click.prevent="submit" type="submit">Sign up</button>
                        </form>
                    </div>
                    <div>
                        <ul>
                            <li><a href="">aabhaskrjha </a></li>
                            <li><a href="">denfin</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section class="right">
        <img src="~/static/img/Email_SVG.svg" alt="">
    </section>
  </div>
</template>

<script>
import axios from "axios"

export default {
    data(){
        return {
            email: '',
            password: ''
        }
    },
    methods: {
        submit(){
            const res = axios({
                method: 'post',
                url: 'https://contactor.herokuapp.com/auth/signup',
                data: {
                    email: this.email,
                    password: this.password
                } 
            })
                .then( function(response){
                    console.log(response)
                })
        }
    }
}
</script>

<style lang="sass" scoped>
$blue: #0a2463
$lighterBlue: #144bc9
$white: #ffffff

.page
    display: flex
    justify-content: center
    align-items: center
    min-height: 100vh

.left,
.right
    min-height: 100vh
    display: flex
    justify-content: center
    align-items: center

.left
    width: 30%


.right
    background: $blue
    width: 70%

h1
    margin-bottom: 0

p
    color: #999
    font-size: 1.4rem
    margin-top: 0
    margin-bottom: 4rem

a
    color: $blue
    font-weight: bold

input,
.btn
    font-family: inherit

input
    display: block
    font-size: inherit
    padding: .75em
    width: 100%

.btn
    background: $blue
    border: none
    color: $white
    cursor: pointer
    display: block
    font-size: inherit
    padding: .75em 1.5em
    width: 100%

    transition: background .35s ease

    &:hover
        background: lighten($blue, 10%)


img
    max-width: 700px
    filter: grayscale(1)


.app-name
    color: $lighterBlue
    font-weight: bold
    margin-bottom: 12rem
    display: block

ul
    list-style: none
    margin: 0
    padding: 0
    margin-top: 8rem

li
    display: inline-block

    a
        display: block
        font-size: 1.4rem

</style>