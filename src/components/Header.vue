<template>
    <header>
        <div>
            <img src="../assets/logo.svg" alt="Logo d'odissey sécurité privée">
            <h1>Odissey <br> <span>Sécurité Privée</span></h1>
        </div>
        <div>
            <i @click.prevent="showMenu()" v-if="windowWidth < 749 && !burgerMenuActive" class="fas fa-bars burger"></i>
            <i @click.prevent="showMenu()" v-if="windowWidth < 749 && burgerMenuActive" class="fas fa-times burger"></i>
            <div v-if="windowWidth > 748" class="menu-mobile">
                <ul> 
                    <li> <a href="">Accueil</a></li>
                    <li> <a href="">Nos services</a></li>
                    <li> <a href="">Nous contacter</a></li>
                    <li> <a href="">Nous rejoindre</a></li>
                </ul>
            </div>
            <div v-if="burgerMenuActive" class="menu-mobile-fixed">
                <ul> 
                    <li> <a href="">Accueil</a></li>
                    <li> <a href="">Nos services</a></li>
                    <li> <a href="">Nous contacter</a></li>
                    <li> <a href="">Nous rejoindre</a></li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="stylus" scoped>
@import '../css/variables'

header 
    display flex
    align-items center
    height 80px
    font-family $font
    background white
    justify-content space-between
    padding 0 80px
    border-bottom 1px solid #E5E9F2
    @media tablet 
        padding 0 50px
    @media mobile
        padding 0
        position fixed
        width 100%
        padding 0
    div
        display flex
        align-items center

h1
    font-size 32px
    font-weight black
    text-align center
    @media mobile
        display none
    span 
        position absolute
        font-size 12px
        font-weight regular
        color $black-color
img 
    height 50px
    margin-right 15px
    @media mobile 
        position relative
        left 30px

ul
    list-style-type none
    padding 0
    @media mobile
        display flex
        flex-direction column
        align-items center
        justify-content center
        width 100%

.menu-mobile
    @media mobile
        display none 

.menu-mobile-fixed
    @media mobile 
        position fixed 
        left 0
        top 80px
        width 100%
        background $black-color
        height calc(100vh - 80px)
        

li
    display inline-block
    margin 0 15px
    @media mobile 
        margin 20px 0


a
    color $black-color
    text-decoration none 
    font-weight 500
    font-size 14px
    &:hover
        text-decoration underline
    @media mobile 
        color $white-color
        font-size 25px
        font-weight bold
        text-transform uppercase
        &:hover
            text-decoration none

.burger
    font-size 20px
    @media mobile 
        position relative
        right 30px
</style>

<script>
export default {
    data() {
        return {
            windowWidth: 0,
            burgerMenuActive: false,
        }
    },

    mounted() {
        this.$nextTick(function() {
            window.addEventListener('resize', this.getWindowWidth);
            //Init
            this.getWindowWidth()
        })
    },

    methods: {
        getWindowWidth() {
            this.windowWidth = document.documentElement.clientWidth;
        },
        showMenu(){
            this.burgerMenuActive = !this.burgerMenuActive;
        }
    },

    beforeDestroy() {
        window.removeEventListener('resize', this.getWindowWidth);
        window.removeEventListener('resize', this.getWindowHeight);
    }
}
</script>