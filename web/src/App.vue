<template>
  <div id="app">
    <v-header/>
    <div class="container">
      <v-nav/>
      <router-view/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    'v-header': () => import('@/components/header'),
    'v-nav': () => import('@/components/nav')
  }
}
</script>

<style lang="scss">
  @import 'assets/css/common.scss';

  #app > div.container {
    margin-top: 80px;
  }

</style>
