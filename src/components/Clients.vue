
<script setup>
</script>

<template>
    <section>
        <h2>
            Ils nous font confiance. <br>
            Pourquoi pas vous ?
        </h2>
        <div class="clients">
            <img class="client" alt="Auchan, Client d'odissey" src="../assets/clients/auchan.svg"/>
            <img class="client" alt="Paris Aéroport, Client d'Odissey" src="../assets/clients/roissy.svg"/>
            <img class="client" alt="Paris Aéroport, Client d'Odissey" src="../assets/clients/roissy.svg"/>
            <img class="client" alt="Paris Aéroport, Client d'Odissey" src="../assets/clients/roissy.svg"/>
            <img class="client" alt="Paris Aéroport, Client d'Odissey" src="../assets/clients/roissy.svg"/>
            <img class="client" alt="Paris Aéroport, Client d'Odissey" src="../assets/clients/roissy.svg"/>
            <img class="client" alt="Paris Aéroport, Client d'Odissey" src="../assets/clients/roissy.svg"/>

        </div>
    </section>
</template>

<style lang="stylus" scoped>
@import '../assets/variables.styl'
section
    display: flex
    flex-wrap: wrap
    background: $white-color
    flex-direction: column
    justify-content: space-around
    align-items: center
    padding 80px 0
    max-width: 100%
    gap: 80px
    @media tablet {
        gap: 60px
        padding-top 60px
    }
h2
    color $black-color
.clients
    display: flex
    gap: 24px
    width: 100%
    flex-wrap: wrap
    justify-content: center
    @media tablet
        gap 12px
    img
        width: auto
        @media tablet
            width 45%
</style>
