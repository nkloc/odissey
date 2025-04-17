
<script setup>
</script>

<template>
    <section>
        <h2>
            Parce que la sécurité
            <br>ne s’improvise pas.
        </h2>
        <div class="container">
            <div class="engagements">
                <article>
                    <div class="article-left">
                        <h1>01</h1>
                        <div>
                            <h3>Formation continue</h3>
                            <p>Nous investissons dans la formation continue de nos agents pour assurer un service de qualité et une sécurité à la pointe des exigences.</p>
                        </div>
                    </div>
                </article>
                <article>
                    <div class="article-left">
                        <h1>02</h1>
                        <div>
                            <h3>Innovation adaptée</h3>
                            <p>Bien que nous privilégions des solutions éprouvées, nous restons ouverts à l’intégration de technologies nouvelles adaptées aux besoins de nos clients.</p>
                        </div>
                    </div>
                </article>
                <article>
                    <div class="article-left">
                        <h1>03</h1>
                        <div>
                            <h3>Respect des normes</h3>
                            <p>Nos services respectent les normes les plus strictes en matière de sécurité, de prévention et d’intervention.</p>
                        </div>
                    </div>
                </article>
            </div>
            <img alt="Agent de sécurité de dos" src="../assets/engagements/securite.png"/>
        </div>
    </section>
</template>

<style lang="stylus" scoped>
@import '../assets/variables.styl'
section
    display: flex
    flex-direction: column
    justify-content: space-between
    align-items: center
    padding-top 40px
    padding-bottom 40px
    width: 100%
    gap: 80px
    @media tablet {
        padding-top 0
        gap: 60px
    }

.container
    display: flex
    width: 100%
    justify-content: space-around
    align-items: center
    gap: 52px
    @media tablet {
        flex-direction: column
        gap: 24px
    }

.engagements
    display flex
    flex-direction: column
    gap: 52px
    align-items: center
    @media tablet
        gap: 24px
        justify-content: center

article
    display: flex
    width 100%
    justify-content: space-around
    align-items: center
    .article-left
        display: flex
        gap: 32px
        h1
            position relative
            top: -32px
            @media tablet {
                top: -12px
                width 24px
            }
        h3
            margin-bottom 8px
            @media tablet
                width 100%
    p
        max-width 600px
        @media tablet
            width: 100%

img
    width: 33%
    height auto
    filter: grayscale(1);
    @media tablet {
        width: 100%
    }

</style>
