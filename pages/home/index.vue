<template>
  <div class="container align-items-center margin-left-30 margin-right-30">
    <frontPage :title="personal.personal.presentName" :subTitle="personal.personal.subTitle" :message="personal.personal.message" :image="imageLink"/>
  </div>

</template>

<script>
  import appNav from '@/components/app-nav'
  import personal from '@/static/data/personal.json'
  import frontPage from '@/components/front-page'

  export default {
    components: {
      appNav,
      frontPage
    },
    data() {
      return {
        personal,
        imageLink: require('@/assets/img/landing.png')
      }
    }
  }
</script>

<style lang="scss" scoped>
  .container {
    min-height: calc(100vh -80px);
  }
</style>
