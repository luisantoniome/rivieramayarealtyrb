<template lang="pug">
  .featured-text
    .container
      p
        | El momento de 
        span invertir
        |  en la Riviera Maya 
        span es ahora
        | , con 
        span retorno de inversión
        |  hasta de un 
        span 18 %
        | .
      button
        | Conoce más 
        i.fa.fa-angle-double-right
</template>

<style lang="stylus" scoped>
  .featured-text
    background linear-gradient(to bottom, #3498db, #16a085)
    color white
    text-align center
    padding 5rem 1rem
    p
      font-size 2rem
      line-height 3rem
      margin 1rem auto
      span
        font-weight 700

    @media (min-width 1024px)
      .featured-text
        padding 6rem 1rem
        p
          font-size 2.2rem
          line-height 4rem

    @media (min-width 1200px)
      .featured-text
        padding 7rem 1rem
        p
          font-size 2.5rem
</style>
