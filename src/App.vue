<template lang="pug">
#app
  Hero(@setActive='tab => active = tab')
  .container
    component(:is='active')
  footer.footer.blue
</template>

<script>
import Hero from '@/components/Hero';
import Home from '@/containers/Home';
import Projects from '@/containers/Projects';
import Resume from '@/containers/Resume';
import Blog from '@/containers/Blog';

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

$pink: #f8a5c2
$pink-invert: findColorInvert($pink)
$purple: #786fa6
$purple-invert: findColorInvert($purple)
$blue: #546de5
$blue-invert: findColorInvert($blue)
$charcoal: #3a435e
$charcoal-invert: findColorInvert($charcoal)

$primary: $pink
$primary-invert: $pink-invert
$info: $blue
$info-invert: $blue-invert
$danger: $purple
$danger-invert: $purple-invert
$warning: $charcoal
$warning-invert: $charcoal-invert

@import '~bulma/bulma'

.blue
  background: white
</style>
