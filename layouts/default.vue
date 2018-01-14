<template>
  <div id="app" class="bg-color">
    <appNav/>
    <nuxt/>
  </div>
</template>

<script>
  import appNav from '@/components/app-nav'

  export default {
    name: 'app',
    components: {
      appNav
    },
    mounted() {},
    data() {
      return {}
    }
  }
</script>

<style lang="scss">
  @import './assets/css/main.scss';

  #app {
    min-height: 100vh;
  }
</style>
