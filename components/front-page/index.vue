<template lang="html">
  <div class="front-page container-colunm">
    <h1 class="front-page__title">{{title}}</h1>
    <p class="front-page__message">{{message}}</p>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String
    },
    message: {
      type: String
    }
  }
}
</script>

<style lang="css" scoped>
  .front-page {
    height: calc(100vh - 80px);
    width: 50%;
  }
</style>
