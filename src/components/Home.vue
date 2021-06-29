<template>
<div>
    <section class="discover">
    <div class="discover-text">
      <h1>Sécuriser votre business</h1>
      <h2>Odissey est une société de sécurité privée basée en Île-De-France, avec l'ambition d'offrir à nos clients un panel d'agents qualifiés qui vous protègeront des incendies, des agressions, des risques terroristes... </h2>
      <button>
        Découvrez nos références
      </button>
    </div>
    <div class="container-img">
      <img
        src="../assets/security-guard.jpg"
        alt="Photo d'un agent de sécurité"
      />
    </div>
  </section>
  <section>
    <div>

    </div>
  </section>
</div>
</template>

<style lang="stylus" scoped>
@import '../css/variables'

.discover
  display flex
  align-items center
  justify-content space-between
  min-height calc(100vh - 80px)
  padding 30px 80px
  background white
  color $black-color
.discover-text
  max-width 50%
  h1
    max-width 80%
    font-family $font
    font-size 72px
    line-height 98px
    font-weight bold
  h2
    max-width 80%
    margin 32px 0
    font-size 18px
    line-height 32px
  button
    background-color black
    color white
    padding 16px 32px
    border-radius 16px
    font-family $font
    font-weight 500
    cursor pointer
.container-img
  width 70vh
  height 70vh
  border-radius 50%
  background #D6B1FF
  overflow hidden
  position relative
  img
    position absolute
    top 0
    left 0
    height 100%
    object-fit contain


</style>
