<template lang="pug">
  .main.container
    h3 Últimos desarrollos en preventa
    section
      router-link(to='playa')
        .card.playa
          h4 Playa del Carmen
      a(href='/tulum')
        .card.tulum
          h4 Tulum
</template>

<style lang="stylus" scoped>
  .main
    padding 1rem
    text-align center

  h3
    font-size 1.5rem

  section
    display flex
    flex-direction column

  .card
    border-radius 3px
    box-shadow 0 0 5px rgba(0, 0, 0, 0.3)
    max-width 70vw
    min-width 300px
    padding 4rem
    margin 1rem auto
    cursor pointer
    transition .2s all
    &:active
      transform scale(.9)

  h4
    color white
    font-size 1.1rem
    text-shadow 0 0 15px rgba(0, 0, 0, 1)

  .playa
    background-image url('https://images.unsplash.com/photo-1461637908059-3c43f42f8fe0')

  .tulum
    background-image url('https://images.unsplash.com/photo-1473798349978-d18a8c8dbf41')

  .playa,
    .tulum
      background-size cover
      background-position center

  @media (min-width 1024px)
    .main
      padding 3rem
    h3
      font-size 2rem
    section
      flex-direction row
      justify-content center
      padding 2rem
    .card
      margin 1rem
      min-width 400px
      padding 6rem 4rem
    h4
      font-size 1.5rem
      text-shadow 0 0 15px rgba(0, 0, 0, 1)
</style>
