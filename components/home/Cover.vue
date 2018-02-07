<template lang="pug">
  .cover
    .container.coverContent
      h2 ¿Qué buscas?
      .searchForm
        form
          .formItem
            label Ciudad
            select
              option Playa del Carmen
              option Cancún
          .formItem
            label Tipo
            select
              option Penthouse
              option Departamento
              option Estudio
          .formItem
            label Presupuesto
            .multipleBoxes
              select.budget
                option $ 50,000
                option $ 100,000
                option $ 150,000
              select.budget
                option USD
                option MXN
          .formItem
            button
              | Buscar 
              i.fa.fa-search
</template>

<style lang="stylus" scoped>
  .cover
    background-image url('https://images.unsplash.com/photo-1415018255745-0ec3f7aee47b')
    background-size cover
    background-position center
    text-align center
    height calc(100vh - 25vh)

  .coverContent
    display flex
    height inherit
    justify-content center
    flex-direction column

  h2
    font-size 2rem
    text-shadow 0 0 5px rgba(0, 0, 0, 0.2)
    color white

  form
    display flex
    flex-direction column

  .formItem
    display flex
    color white
    font-weight 700
    flex-direction column
    max-width 75vw
    font-size 1.5rem
    margin .5rem auto

  label
    text-shadow 0 0 5px rgba(0, 0, 0, 0.2)
    padding 5px

  option
    font-weight inherit

  .multipleBoxes
    select
      margin 0 5px

  @media (min-width 1024px)
    h2
      font-size 3rem
    form
      flex-direction row
      justify-content center
    .formItem
      font-size 1.8rem
      margin 1.5rem
      justify-content flex-end
      max-width auto
    select
      font-size 1.2rem
</style>
