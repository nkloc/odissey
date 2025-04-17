
<script setup>
</script>

<template>
    <section>
        <h2>
            On adapte nos services à vos besoins,
            <br> sur ces <u>cinq secteurs</u>.
        </h2>
        <div class="besoins">
            <div class="line"></div>
            <article>
                <div class="article-left">
                    <h1>01</h1>
                    <div>
                        <h3>Secteur aéroportuaire</h3>
                        <p>Surveillance des installations, contrôle des accès, gestion des flux de passagers et de marchandises, protection des zones sensibles.</p>
                    </div>
                </div>
                <img src="../assets/besoins/aeroportuaire.png" alt="Notre coeur d'activité numéro 1 : le secteur aéroportuaire.">
            </article>
            <div class="line"></div>
            <article>
                <div class="article-left">
                    <h1>02</h1>
                    <div>
                        <h3>Grande distribution</h3>
                        <p>Sécurisation des surfaces de vente, prévention des vols, protection des clients et des employés, gestion des situations d’urgence.</p>
                    </div>
                </div>
                <img src="../assets/besoins/grande-distribution.png" alt="Notre coeur d'activité numéro 2 : la grande distribution.">
            </article>
            <div class="line"></div>
            <article>
                <div class="article-left">
                    <h1>03</h1>
                    <div>
                        <h3>Secteur tertiaire</h3>
                        <p>Sécurité des bureaux et des sièges sociaux, contrôle des accès, gestion des flux de visiteurs, surveillance des installations.</p>
                    </div>
                </div>
                <img src="../assets/besoins/tertiaire.png" alt="Notre coeur d'activité numéro 3 : l'activité tertiaire.">
            </article>
            <div class="line"></div>
            <article>
                <div class="article-left">
                    <h1>04</h1>
                    <div>
                        <h3>Logistique</h3>
                        <p>Surveillance des entrepôts et des zones de stockage, protection des marchandises, contrôle des accès et des flux de transport.</p>
                    </div>
                </div>
                <img src="../assets/besoins/logistique.png" alt="Notre coeur d'activité numéro 4 : la logistique.">
            </article>
            <div class="line"></div>
            <article>
                <div class="article-left">
                    <h1>05</h1>
                    <div>
                        <h3>Événementiel</h3>
                        <p>Sécurité des événements, gestion des foules, contrôle des accès, protection des personnalités et des participants.</p>
                    </div>
                </div>
                <img src="../assets/besoins/evenement.png" alt="Notre coeur d'activité numéro 5 : l'évènementiel.">
            </article>
            <div class="line"></div>
            
        </div>
    </section>
</template>

<style lang="stylus" scoped>
@import '../assets/variables.styl'
section
    display: flex
    background: $white-color
    flex-direction: column
    justify-content: space-between
    align-items: center
    padding-top 80px
    padding-bottom 40px
    width: 100%
    gap: 80px
    @media tablet {
        padding-top 60px
        gap: 60px
        padding-bottom 0
    }

.line
    width 100%
    background: $grey-color
    height 1px
    @media tablet {
        display: none
    }

.besoins
    width: 100%
    display flex
    flex-direction: column
    gap: 52px
    align-items: center
    @media tablet {
        gap: 24px
    }

article
    display: flex
    width 100%
    justify-content: space-around
    align-items: center
    @media tablet {
        flex-direction: column-reverse
        align-items: flex-start
    }
    .article-left
        display: flex
        gap: 32px
        @media tablet {
            gap: 16px
            align-items: flex-start
        }
        h1
            position relative
            top: -32px
            @media tablet {
                top -12px
            }
        h3
            margin-bottom 8px
    p
        max-width 600px

img
    width: 33%
    margin-left: 24px
    height auto
    filter: grayscale(1);
    @media tablet {
        width: 100%
        margin-bottom: 24px
        margin-left 0
    }

h1, h2, h3, p
    color $black-color
</style>
