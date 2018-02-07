<template lang="pug">
  div
    rb-header
    nuxt
    rb-contact-form
    rb-footer
</template>

<script>
  import RbHeader from '~/components/layout/Header.vue'
  import RbFooter from '~/components/layout/Footer.vue'
  import RbContactForm from '~/components/layout/ContactForm.vue'

  export default {
    components: {
			RbHeader,
			RbFooter,
			RbContactForm
    }
  }
</script>

<style lang="stylus">
  @import('../assets/stylus/main')
  
  .cover
    background-image url('https://images.unsplash.com/photo-1461637908059-3c43f42f8fe0')
    background-size cover
    background-position center
    text-align center
    height calc(100vh - 50vh)

  .coverContent
    display flex
    height inherit
    justify-content center
    flex-direction column

  h2
    color white
    font-size 2rem
    text-shadow 0 0 5px rgba(0, 0, 0, 0.2)
  
  .devs
    padding 1rem
</style>
