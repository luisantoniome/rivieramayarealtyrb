<template lang="pug">
  main
    rb-cover
    rb-last
    rb-featured
    rb-contact-form
</template>

<script>
  import RbCover from '~/components/home/Cover.vue'
  import RbLast from '~/components/home/Last.vue'
  import RbFeatured from '~/components/home/Featured.vue'
  import RbContactForm from '~/components/layout/ContactForm.vue'

  export default {
    components: {
      RbCover,
      RbLast,
      RbFeatured,
      RbContactForm
    }
  }
</script>
