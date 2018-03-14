<template lang="pug">
section.hero.is-primary.is-bold.is-medium(v-once)
  .hero-body
    .container
      h1.title.has-text-warning matthew ess
      h2.subtitle.has-text-warning software developer, social justice warrior, wannabe artist
  .hero-foot
    .tabs.is-boxed.is-fullwidth.is-three-quarters
      ul.has-text-weight-semibold.has-text-warning
        li
          nuxt-link(to='/') home
        li
          nuxt-link(to='/projects') projects
        li
          nuxt-link(to='/resume') resume
</template>

<style lang="sass" scoped>
@import '~bulma/sass/utilities/mixins'

section
  margin-bottom: 2rem
+desktop
  .is-three-quarters
    width: 75%
</style>
