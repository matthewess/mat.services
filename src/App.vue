<template lang="pug">
#app
  Hero(@setActive='tab => active = tab')
  .container
    component(:is='active')
  footer.footer.white
</template>

<script>
import Hero from './components/Hero.vue';
import Home from './containers/Home.vue';
import Projects from './containers/Projects.vue';
import Resume from './containers/Resume.vue';
import Blog from './containers/Blog.vue';

export default {
  name: 'App',
  components: {
    Hero,
    Home,
    Projects,
    Resume,
    Blog,
  },
  data() {
    return { active: 'Home' };
  },
};
</script>

<style lang="sass">
@import '~bulma/sass/utilities/initial-variables'
@import '~bulma/sass/utilities/functions'

$pink: #ffa69e
$pink-invert: findColorInvert($pink)
$mint: #a5ffd6
$mint-invert: findColorInvert($mint)
$red: #ff686b
$red-invert: findColorInvert($red)

$primary: $pink
$primary-invert: $pink-invert
$info: $mint
$info-invert: $mint-invert
$danger: $red
$danger-invert: $red-invert

@import '~bulma/bulma'

.white
  background: white
</style>
