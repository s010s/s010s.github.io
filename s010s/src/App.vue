<template>
  <div id="app" class="flex flex-main-justify">
    <page-left-nav class="page-left-nav"></page-left-nav>
    <router-view class="flex-box-1"></router-view>
  </div>
</template>

<script>
  import pageHeader from '@/components/pageHeader'
  import pageLeftNav from '@/components/pageLeftNav'
  export default {
    name: 'app',
    components: {
      pageHeader,
      pageLeftNav
    }
  }

</script>

<style>
  [v-cloak] {
    display: none;
  }

  #app {
    width: 100%;
    height: 100%;
    overflow: hidden;
    /*background-image: url('./assets/images/bg_login.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: fixed;*/
  }

</style>
