<template lang="html">
  <div class="front-page container justify-content-between">
    <div class="front-page__console container-column">
      <vue-typer text='Test'></vue-typer>
      <h1 class="front-page__title">{{title}}</h1>
      <h2 class="front-page__sub-title">{{subTitle}}</h2>
      <p class="front-page__message">{{message}}</p>
    </div>
    <div class="front-page__canvas container-column">
      <img class="front-page__canvas__img" v-bind:src="image" alt="">
    </div>
  </div>
</template>

<script>
  export default {
    components: {
    },
    props: {
      title: {
        type: String
      },
      subTitle: {
        type: String
      },
      message: {
        type: String
      },
      image: {
        type: String
      }
    }
  }
</script>

<style lang="scss" scoped>
  .front-page {
    height: calc(100vh - 80px);
    width: 100%;
    margin-left: 3vw;
    .front-page__console,
    .front-page__canvas {
      width: 40%;
      .front-page__canvas__img {
        width: 100%;
      }
    }
  }
</style>
