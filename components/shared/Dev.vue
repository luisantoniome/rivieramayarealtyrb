<template lang="pug">
  .card
    .image
      img(src='https://images.unsplash.com/photo-1501855901885-8b29fa615daf', alt='')
    .info
      h3
        i.fa.fa-home
        |  Miranda Condos - 
        span Preventa
      p.units 32 unidades, desde $ 10,000 USD
      p
        i.fa.fa-caret-right
        |  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean lacus lorem, molestie eget eros quis, pretium elementum erat. Donec eu facilisis sapien, id tempus quam. Praesent id magna vel sapien posuere lobortis sed tempus ligula. Phasellus leo arcu, maximus id tortor eget, viverra eleifend dui.
      button
        | Ver más 
        i.fa.fa-angle-double-right
</template>

<style lang="stylus" scoped>
  .card
    display flex
    flex-direction column
    margin 2rem 0

  h3
    margin-bottom 1rem 0
    span
      border-bottom 3px solid #16a085

  .units
    margin .7rem 0

  button
    font-size 1rem
    margin .5rem 0

  @media (min-width 720px)
    .card
      flex-direction row
      margin 3rem 0
    .info
      padding 0 1rem
    img
      border-radius 4px
      max-width 300px

  @media (min-width 1024px)
    .card
      margin 5rem 0
    .info
      font-size 1.1rem
    h3
      font-size 1.5rem
</style>
