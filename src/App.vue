<script setup>
import LandingPage from '@/pages/LandingPage.vue'
import logo from '@/assets/logo-texte.png'
import logoTigre from '@/assets/logo-tigre.svg'
</script>

<template>
  <header>
    <img class="logo" alt="Odissey logo" :src="logo" />
  </header>

  <main>
    <LandingPage/>
  </main>

  <footer>
    <img class="logo" alt="Odissey logo version tigre" :src="logoTigre" />
    <div>
      <p><b>Odissey Sécurité Privée</b></p>
      <p><a href="tel:0674554933">06 74 55 49 33</a></p>
      <p><a href="mailto:contact@odissey.fr">contact@odissey.fr</a></p>
      <p>4 Rue de la Croix Blanche <br>
        95370 Montigny-lès-Cormeilles</p>
    </div>
  </footer>
</template>

<style lang="stylus" scoped>
@import '/assets/variables.styl'


header
  display: flex
  width: 100%
  height: 80px
  margin-top: 40px
  margin-bottom: 40px
  @media tablet {
    margin-top 24px
    margin-bottom 24px
  }
  img
    height: 100%
    @media tablet
      height 64px

footer
  display: flex
  width 100%
  background: $white-color
  color: $black-color
  justify-content: space-between
  align-items: center
  padding 52px 80px
  img 
    height: 120px
    margin-right: 24px
    @media tablet
      max-height 80px
  p
    text-align: right
    margin-bottom: 8px
  a
    text-decoration: underline
    color: $black-color
  @media tablet
    padding 32px 16px

</style>
