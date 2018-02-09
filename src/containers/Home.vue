<template lang="pug">
#home
  .tile.is-ancestor
    .tile.is-vertical.is-4
      .tile.is-9
        .notification.is-info
          h1.title.is-4 me
          p.content.
            i'm a communist, a
            #[a(href='https://mattandmack.website' target='_blank') spouse-to-be],
            a recently graduated student, and a software developer at yelp.
      .tile.placeholder.notification.is-white
      .tile.is-9
        .notification.is-warning
          h1.title.is-4 what's inspiring me now
          .content
            p david lynch's twin peaks
            p the musical stylings of #[a(href='https://mitski.com/' target='_blank') mitski]
            p jeff vandermeer's southern reach trilogy
    .tile.is-4
      .tile.is-9
        .notification.is-danger
            h1.title.is-4 what i care about
            p.content.
              as a communist, i'm passionate about anti-imperialism and decolonization.
              i believe that software can be a tool for liberation, and those are the tools
              i want to develop. feel free to get in touch with
              me at mess [at] yelp [dot] com if you have similar goals.
            p.content.
              "the philosophers have only interpreted the world, in various ways.
              the point, however, is to change it."
    .tile.is-4
      figure.image
        img(src='@/assets/me.png')
</template>

<script>
export default {
  name: 'Home',
};
</script>

<style lang="sass" scoped>
.placeholder
  height: 1rem
</style>
