<template>
<div>
    <section class="discover">
    <div class="discover-text">
      <h1>Sécuriser votre business</h1>
      <h2>Odissey est un partenaire de groupe spécialisée dans la surveillance humaine basée en Île-De-France, dont l'ambition est d'offrir à ses clients un panel d'agents qualifiés qui vous protègeront des incendies, des agressions, des risques terroristes... </h2>
      <button>
        Découvrez nos agents
      </button>
    </div>
    <div class="container-img">
      <img
        src="../assets/security-guard.jpg"
        alt="Photo d'un agent de sécurité"
      />
    </div>
  </section>
  <section class="agents">
    <div class="agents-text">
      <h2>Nos différents profils d'agents</h2>
    </div>
    <div class="agents-profiles-container">
      <article class="agents-profiles">
        <h3>Agent SSIAP 1</h3>
        <p>Les agents SSIAP1 ont pour mission d’assurer la sécurité des personnes et la sécurité incendie des biens.</p>
      </article>
      <article class="agents-profiles">
        <h3>Agent SSIAP 1</h3>
        <p>Les agents SSIAP1 ont pour mission d’assurer la sécurité des personnes et la sécurité incendie des biens.</p>
      </article>
      <article class="agents-profiles">
        <h3>Agent SSIAP 1</h3>
        <p>Les agents SSIAP1 ont pour mission d’assurer la sécurité des personnes et la sécurité incendie des biens.</p>
      </article>
      <article class="agents-profiles">
        <h3>Agent SSIAP 1</h3>
        <p>Les agents SSIAP1 ont pour mission d’assurer la sécurité des personnes et la sécurité incendie des biens.</p>
      </article>
      <article class="agents-profiles">
        <h3>Agent SSIAP 1</h3>
        <p>Les agents SSIAP1 ont pour mission d’assurer la sécurité des personnes et la sécurité incendie des biens.</p>
      </article>

    </div>
  </section>
</div>
</template>

<style lang="stylus" scoped>
@import '../css/variables'
@import '../css/home/discover'
@import '../css/home/agents'

section
  display flex
  min-height calc(100vh - 80px)
  padding 30px 80px
  background white
  color $black-color
</style>
