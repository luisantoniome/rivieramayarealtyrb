<template lang="pug">
  main
    .cover
      .container.coverContent
        h2 Tulum
    .devs.container
      rb-dev(v-for='i in devs', :key='i')
</template>

<script>
  import RbDev from '~/components/shared/Dev.vue'

  export default {
    layout: 'city',

    components: { RbDev },

    data () {
      return {
        devs: [1, 2, 3, 4]
      }
    }
  }
</script>
