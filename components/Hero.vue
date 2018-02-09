<template lang="pug">
section.hero.is-primary.is-bold.is-medium(v-once)
  .hero-body
    .container
      h1.title matthew ess
      h2.subtitle software developer, social justice warrior, wannabe artist
  .hero-foot
    .tabs.is-boxed.is-fullwidth.is-three-quarters
      ul.has-text-weight-semibold
        li
          nuxt-link(to='/') home
        li
          nuxt-link(to='/projects') projects
        li
          nuxt-link(to='/resume') resume
        li
          nuxt-link(to='/blog') blog
</template>

<style lang="sass" scoped>
@import '~bulma/sass/utilities/mixins'

section
  margin-bottom: 2rem
+desktop
  .is-three-quarters
    width: 75%
</style>
