<template lang="html">
  <div class="nav container justify-content-end align-items-center margin-right-10 bg-color">
    <ul class="nav__list container margin-right-10">
      <li class="nav__list__item margin-10" v-for="title in base.nav.titleHeader"><router-link :to="{ path: title.url }">{{title.title}}</router-link></li>
    </ul>
  </div>
</template>

<script>
  import base from '@/static/data/base.json'

  export default {
    data() {
      return {
        base
      }
    }
  }
</script>

<style lang="scss" scoped>
  .nav {
      width: 100%;
      height: 80px;
    .nav__list {
      list-style: none;
    }
    .nav__list__item {
      font-size: 24px;
    }
  }
</style>
