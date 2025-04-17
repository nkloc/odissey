
<script setup>
</script>

<template>
    <section>
        <h2>
            Des professionnels formés et qualifiés,
            <br> prêts à intervenir.
        </h2>
        <div class="profils">
            <div class="profil">
                <img src="../assets/profils/agent-de-securite.png" alt="Image montrant un agent de sécurité en train de parler dans un talkie-walkie">
                <h3>Agents de <br> sécurité</h3>
                <p>Assurent la surveillance et la protection des sites, le contrôle des accès, et la prévention des risques.</p>
            </div>
            <div class="profil">
                <img src="../assets/profils/incendie.png" alt="Image montrant un agent de sécurité incendie">
                <h3>Agents de sécurité incendie</h3>
                <p>Spécialistes de la prévention des risques d’incendie et des interventions en cas d’urgence, ils veillent à la sécurité des installations et des personnes.</p>
            </div>
            <div class="profil">
                <img src="../assets/profils/cynophile.png" alt="Image montrant un agent de sécurité cynophile avec son chien">
                <h3>Agents <br> cynophiles</h3>
                <p>Utilisant l’expertise conjointe d’un agent de sécurité et d’un chien, ces équipes sont particulièrement efficaces dans les environnements nécessitant une vigilance accrue.</p>
            </div>
        </div>
    </section>
</template>

<style lang="stylus" scoped>
@import '../assets/variables.styl'
section
    display: flex
    flex-wrap: wrap
    flex-direction: column
    justify-content: space-around
    align-items: center
    padding 80px 0
    max-width: 100%
    gap: 80px
    @media tablet {
        gap: 60px
        padding-bottom 60px
    }
h2
    color $white-color

.profils
    display: flex
    align-content: center
    gap: 40px
    flex-wrap: wrap
    justify-content: center

.profil
    display: flex
    flex-direction: column
    max-width: 400px
    padding 40px 20px
    border: 1px solid $white-color
    align-items: center
    text-align: center
    border-radius 8px
    @media tablet {
        max-width: 75%
        padding 20px 10px
    }
    h3
        margin 48px 0
        @media tablet {
            margin: 16px 0
        }
    img
        width: 150px
        filter: grayscale(1);
</style>
