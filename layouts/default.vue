<template lang="pug">
  div
    rb-header
    nuxt
    rb-footer
</template>

<script>
  import RbHeader from '~/components/layout/Header.vue'
  import RbFooter from '~/components/layout/Footer.vue'

  export default {
    components: { RbHeader, RbFooter }
  }
</script>

<style lang="stylus">
  @import('../assets/stylus/main')
</style>
