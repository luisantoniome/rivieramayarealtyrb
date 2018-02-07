<template lang="pug">
  .main
    .container
      h3 No dudes en contactarnos
      section
        form
          .formItem
            input(type='text', placeholder='Nombre')
          .formItem
            input(type='email', placeholder='Correo electrónico')
          .formItem
            input(type='text', placeholder='Teléfono')
          .formItem
            textarea(placeholder='Mensaje')
          .formItem
            button Enviar mensaje
</template>

<style lang="stylus" scoped>
  .main
    background linear-gradient(to bottom, #34495e, #2c3e50)
    background #34495e
    padding 2rem
    text-align center

  h3
    color white

  section
    padding 1rem

  .formItem
    margin 1rem auto

  input, textarea
    min-width 70%
    max-width 90%

  textarea
    min-height 150px

  @media (min-width 1024px)
    .main
      padding 5rem 2rem
    form
      display flex
      flex-wrap wrap
      justify-content center
    .formItem
      margin 1rem
      &:nth-child(4)
        width 100%
    input,
    textarea
      min-width auto
      font-size 1.1rem
    textarea
      min-width 100%
    
    h3
      font-size 2rem

  @media (min-width 1200px)
    input,
    textarea
      font-size 1.2rem
</style>
