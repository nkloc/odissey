
<script setup>
</script>

<template>
    <section>
        <div class="text">
            <h1>sécurité claire, <br>confiance solide</h1>
            <p>
                <b>Odissey Sécurité Privée</b> est dédiée à la protection des biens et des personnes dans des secteurs sensibles et variés. <br> <br> Forts d'une expérience et de notre expertise, nous intervenons principalement dans le secteur aéroportuaire, la grande distribution ainsi que dans les domaines du tertiaire, de la logistique et de l'événementiel.
            </p>
        </div>
        <img alt="Odissey tigre" src="../assets/tigre.svg"/>
    </section>
</template>

<style lang="stylus" scoped>
@import '../assets/variables.styl'

section
    height calc(100vh - 160px)
    display: flex
    justify-content: space-between
    align-items: flex-end
    overflow: hidden
    @media tablet {
        overflow: visible
        height: auto
        flex-direction: column
        align-items: center
        justify-content center
    }

.text
    display: flex
    flex-direction: column
    margin-bottom 160px
    @media tablet 
        margin-bottom: 0px
        text-align: center
        max-width: 75%
    @media mobile
        max-width: 100%
        text-align: left

img
    position relative
    top 20px
    @media tablet
        width: 45%
        top 0
        left 100px

h1
    margin-bottom 52px
    @media tablet
        margin-bottom: 24px

p
    max-width 800px
    @media tablet {
        max-width: none
    }
</style>
