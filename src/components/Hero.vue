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
          a(@click='$emit("setActive", "home")') home
        li
          a(@click='$emit("setActive", "projects")') projects
        li
          a(@click='$emit("setActive", "resume")') resume
        li
          a(@click='$emit("setActive", "blog")') blog
</template>

<script>
export default {
  name: 'Hero',
};
</script>

<style lang="sass" scoped>
section
  margin-bottom: 2rem
.is-three-quarters
  width: 75%
</style>
