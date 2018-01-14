<template>
  <div>
    <home/>
    <arrowNav/>
  </div>
</template>

<script>
  import home from '@/pages/home'
  import arrowNav from '@/components/scroll-nav'

  export default {
    components: {
      home,
      arrowNav
    },
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss">
</style>
