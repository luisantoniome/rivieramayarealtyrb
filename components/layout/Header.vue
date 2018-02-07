<template lang="pug">
  header.container
    .logo
      h1
        router-link(to="/") {Logo}
    .burger
      a(@click="toggleMenu()")
        i.fa.fa-bars
    nav(v-show="showMenu")
      ul
        li(v-for="item in menuItems")
          router-link(:to="item.slug" @click.native="toggleMenu()") {{ item.name }}
</template>

<script>
  export default {
    data () {
      return {
        menuItems: [
          {
            name: 'Playa del Carmen',
            slug: 'playa'
          },
          {
            name: 'Tulum',
            slug: 'tulum'
          },
          {
            name: 'Nosotros',
            slug: 'nosotros'
          },
          {
            name: 'Contacto',
            slug: 'contacto'
          }
        ],
        showMenu: false
      }
    },

    methods: {
      toggleMenu() {
        this.showMenu = !this.showMenu
      }
    } 
  }
</script>

<style lang="stylus" scoped>
  header
    display flex
    flex-wrap wrap
    justify-content space-between
    align-items center

  h1
    font-size 1rem
    padding 5px

  .burger
    font-size 1.5rem
    padding 8px

  nav
    transition .2s all
    height calc(100vh - 10vh)
    width 100%

  ul
    height inherit
    list-style none
    padding 0
    display flex
    flex-direction column
    justify-content center
    align-items center

  li
    height 25%
    display flex
    align-items center
    text-transform uppercase
    font-weight 700
    a
      border-bottom 4px solid #1abc9c

  @media (min-width 1024px)
    header
      padding 1rem
    .burger
      display none
    nav
      display block !important
      height auto
      width auto
    ul
      flex-direction row
    li
      padding 0 1rem
      a
        font-size 1.2rem
        transition .2s all
        border-bottom-color transparent
        &:hover
          border-bottom 4px solid #1abc9c
        &:active
          color #1abc9c

  @media (min-width 1200px)
    li
      a
        font-size 1.5rem
</style>
