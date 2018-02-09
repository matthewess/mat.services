<template lang="pug">
.nuxt
  Hero
  .container
    nuxt
  footer.footer.white
</template>

<script>
import Hero from '../components/Hero.vue';

export default {
  components: { Hero },
};
</script>

<style lang="sass">
@import '~assets/sass/mat'
</style>
